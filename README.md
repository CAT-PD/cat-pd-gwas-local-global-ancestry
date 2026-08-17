# Central Asian and Transcaucasian Parkinson's disease Genetics Study Consortium (CAT-PD Consortium)

## CAT-PD GWAS with SAIGE, ATT and TRACTOR-MIX using local and global ancestry
Originally developed by LARGE-PD, Mata Lab, CCF, adapted for CAT-PD cohort: https://github.com/MataLabCCF/LARGE-PD_Phase2_Paper

### Repository structure

```bash=
root/
├── LICENSE
├── README.md
├── ./quality_control:
|   ├── 00_Quality_Control_GenoTools.ipynb
|   ├── 01_Quality_Control_GWASQC.ipynb
|   └── 02_After_imputation.ipynb
├── ./admixture_pca:
|   ├── 00_PCA.ipynb
|   ├── 01_Admixture.ipynb
|   └── 02_Plotting_with_xadmix.ipynb
├── ./calling:
|   ├── GenomeStudio_Caller.ipynb
|   └── NeuroBooster_IDAT_Calling.ipynb
├── ./gwas_local_global:
|   ├── 01_SAIGE_GWAS.ipynb
|   ├── 02_TractorMix_GWAS.ipynb
|   └── 03_ATT_GWAS.ipynb
├── ./gwas_stratified:
|   ├── GWAS_logistic_regression.ipynb
|   └── Meta_GWAMA_METAL_MRMEGA.ipynb
├── ./local_ancestry:
|   └── 01_Gnomix_Local_Ancestry_Inference.ipynb
└── ./prs:
    └── PRS.ipynb
```

### Details
|Notebook| Description|
|---|---|
|**00_SAIGE_GWAS.ipynb**| GWAS in Related individuals with Genetic Relationship Matrix (GRM) using [SAIGE](https://saigegit.github.io/SAIGE-doc/) (pixi). |
|**01_Gnomix_Local_Ancestry_Inference.ipynb**| Perform Local ancestry inference with G-nomix and using the standardized pipeline by Mata lab, CCF [LARGE-PD Pipeline](https://github.com/MataLabCCF/LARGE-PD_Phase2_Paper).|
|**02_TractorMix_GWAS.ipynb**|  [TRACTOR-MIX](https://github.com/Atkinson-Lab/Tractor-Mix) implementation and GWAS for 6-way ancestry inference. Uses related individuals with GRM.  |
|**03_ATT_GWAS.ipynb**| GWAS using Cochran-Armitage Trend Test via [admix kit](https://github.com/KangchengHou/admix-kit) tool. Unrelated individuals only.  |

Software used:

|Item| Version|
|-----|-------|
|Plink1.9 | 20250615|
|Plink2.0 |20250609|
|G-nomix| 0.0.7|
|GCTA| 1.93.1|
|Admix-kit| 0.1.1|
