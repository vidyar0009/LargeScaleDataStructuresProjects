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
