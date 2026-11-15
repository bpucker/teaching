# Applied Plant Transcriptomics

### WEEK 1 ###
# Introduction to VM & Ubuntu
- de.NBI cloud registration
- Connecting to de.NBI VM
- ls, cd, mkdir, top, htop
- file transfer via scp and rsync
- conda
- docker

#Introduction to Python
- Basic Python syntax
- Running a Python script
- virtualenv
- Install Python modules
- Using LLMs to generate code snipets for standard tasks
- Generate a Python script to conduct a statistical test

#Introduction to R
- Basic syntax
- Intall R packages
- Conduct statistical test on given dataset
- Generate figures to illustrate data distribution
- Export files and figures with R results

#Downloading from SRA
- SRA and RunSelector
- prefetch + fasterq-dump
- Download one RNA-seq dataset of Digitalis purpurea
- Document metadata
- Downloading RNA-seq data with XpBrew (all Digitalis data)

#RNA-seq quality control & de novo transcriptome assembly
- FastQC
- Trimmomatic
- Transcriptome assembly with Trinity


### WEEK 2 ###
# Assembly QC
- Calculate statistics
- Trimming assembly and header names
- BUSCO: assembly completeness

# RNA-seq read mapping
- STAR
- HISAT
- bowtie2
- converting, sorting, indexing with samtools
- coverage calulation
- DNA vs. RNA quantification

# Expression quantification
- read counting in mapping
- mapping-free quantification (kallisto)
- count table layout
- heatmap construction

# DEG identification
- DESeq2
- edgeR
- visualize DEG numbers


### WEEK 3 ###
# Functional annotation
- CDS identification
- Translation to PEP
- construct_anno.py
- KIPEs

# Pathway enrichment
- KEGG
- GO
- coexpression

# Phylotranscriptomics
- collect_best_BLAST_hits.py
- construction of alignment with MAFFT
- alignment trimming with algn_trim.py
- construct tree with IQ-TREE3
- visualization with iTOL

# Scientific publications
- scientific publishing seminar

# Long read transcriptomics (optional)
- de novo transcriptome assembly


### WEEL 4 ###
Individual projects & final presentation
