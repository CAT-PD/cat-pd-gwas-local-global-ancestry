# Central Asian and Transcaucasian Parkinson's disease Genetics Study Consortium (CAT-PD Consortium)

## PCA and Admixture

### Repository structure

```bash=
root/
├── LICENSE
├── README.md
├── 00_PCA.ipynb
├── 01_Admixture.ipynb
└── 02_Plotting_with_xadmix.ipynb
```

### Details
|Notebook| Description|
|---|---|
|**00_PCA.ipynb**| Perform PCA and plot by country. |
|**01_Admixture.ipynb**| Run supervised admixture using [AdmixtureWithReference](https://github.com/MataLabCCF/AdmixtureWithReference) Pipeline.|
|**02_Plotting_with_xadmix.ipynb**| Alternative plotting method with R package `xadmix`.  |



Software used:

|Item| Version|
|-----|-------|
|Plink1.9 | 20250615|
|Plink2.0 |20250609|
|Admixture |1.3.0|
|GCTA| 1.93.1|