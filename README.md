# Central Asian and Transcaucasian Parkinson's disease Genetics Study Consortium (CAT-PD Consortium)

## GWAS Logistic Regression with Plink (GLM)

### Repository structure

```bash=
root/
├── LICENSE
├── README.md
└── GWAS_logistic_regression.ipynb
```

### Details
Code in this repository is built to perform logistic regression with `Plink2.0` adjusted for sex, age and PC1-5 on unrelated individuals. It uses data that underwent quality control and was subset by GenoTools, then imputed on TOPMed Imputation Server. The intention is to run in parallel regressions for all ancestries and chromosomes.
After regression, the script uses `pandas` to concatenate outputs per chromosome and plot Manhattan and QQ plots per ancestry using `GWASLab 4.1.2`.

Software used:

|Item| Version|
|-----|-------|
|Plink1.9 | 20250615|
|Plink2.0 |20250609|
|GWASLab  | 4.1.2|
