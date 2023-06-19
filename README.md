# RNA Sequencing Pipeline: From FASTQ to DEA

Adv. Machine Learning Methods Final Project RNA Seq

Prompt: A topic of your own about visual, acoustic, language and other data modeling using modern deep learning techniques including convolutional neural networks, recurrent neural networks, auto-encoder etc. You can look for interesting topics on recent NeurIPS, CVPR, ICLR, ICCV, ACL, AAAI, etc.

Goals:
- Analyze raw reads from FASTQ Files
- Preprocessing with command line file to get counts matrix. (Packages used: fastp, hisat2, samtools, subread)
- Experimental data from lab, 18 paired reads.
- Gene ID's will be kept private, results will be published later as part of a larger study
- Create a template R file for analyzing counts matrix
- Differential expression, PCA, and GSEA heatmaps
- Apply auto-encoder for sample prediciton based on genetic expression profiles

Packages used for command line preprocessing:
- fastp
- hisat2
- samtools
- subread

Packages used for DEA:
- pyDESeq2
- matplotlib
- scanpy
- sklearn
- tensorflow, keras
