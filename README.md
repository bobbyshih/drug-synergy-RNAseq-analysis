# CTCL romidepsin + afatinib dimaleate combination synergism RNA-seq analysis
RNA-seq data analysis performed in R. RNA-seq data from MYLA cells treated with DMSO, romidepsin, afatinib dimaleate or the combination to understand molecular mechanisms underlying synergy between romidepsin and afatinib dimaleate.

A basic analysis can be found in MYLA_RomiAfaDimSyn_RNAseq.Rmd and the associated .html file. This script will scale expression of every gene and export the results of DESEQ2 (https://bioconductor.org/packages/release/bioc/html/DESeq2.html) across every pairwise comparison to a .csv file for further analysis. In addition, I attempt to utilize Monte Carlo Reference-based Consensus Clustering (https://www.bioconductor.org/packages/release/bioc/html/M3C.html) to identify genes that are specifically dysregulated upon treatment with the combination of romidepsin and afatinib Dimaleate that are not observed during single agent treatment.

Under CompleteUpset_Figures/ scripts can be found to generate circos plots comparing the varying treatment conditions to understand differences and similarity. These circos plots are based off of differential expression analysis compared to DMSO (combination vs. DMSO, romidepsin vs. DMSO, afatinib dimaleate vs. DMSO).

To view the R Markdown notebook in html, please use the below link:

https://htmlpreview.github.io/?https://github.com/bobbyshih/CTCL-drug-synergy-RNAseq-analysis/blob/main/MYLA_RomiAfaDimSyn_RNAseq.nb.html
