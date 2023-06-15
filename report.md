### RNA Sequencing (Adv. Machine Learning Methods Final Project) Report

#### Abstract:

- Highlight the interesting aspects of your problem and its potential impact (Question 1).

The main objective of this project is to develop a user-friendly pipeline that can be easily utilized by researchers in our laboratory, 
even those with limited to no experience at all. By providing a general framework and clear guidelines, we aim to empower researchers to 
conduct RNA-seq analysis on their own, enabling them to explore the rich insights hidden in gene expression data. In the following sections, 
we provide a comprehensive introduction to RNA sequencing, its underlying principles, and its wide-ranging applications in various fields. 
We emphasize the uniqueness of our dataset and size (~50 gb of raw reads in fastq.gz files) and its relevance to our research goals, highlighting
the experimental nature of the data and its potential to unveil novel findings. Overall, this project not only contributes to the advancement of 
RNA-seq analysis but also has the potential to make a significant impact by providing a valuable tool for researchers in our laboratory and beyond. 
By simplifying the analysis process and enabling researchers to uncover valuable insights from their gene expression data, we strive to facilitate 
further discoveries and advancements in our research domain.


#### Introduction:

- Provide background information on RNA sequencing and its applications (Question 3).
- Describe the uniqueness of your dataset and its relevance to your research (Question 3).
- Discuss the challenges and opportunities associated with analyzing large RNA-seq datasets.


#### Methods:

- Explain the experimental design and data collection process, highlighting the challenges of working with a large dataset (Question 2).
- Describe the preprocessing steps and the specific tools used, emphasizing their relevance and ease of use for beginners (Question 6).

#### Experiments:

- Discuss the comprehensiveness of your experimental design, including the tuning of hyperparameters (Question 4).
- Present the results of differential expression analysis, highlighting any novel findings (Question 3).
- Showcase visualizations, such as PCA plots, to demonstrate the quality and validity of your analysis (Question 5).

#### Conclusion:

- Summarize the key findings and their relevance to the problem studied (Question 1).
- Reflect on the strengths and limitations of your analysis (Question 4).
- Discuss future directions and potential applications of your work (Question 6).

#### References:

- Include a comprehensive list of references used in your report.
- TPM calc: https://github.com/lucynwosu/TPM-Transcripts-Per-Million-Normalization-Python/blob/main/TPM-Transcripts-Per-Million-Normalization.ipynb
- pydeseq2 syntax help: https://github.com/mousepixels/sanbomics_scripts/blob/main/PyDeseq2_DE_tutorial.ipynb
- fastp: 1) Shifu Chen. 2023. Ultrafast one-pass FASTQ data preprocessing, quality control, and deduplication using fastp. iMeta 2: e107. https://doi.org/10.1002/imt2.107; 2) Shifu Chen, Yanqing Zhou, Yaru Chen, Jia Gu; fastp: an ultra-fast all-in-one FASTQ preprocessor, Bioinformatics, Volume 34, Issue 17, 1 September 2018, Pages i884–i890, https://doi.org/10.1093/bioinformatics/bty560
- samtools: Twelve years of SAMtools and BCFtools, Petr Danecek, James K Bonfield, Jennifer Liddle, John Marshall, Valeriu Ohan, Martin O Pollard, Andrew Whitwham, Thomas Keane, Shane A McCarthy, Robert M Davies, Heng Li (GigaScience, Volume 10, Issue 2, February 2021, giab008)  https://doi.org/10.1093/gigascience/giab008
- hisat2: https://daehwankimlab.github.io/hisat2/
- subread: Liao, Y., Smyth, G. K., & Shi, W. (2013). The Subread aligner: fast, accurate and scalable read mapping by seed-and-vote. Nucleic acids research, 41(10), e108. https://doi.org/10.1093/nar/gkt214
