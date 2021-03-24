# Analysis specific papers

Select papers with detailed methods/good figures which may help when planning pipelines.

## [INHBA is a prognostic predictor for patients with colon adenocarcinoma](https://bmccancer.biomedcentral.com/articles/10.1186/s12885-020-06743-2)

* Aimed to ID prognostic genes for COAD - detailed methods.
* Microarray data from GEO - multiple datasets, approx. 200 samples total.
* DEGs from GEO2R.
* GEO2R is an extension of GEO, compares two or more samples to ID DEGs (based on limma).
* Clinicopathological data from TGCA – 459 patients. Divided patients into high/low expression groups based on median RNA expression value.
* Microarray data choice – datasets that compared CRC tissue to normal. [Note – paper includes detail on platform used].
* Used a website (GEPIA) for Kaplan-Meier curves – of overall survival and disease frees survival based on gene expression – low/high gene TPM.
* [GEPIA](https://academic.oup.com/nar/article/45/W1/W98/3605636#90592750) is a web server for analyzing the RNA sequencing expression data of 9,736 tumors and 8,587 normal samples from the TCGA and the GTEx projects, using a standard processing pipeline.

## [Expression pattern of FGFR2, Grb2 and Plcγ1 acts as a novel prognostic marker of recurrence recurrence-free survival in lung adenocarcinoma](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4656736/)

* Looking at mRNA and protein levels of FGFR2, Grb2 and Plcγ1, testing correlation with clinical outcome.
* Combinational data on relative expression levels – eg high, high, low expression relatively = poor outcome.
* Patient characteristics and clinical outcomes summarised by mean and median for continuous variables, frequency (%) for categorical variables.  
* Included information on the entire chosen dataset in the supplementary as follows:
  * Table of patient characteristics – ages, tumour size, gender, etc, with Mean SD, Median (min,max).
  * K-M survival curves of OS and RDS for the whole cohort.
  * Good first steps for to get a feel for your chosen dataset. Would assume that these plots might already exist in the associated publication – good sense check.
