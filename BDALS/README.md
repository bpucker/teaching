# Summer School 'Big Data Analytics in Life Sciences'

This Summer School is organized by the Plant Biotechnology and Bioinformatics group at TU Braunschweig. Please visit the [BDALS website](https://www.tu-braunschweig.de/en/ifp/pbb/teaching/bdals) for additional details. This repository provides links to various resources required for the exercises of the summer school and harbors the slides of background presentations.

## Overview
- Day1: Introduction
- Day2: Genomics #1
- Day3: Genomics #2 and Phylogenetics
- Day4: Transcriptomics
- Day5: Summarizing, visualizing, publishing


## Day1: Introduction
- [Jupyter Notebook](https://jupyter.org/) is an excellent way to document
- [de.NBI cloud](https://www.denbi.de/cloud)
- [ssh](https://en.wikipedia.org/wiki/Secure_Shell)
- [Filezilla](https://filezilla-project.org/)
- [scp](https://www.freecodecamp.org/news/scp-linux-command-example-how-to-ssh-file-transfer-from-remote-to-local/)
- [Linux basics](https://ubuntu.com/tutorials/command-line-for-beginners)
- [Mounting disk](https://superuser.com/questions/134734/how-to-mount-a-drive-from-terminal-in-ubuntu)
- [conda](https://conda.io/projects/conda/en/latest/user-guide/getting-started.html)
- [cloning from GitHub](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)
- [virtual environments](https://docs.python.org/3/library/venv.html)
- Install tools:
    - [Shasta](https://github.com/paoloshasta/shasta)
    - [BRAKER3](https://github.com/Gaius-Augustus/BRAKER)
    - [minimap2](https://github.com/lh3/minimap2)
    - [SVIM2](https://github.com/eldariont/svim)
    - [BUSCO5](https://busco.ezlab.org/busco_userguide.html)
    - [KIPEs3](https://github.com/bpucker/KIPEs)


## Day2: Genomics #1
- QC & trimming/filtering of ONT long reads: [nanostat](https://github.com/wdecoster/nanostat)
- Assembly: [Shasta](https://github.com/paoloshasta/shasta)
- Gene prediction: [BRAKER3](https://github.com/Gaius-Augustus/BRAKER)
- Assess data set completeness: [BUSCO5](https://busco.ezlab.org/busco_userguide.html)
- Functional annotation:
    - [Mercator](https://www.plabipd.de/mercator_main.html)
    - [KIPEs3](https://github.com/bpucker/KIPEs)
- Find and install a tool to check read quality and perform trimming if necessary
- Running an assembly of digi1 and digi4 with Shasta requires conversion of FASTQ to FASTA: [fastq2fasta.py](https://github.com/bpucker/PBBtools/blob/main/collection/fastq2fasta.py)
- Calculate assembly statistics: [contig_stats3.py](https://github.com/bpucker/GenomeAssembly/blob/main/contig_stats3.py)
- Run [BUSCO5](https://busco.ezlab.org/busco_userguide.html) on assembly
- Install [HISAT2](http://daehwankimlab.github.io/hisat2/) and map some RNA-seq reads to the assembly
- Run gene prediction with [BRAKER3](https://github.com/Gaius-Augustus/BRAKER)
- Run [BUSCO5](https://busco.ezlab.org/busco_userguide.html) on structural annotation
- Perform a functional annotation with Mercator and [KIPEs3](https://github.com/bpucker/KIPEs)
- Map digi1 and digi4 reads with [minimap2](https://github.com/lh3/minimap2) to assembly
- Identify sequence variants with [SVIM2](https://github.com/eldariont/svim) based on the mapping
- Predict variant effects with [SnpEff](https://pcingola.github.io/SnpEff/) and [NAVIP](https://github.com/bpucker/NAVIP)
- Perform a synteny analysis with between a digi1 and digi4 assembly with [MCscan/JCVI](https://github.com/tanghaibao/jcvi/wiki/MCscan-(Python-version))


## Day3: Genomics #2 & Phylogenetics
- Generate [circos](https://circos.ca/) plots
- Collect sequences: [NCBI](https://www.ncbi.nlm.nih.gov/)
- Construct a multiple sequence alignment: [MAFFT](https://mafft.cbrc.jp/alignment/server/index.html)
- Phylogenetic tree construction: [FastTree2](http://www.microbesonline.org/fasttree/), [IQ-TREE2](http://www.iqtree.org/)
- Visualization of a phylogenetic tree: [iTOL](https://itol.embl.de/)


## Day4: Transcriptomics
- Retrieve RNA-seq data sets from SRA/PUB: [sra-toolkit](https://github.com/ncbi/sra-tools)
- Quality control: [fastQC](https://github.com/s-andrews/FastQC)
- Trimming of reads: [Trimmomatic](http://www.usadellab.org/cms/?page=trimmomatic)
    - Requires renmaing reads in FASTQ file: [https://github.com/bpucker/codi/blob/main/rename_reads_for_trinity.py]
- De novo transcriptome assembly: [Trinity](https://github.com/trinityrnaseq/trinityrnaseq/wiki)
- Split read mapping: [STAR](https://physiology.med.cornell.edu/faculty/skrabanek/lab/angsd/lecture_notes/STARmanual.pdf), [HISAT2](http://daehwankimlab.github.io/hisat2/)
- Quantification of gene expression: [kallisto](https://github.com/pachterlab/kallisto)
- Identification of DEGs: [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html)
- Co-expression analysis: [pbb-tools.de](https://pbb-tools.de/)


## Day5: Summarizing, visualizing, publishing
- Analyze expression data with a PCA to see similarity of replicates: [PCA instructions](https://bioconductor.org/packages/release/bioc/html/pcaExplorer.html)
- Generate a heatmap of some anthocyanin biosynthesis genes: [Python heatmap constrution](https://seaborn.pydata.org/generated/seaborn.heatmap.html)
- Prepare your sequencing data for submission to [ENA](https://ena-docs.readthedocs.io/en/latest/)
- Prepare a documentation describing your genome sequence and annotation for publication through [LeoPARD](https://leopard.tu-braunschweig.de/content/index.xml)
- Generate a [GitHub](https://github.com/) or [codeberg](https://codeberg.org/) repository and document your workflow of the week


## References
Nowak M. S., Harder B., Meckoni S. N., Friedhoff R., Wolff K., Pucker B. (2024). Genome sequence and RNA-seq analysis reveal genetic basis of flower coloration in the giant water lily Victoria cruziana. bioRxiv 2024.06.15.599162; doi: [10.1101/2024.06.15.599162](https://doi.org/10.1101/2024.06.15.599162).

Wolff K., Friedhoff R., Horz J. M., Pucker B. (2024). Genome sequence of the medicinal and ornamental plant Digitalis purpurea reveals the molecular basis of flower color variation. bioRxiv 2024.02.14.580303; doi: [10.1101/2024.02.14.580303](https://doi.org/10.1101/2024.02.14.580303).

Pucker, B. (2024). Functional Annotation – How to Tackle the Bottleneck in Plant Genomics. Preprints. doi: [10.20944/preprints202402.0645.v1](https://doi.org/10.20944/preprints202402.0645.v1).

Baasner J.-S., Rempel A. Howard D., Pucker B. (2024). NAVIP: Unraveling the Influence of Neighboring Small Sequence Variants on Functional Impact Prediction. bioRxiv 596718; doi: [10.1101/596718](https://doi.org/10.1101/596718).

Pucker, B.*, Walker-Hale, N.*, Dzurlic, J., Yim, W.C., Cushman, J.C., Crum, A., Yang, Y. and Brockington, S.F. (2024), Multiple mechanisms explain loss of anthocyanins from betalain-pigmented Caryophyllales, including repeated wholesale loss of a key anthocyanidin synthesis enzyme. New Phytol., 241: 471-489. doi: [10.1111/nph.19341](https://doi.org/10.1111/nph.19341).

Wolff, K.; Friedhoff, R.; Schwarzer, F.; Pucker, B. (2023). Data Literacy in Genome Research. Journal of Integrative Bioinformatics, 2023, pp. 20230033. doi: [10.1515/jib-2023-0033](https://doi.org/10.1515/jib-2023-0033).

Rempel A., Choudhary N. and Pucker B. (2023). KIPEs3: Automatic annotation of biosynthesis pathways. PLOS ONE 18(11): e0294342. doi: [10.1371/journal.pone.0294342](https://doi.org/10.1371/journal.pone.0294342).

Pucker B & Iorizzo M (2023). Apiaceae FNS I originated from F3H through tandem gene duplication. PLOS ONE 18(1): e0280155. doi: [10.1371/journal.pone.0280155](https://doi.org/10.1371/journal.pone.0280155).

Pucker B, Irisarri I, de Vries J and Xu B (2022). Plant genome sequence assembly in the era of long reads: Progress, challenges and future directions. Quantitative Plant Biology, 3, E5. doi: [10.1017/qpb.2021.18](https://doi.org/10.1017/qpb.2021.18).

