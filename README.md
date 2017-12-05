# final2017

#Welcome to the 2017 final page!

This "readme" is designed to explain the course of action I took to produce the two plots for my ChIP-seq data. 

I started with fastq files (unable to post here because of its size) and aligned it to the reference genome _hg19_ via bowtie. 

I then used macs 1.4 to call peaks for all the samples using the input DNA as control (as I had four replicates for both control,
I used samtools merge to merge all of them to one file) 

My ultimate goal was to produce plots showing how well the replicates were compared to eachother and then compared to the other condition.

To do this, I established the "peak" definition as having 50% reciprocal overlap with the other peaks. I then used jaccardi to produce a comparison of all replicates to eachother as well as other condition.

To view this graph simply download the Rmarkdowns of both indexheat.rmd and indexpca.rmd. 

__ENJOY__
