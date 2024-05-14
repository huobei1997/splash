For SPLASH, reads were first aligned to the reference using Bwa-Mem2.
Then reads were deduplicated using ‘sambamba’ (markdup). 
Afterwards, the custom script ‘find_chimeras.py’ was used to detect the split reads that were filtered using ‘filter_chimeras.py’. 
In contrast to the original paper, we also kept chimeric reads whose segments are 50 bases or less apart.
