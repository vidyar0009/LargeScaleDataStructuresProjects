# LargeScaleDataStructuresProjects
Genome Scaffold Analysis - This project analyzes genome scaffolds for length, GC content, and performance.  
Total Scaffolds: 607  
Largest: `568815346-9606` (147,687,514)  
Smallest: `568802230-9606` (340)  
Average Length: 5,036,551  
GC Content: 40.39%  
Time Complexity: O(N)  
Execution Time: 107.72s  
Run the script with:  
bash
sbatch job.sh
Genome Fragment Search - This project searches 32-character fragments of a subject dataset in a query dataset and measures performance.
Part A:
bash
./main "path_to_subject" "path_to_query" "A" 10000
Part B:
bash
./main "path_to_subject" "path_to_query" "B" 10000
Performance
Part A: 10K: 52 min, 1M: 66 hrs
Part B: 10K: 100 sec, 1M: 9,548 sec
Output
First 10 matches:
CTAACCCTAACCCTAACCCTAACCCTAACCCT, etc.
Hash Table and Genome Fragment Search - This project analyzes hash table performance and searches genome fragments using optimized algorithms. The impact of hash table sizes on collisions and search performance is assessed.
Problem A: Hash Table Performance  
bash
./main /common/contrib/classroom/inf503/genomes/human.txt \
/common/contrib/classroom/inf503/human_reads_2_trimmed.fa A <size>
Problem B: Search Fragments  
bash
./main /common/contrib/classroom/inf503/genomes/human.txt \
/common/contrib/classroom/inf503/human_reads_2_trimmed.fa B
Results
Problem A  
Collisions:  
1M: 27,512,408 | 10M: 25,866,925  
30M: 22,964,562 | 60M: 19,935,984  
Population Time: ~38 seconds (all sizes)  
Problem B  
Search Time: 4,892 seconds  
Fragments Found: 542,457,874  
First 15 Matches: `AAGACCACACTTCATT`, `ATTTATAAGCCACCCA`, ..., `NNNNNNNNNNNNNNNA`  
