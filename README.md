# Multiple Sclerosis Cell Type Annotation with scGPT

This repository provides code and documentation for fine-tuning the [scGPT](https://github.com/bowang-lab/scGPT) transformer-based foundation model on single-cell and single-nucleus RNA sequencing (sc/snRNA-seq) datasets related to **Multiple Sclerosis (MS)**. The goal is to improve cell type annotation performance to support more precise drug testing and target discovery in MS research.

---

## Datasets Used

The following datasets were used for fine-tuning and evaluating scGPT. Each dataset includes a short description and a direct download link. The exact folder that was used to train the model can be found here: [Google Drive Folder](https://drive.google.com/drive/folders/1ZxHeCjuoq77Tykups8tm0Lx2PSm_Lq7I?usp=drive_link)  

| Dataset | Usage Description | Download |
|--------|-------------------|----------|
| **Schirmer et al. (2019)**<br>_“Neuronal Vulnerability and Multilineage Diversity in Multiple Sclerosis”_ | Testing dataset — 77,891 cells from MS lesions (E-HCAD-35) | [Download](https://www.ebi.ac.uk/biostudies/arrayexpress/studies/E-HCAD-35) |
| **Rasmussen et al. (2020)**<br>_“Single-Cell RNA-Sequencing of CSF and Blood Leukocytes in MS”_ | Fine-tuning dataset — CSF & blood leukocytes (GSE138266) | [Download](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE138266) |
| **Jakel et al. (2019)**<br>_“Altered Human Oligodendrocyte Heterogeneity in MS”_ | Oligodendrocyte-specific fine-tuning (GSE118257) | [Download](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE118257) |
| **Schirmer et al. (2023)**<br>_“Single-Nucleus RNA-Seq of MS Lesions and NAWM”_ | Alternate testing dataset — MS lesions and NAWM | [Download](https://doi.org/10.5281/zenodo.8342315) |

---

## Results Summary

| Metric | Baseline scGPT | Fine-tuned Model |
|--------|----------------|------------------|
| Accuracy | 0.856 | 0.940 |
| Precision | 0.729 | 0.936 |
| Recall | 0.720 | 0.945 |
| Macro F1 | 0.703 | 0.926 |
