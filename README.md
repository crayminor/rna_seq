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
- 1) Identifier ("@XXXX....."
- 2) Sequence  ("ATGCGCGCATATATTTTGGCGCGTATGAGAC"
- 3) '+'
- 4) Quality scores (phred encoded, represents confidence in correct base pair read)


featurecounts matrix outpur ex.)
- Index: 'Geneid'
- Column 1: Chromosome annotation
- Column 2: Start gene read position
- Column 3: End gene read position
- Column 4: Strand annotation
- Column 5: Gene length
- Column 6: sorted_read.bam file annotation


Abstract:
- Highlight the interesting aspects of your problem and its potential impact (Question 1).
Introduction:
- Provide background information on RNA sequencing and its applications (Question 3).
Describe the uniqueness of your dataset and its relevance to your research (Question 3).

Methods:
- Explain the experimental design and data collection process, highlighting the challenges of working with a large dataset (Question 2).
- Describe the preprocessing steps and the specific tools used, emphasizing their relevance and ease of use for beginners (Question 6).

Experiments:
- Discuss the comprehensiveness of your experimental design, including the tuning of hyperparameters (Question 4).
- Present the results of differential expression analysis, highlighting any novel findings (Question 3).
- Showcase visualizations, such as PCA plots, to demonstrate the quality and validity of your analysis (Question 5).

Conclusion:
- Summarize the key findings and their relevance to the problem studied (Question 1).
- Reflect on the strengths and limitations of your analysis (Question 4).
Discuss future directions and potential applications of your work (Question 6).
References:

Include a comprehensive list of references used in your report.

### Explanation of packages used
fastp: Fastp is a tool for comprehensive quality control and preprocessing of fastq files. It performs tasks such as adapter trimming, quality filtering, read
trimming, and read length filtering. Fastp helps to ensure that the input fastq files are of high quality and suitable for downstream analysis.

hisat2: Hisat2 is an accurate alignment tool for mapping RNA-seq reads to a reference genome. In this specific case we are using the Mus musculus dataset as a reference
useing a two-step process to align the reads. First, it builds an index of the reference genome using the hisat2-build command. Then, it aligns the reads to the indexed
genome using the hisat2 command. Hisat2 produces a SAM/BAM file containing the aligned reads, which can be further processed and analyzed.

samtools: Samtools is a suite of tools for manipulating and working with SAM/BAM files, which are commonly used for storing aligned sequencing reads. Samtools provides
various functionalities, including sorting, indexing, filtering, merging, and converting SAM/BAM files. It is widely used in bioinformatics pipelines to perform tasks
such as read alignment post-processing and downstream analysis.

subread (featureCounts): Subread is a software package that includes featureCounts, a tool used for read counting and summarizing aligned reads to genomic features, such
as genes or exons. FeatureCounts takes aligned reads (in BAM format) and an annotation file (in GTF/GFF format) as input. It assigns each read to the corresponding
genomic feature and counts the number of reads per feature. The output is a counts matrix, where each row represents a genomic feature and each column represents a
sample.
