HASEM manuscript reproducibility archive — unsupervised component only

This archive corresponds to the accompanying Briefings in Bioinformatics manuscript on patient-aware, leakage-safe healthy-reference transcriptomic anomaly detection. It contains the unsupervised analysis notebook, saved preprocessing artefacts, split manifest, metadata, per-sample T²/Q scores, empirical-rule metrics, source-stratified false alarms and tissue-exclusion results.

The original full archive supplied by the authors is retained separately and contains exploratory supervised classification and gene-contribution analyses for the authors' future hybrid-model project. Those supervised analyses are not part of this manuscript and have been omitted from this manuscript-specific archive.

Data inputs: the notebook expects the UCSC Xena Toil expression and phenotype files named in the manuscript. The raw expression matrix is not included in this archive.

Batch correction: none was applied in the reported analysis. The notebook's healthy-source audit code has been corrected to group the separate metadata labels TCGA and TARGET together. The previous archived source-AUC outputs were invalid (NaN) and have been removed; the corrected audit cell has no saved output and must be rerun in the original data environment before any source-separability AUC is reported. The manuscript does not report such an AUC.

The archive does not contain a locked package environment. The notebook installs core dependencies but does not pin exact package versions.

The `gene_contributions_global.csv` file from the original archive was derived from a supervised random-forest model and is not an explanation of the unsupervised anomaly score; it is therefore not included here.
