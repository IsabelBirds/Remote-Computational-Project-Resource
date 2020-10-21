# Online tutorials

## [Intro to survival analysis, originally from Memorial Sloan Kettering Cancer Centre](https://www.emilyzabor.com/tutorials/survival_analysis_in_r_tutorial.html#part_1:_introduction_to_survival_analysis)

* Detailed tutorial, will help with background knowledge – eg what is censoring?
* Improve understanding for when you need to justify decisions in your work.
* Data is from the survival package, so this tutorial doesn’t detail how to get from GEO.

Will need to install following packages in R:  
install.packages("survival")  
install.packages("survminer")  
install.packages("lubridate")  

## [Survival analysis with gene expression](https://www.biostars.org/p/344233/)

* Less detailed/not as beginner friendly.
* Loads some data from GEOquery – helpful for how to load, how to get gene ID from microarray IDs, basic High/mid/low plot.
* Lots of community queries and answers, may link to further resource.

Will need to install following packages in R:  
if (!requireNamespace("BiocManager", quietly = TRUE))  
install.packages("BiocManager")  
BiocManager::install("GEOquery")  
BiocManager::install("Biobase")  
install.packages("survival")  
BiocManager::install("RegParallel")  
