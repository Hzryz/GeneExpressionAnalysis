# Investigation of The Role of SAA2 in Pulmonary Pre-Malignant Lesions: a Bioinformatics Approach for Biomarker Discovery and Prognostic Assessment.

## Project Overview

This project investigates the role of the Serum Amyloid A2 (SAA2) gene in the progression of pulmonary pre-malignant lesions using bioinformatics approaches. The primary goal is to establish SAA2 as a potential biomarker for early detection and prognostic assessment of lung cancer by analyzing gene expression profiles across normal, pre-malignant, and malignant lung tissues.

By integrating multiple public microarray datasets from the NCBI GEO repository and applying differential gene expression, protein-protein interaction network analysis, pathway enrichment, and survival analysis, this project provides important insights into the molecular mechanisms involving SAA2. The results support the potential of SAA2 as a non-invasive biomarker and therapeutic target to prevent progression to invasive lung cancer.

## Data and Tools Used

| Category               | Name                     | Usage Description                                                   | Reference                   |
|------------------------|--------------------------|---------------------------------------------------------------------|-----------------------------|
| Data repository        | NCBI GEO                 | Source of gene expression microarray data                           | (Barrett et al., 2013)      |
| Protein interaction    | STRING Database          | Protein-protein interaction networks                                | (Szklarczyk et al., 2019)  |
| Functional annotation  | DAVID                    | Gene ontology and pathway enrichment analysis                       | (Huang et al., 2009)        |
| Programming IDE        | RStudio                  | Statistical computing and graphics environment                      | (RStudio Team, 2022)        |
| Gene set enrichment    | GSEA / ssGSEA            | Analysis of gene sets for pathway-level activity                    | (Subramanian et al., 2005)  |
| Survival analysis      | Kaplan-Meier Plotter     | Correlation of gene expression with patient survival                | (Győrffy et al., 2013)      |

## Dataset Information

Five microarray datasets were sourced from NCBI GEO to cover lung tissues in various states:

| Dataset  | Sample Size (Normal / Tumor) | Lesion Type     | Reference                    |
|----------|------------------------------|-----------------|------------------------------|
| GSE79209 | 25 / 57                      | Pre-malignant   | Beane et al., 2017           |
| GSE79210 | 5 / 47                       | Pre-malignant   | Beane et al., 2017           |
| GSE18842 | 44 / 47                      | Malignant       | Sanchez-Palencia et al., 2011|
| GSE19188 | 65 / 91                      | Malignant       | Hou et al., 2010             |
| GSE33532 | 20 / 80                      | Malignant       | Meister et al., 2014         |

## Methodology

1. **Data Acquisition**: Raw datasets downloaded from NCBI GEO.
2. **Data Preprocessing**: Normalization and annotation of gene probes with R and Bioconductor packages.
3. **Differential Expression Analysis**: Using DESeq2 to identify genes differentially expressed between normal, pre-malignant, and malignant tissues.
4. **Protein-Protein Interaction Network**: Constructed with STRING and visualized with Cytoscape to identify key interacting proteins.
5. **Functional Enrichment Analysis**: Gene Ontology (GO) and KEGG pathway analyses performed to identify biological processes and pathways involving SAA2.
6. **Gene Set Enrichment Analysis**: ssGSEA to evaluate pathway activation in individual samples.
7. **Survival Analysis**: Kaplan-Meier analysis correlating SAA2 expression with overall survival.

## Key Findings

- SAA2 expression progressively increases from normal lung tissue to severe dysplasia and is highest in malignant lung tissues.
- Protein networks highlight interactions of SAA2 with proteins involved in inflammation and lipid metabolism, notably apolipoproteins.
- Pathway enrichment points to involvement of PPAR signaling and cholesterol metabolism in SAA2-associated pathways.
- High SAA2 expression correlates with poorer patient survival outcomes, supporting its prognostic value.

## Recommendations

- Further experimental validation of SAA2 as a non-invasive biomarker in clinical samples.
- Exploration of therapeutic strategies targeting SAA2 or its regulatory pathways, especially PPAR signaling, to prevent malignancy progression.
- Development of screening protocols incorporating SAA2 for early-stage lung disease detection.

## How to Run Analysis

- All analysis performed in RStudio using R and Bioconductor packages.
- Scripts for data processing, normalization, DEG identification, PPI network, enrichment, ssGSEA, and survival analysis are included in the repository.
- Users should download microarray datasets from NCBI GEO, place them in the data folder, and follow the instructions in `analysis_script.R` to reproduce findings.

## Citation / Rujukan

If you use this project in your research, please cite:

Muhammad Zam Hazri Bin Zamri (2025). *Investigation of the Role of SAA2 in Pulmonary Pre-Malignant Lesions: A Bioinformatics Approach for Biomarker Discovery and Prognostic Assessment.* Universiti Kebangsaan Malaysia.

## Contact

For any inquiries or collaboration, please contact:  
Muhammad Zam Hazri Bin Zamri  
Email: zamhazri@gmail.com 
Faculty of Science and Technology,  
Universiti Kebangsaan Malaysia
