# T-Cell Lymphoma drug combination synergism RNA-seq analysis

RNA-seq data analysis performed in R. RNA-seq data from T-Cell Lymphoma cells treated with DMSO, Drug A, Drug B or the combination to understand molecular mechanisms underlying drug synergism. Drug names are de-identified as results from this study are currently in submission.

A basic analysis can be found in DrugSynergy_RNAseq.Rmd and the associated .html file. This script will scale expression of every gene and export the results of DESEQ2 (https://bioconductor.org/packages/release/bioc/html/DESeq2.html) across every pairwise comparison to a .csv file for further analysis. In addition, I attempt to utilize Monte Carlo Reference-based Consensus Clustering (https://www.bioconductor.org/packages/release/bioc/html/M3C.html) to identify genes that are specifically dysregulated upon treatment with the combination of romidepsin and afatinib Dimaleate that are not observed during single agent treatment.

Under CompleteUpset_Figures/ scripts can be found to generate circos plots comparing the varying treatment conditions to understand differences and similarity. These circos plots are based off of differential expression analysis compared to DMSO (combination vs. DMSO, Drug A vs. DMSO, Drug B vs. DMSO).

To view the R Markdown notebook in html, please use the below link:

https://htmlpreview.github.io/?https://github.com/bobbyshih/drug-synergy-RNAseq-analysis/blob/main/DrugSynergy_RNAseq.html

To view the R Markdown notebook that generated the ComplexUpset circos and intersection plots, please use the below link:

https://htmlpreview.github.io/?https://github.com/bobbyshih/drug-synergy-RNAseq-analysis/blob/main/CompletUpset_Figures/DrugSynergy_RNAseq_FIGURES.html

This drug combination was identified using a high-throughput synergy screening strategy, summarized in the figure below (made using [BioRender](https://www.biorender.com/)):

![DrugSynergyHTS](https://github.com/bobbyshih/drug-synergy-RNAseq-analysis/assets/37740736/e53ace9f-b525-476f-8703-86bdc11d80c2)
