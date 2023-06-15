# RNA sequencing
Adv. Machine Learning Methods Final Project RNA Seq

Option (5): A topic of your own about visual, acoustic, language and other data modeling using modern deep learning techniques including convolutional neural networks, recurrent neural networks, auto-encoder etc. You can look for interesting topics on recent NeurIPS, CVPR, ICLR, ICCV, ACL, AAAI, etc.

Goals:
- Analyze raw reads from FASTQ Files
- Preprocessing with command line file to get counts matrix. (Packages used: fastp, hisat2, samtools, subread)
- Experimental data from lab, 18 paired reads.
- Gene ID's will be kept private, results will be published later as part of a larger study
- Create a template R file for analyzing counts matrix
- Differential expression, gene set enrichment, and PCA plots

Packages used for preprocessing fastq files to make count matricies

FASTQ file format input ex.)
- 1) Identifier ("@XXXX.....")
- 2) Sequence  ("ATGCGCGCATATATTTTGGCGCGTATGAGAC"
- 3) Place holder ('+')
- 4) Quality scores (ASCII encoded, phred qualities that represents confidence in correct base pair read)


featurecounts matrix outpur ex.)
- Index: 'Geneid'
- Column 1: Chromosome annotation
- Column 2: Start gene read position
- Column 3: End gene read position
- Column 4: Strand annotation
- Column 5: Gene length
- Column 6: sorted_read.bam file annotation
