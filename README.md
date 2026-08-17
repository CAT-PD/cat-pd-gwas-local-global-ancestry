# Central Asian and Transcaucasian Parkinson's disease Genetics Study Consortium (CAT-PD Consortium)

## PCA and Admixture

### Repository structure

```bash=
root/
├── LICENSE
├── README.md
├── 00_SAIGE_GWAS.ipynb
├── 01_Gnomix_Local_Ancestry_Inference.ipynb
├── 02_TractorMix_GWAS.ipynb
└── 03_ATT_GWAS.ipynb
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