# Sources for biological data

## GEO (Gene Expression Omnibus)

* GEO lets you construct a very specific query for microarray data, with inclusion and exclusion criteria.
* [Link to a tutorial](https://www.ncbi.nlm.nih.gov/geo/info/qqtutorial.html).

## TCGA (The Cancer Genome Atlas)

* TCGA has lots of publicly available RNA-seq.
* Some of this requires [access](https://gdc.cancer.gov/access-data/obtaining-access-controlled-data), but most is publicly available.
* You can build a [query](https://docs.gdc.cancer.gov/Data_Portal/Users_Guide/Advanced_Search/) and specify open access only.
* Example query for open access, colon cancer RNA-seq data:

         files.access in ["open"] and files.cases.primary_site in ["colon"] and files.data_category in ["transcriptome profiling"] and files.data_type in ["Gene Expression Quantification"] and files.experimental_strategy in ["RNA-Seq"]
