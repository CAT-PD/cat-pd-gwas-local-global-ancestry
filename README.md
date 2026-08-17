# Central Asian and Transcaucasian Parkinson's disease Genetics Study Consortium (CAT-PD Consortium)

## Quality Control and Imputation Pipeline

### Repository structure

```bash=
root/
├── LICENSE
├── README.md
├── 00_Quality_Control_GenoTools.ipynb
├── 01_Quality_Control_GWASQC.ipynb
└── 02_After_imputation.ipynb
```

### Details
|Notebook| Description|
|---|---|
|**00_Quality_Control_GenoTools.ipynb**| Notebook with [GenoTools](https://github.com/dvitale199/GenoTools) subsets by genetic ancestries and performs quality control in each subset separately. It uses default parameters. Underperforming SNPs were kindly provided by the GP2. |
|**01_Quality_Control_GWASQC.ipynb**| [GWASQC](https://github.com/MataLabCCF/GWASQC) pipeline includes both autosomal and chrX quality control, prepares data for imputation with fixref and submits with API. Underperforming SNPs and LARGE-PD exclusion SNPs were kindly provided by the GP2 and Dr. Thiago Peixoto Leal (Mata Lab, CCF). Relationship estimation was performed with [Natora](https://github.com/ldgh/NAToRA_Public).|
|**02_After_imputation.ipynb**| Extracts TYPED only variants for downstream analyses (e.g. SAIGE GWAS).  |

Software used:

|Item| Version|
|-----|-------|
|GenoTools | 1.3.6|
|Plink1.9 | 20250615|
|Plink2.0 |20250609|
|Eagle|2.4.1|
|tabix|0.2.6|
|bcftools|1.19|
