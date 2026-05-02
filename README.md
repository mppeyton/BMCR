# BMCR (Basically Making Charts Readable) Group Project
## Team Members: Riley Sheldon, Christopher Litwin, Brandon Le, & Mina Peyton  
<img width="494" height="517" alt="bmcR-hex-logo" src="https://github.com/user-attachments/assets/5377234b-29bd-4956-816b-541851c07338" />

# ✨ Multiomics Project  
## Integration of Single-Cell and Single-Nucleus RNA-seq in Aged Human Livers  

**Course Context:**  
Jackson Laboratory — *Methods for Multiomics Data Analysis*  
📅 April 26 – May 1, 2026  
🔗 https://www.jax.org/education-and-learning/education-calendar/2026/04-april/methods-for-multiomics-data-analysis-short-course  

## Project Summary

This project investigates age-associated changes in human liver biology through the integration of single-cell RNA sequencing (scRNA-seq) and single-nucleus RNA sequencing (snRNA-seq) datasets. Leveraging data from the **Cellular Senescence Network (SenNet)** program, we focus on hepatocyte zonation and its disruption with aging.


## Research Questions

1. **Does the single-cell transcriptional landscape of hepatocyte zonation change with age?**  
2. **Are these changes conserved across biological sex?**

---

## Hypothesis

Aging perturbs the spatial and transcriptional organization of hepatocyte zonation observed in young human livers.

---

## Objectives

- Integrate scRNA-seq and snRNA-seq datasets from young and aged human liver samples  
- Characterize zonation-specific transcriptional signatures  
- Assess sex-specific conservation of aging effects  
- Generate reproducible multi-omics analysis workflows  

---

## Data Sources

- **Primary Dataset:** Cellular Senescence Network (SenNet)  
  https://sennetconsortium.org/  

- **Data Types:**
  - Single-cell RNA-seq (scRNA-seq)  
  - Single-nucleus RNA-seq (snRNA-seq)  
  - (Optional extension) ATAC-seq for chromatin accessibility  

---

## Methods

### Data Acquisition
Datasets were obtained from the SenNet Data Portal.

### Experimental Platform
- **10x Genomics Chromium Next GEM Multiome**  
  - Gene Expression  
  - ATAC-seq (if applicable)

### Pre-processing & Integration

- Quality control, normalization, and feature selection  
- Integration using **Seurat Multimodal Reference Mapping**  
  🔗 https://satijalab.org/seurat/articles/multimodal_reference_mapping  

- Batch correction and cross-modality alignment  
- Cell-type annotation and zonation inference  

## Analytical Workflow

- Data preprocessing (QC, filtering, normalization)  
- Dimensionality reduction (UMAP)  
- Dataset integration (Seurat / multimodal mapping)  
- Differential expression analysis  
- Zonation trajectory inference  
- Sex-stratified comparative analysis  

---

## Expected Outputs

- Integrated liver cell atlas across age groups  
- Zonation-specific gene expression profiles  
- Differential aging signatures  
- Reproducible R-based analysis pipelines  

---

## References

- **Cellular Senescence Network (SenNet)**  
  https://sennetconsortium.org/  

- Karpova A, Li X, Peng C-W, et al.  
  *Cellular senescence in human liver under normal aging and cancer.*  
  Cell Genomics. 2026;6:101133.  
  🔗 https://www.sciencedirect.com/science/article/pii/S2666979X25003891  

---

## Tech Stack

- **R (>= 4.4)**  
- **Seurat (v5+)**  
- **Signac** (for ATAC, if used)  
- **tidyverse**  
- **Bioconductor ecosystem**  

---

## Reproducibility

- Version-controlled via GitHub  
- Scripted workflows (R / Quarto / RMarkdown)  
- Modular pipeline design  
- Seeded analyses where applicable  
