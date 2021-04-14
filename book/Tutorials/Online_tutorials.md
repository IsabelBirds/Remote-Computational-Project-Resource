# Online tutorials

To Do
## [Introduction to survival analysis](https://www.emilyzabor.com/tutorials/survival_analysis_in_r_tutorial.html#part_1:_introduction_to_survival_analysis)

* Originally from Sloan Kettering Cancer Centre.
* Detailed tutorial, use to develop background knowledge on cancer data – eg what is censoring?
* Improve understanding for when you need to justify decisions in your work.
* Data is from the survival package.

Will need to install following packages in R:  
install.packages("survival")  
install.packages("survminer")  
install.packages("lubridate")  

## [Survival analysis with gene expression](https://www.biostars.org/p/344233/)

* Less detailed/not as beginner friendly.
* Loads some data from GEOquery – helpful for how to load, how to get gene ID from microarray IDs, how to plot basic high/mid/low plots.
* Lots of community queries and answers, may link to further resource.

Will need to install following packages in R:  
if (!requireNamespace("BiocManager", quietly = TRUE))  
install.packages("BiocManager")  
BiocManager::install("GEOquery")  
BiocManager::install("Biobase")  
install.packages("survival")  
BiocManager::install("RegParallel")  

## [Differential Expression Analysis using edgeR](https://bioinformatics-core-shared-training.github.io/cruk-bioinf-sschool/Day3/rnaSeq_DE.pdf)

* General tutorial for differential expression analysis of GEO data using edgeR.

## [Practical statistical analysis of RNA-Seq data](http://www.nathalievialaneix.eu/doc/html/solution_edgeR-tomato-withcode.html)

* More detailed tutorial of using edgeR, includes plots.
* Doesn't show how to get data.

## [Tutorials for the WGCNA package](https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/Tutorials/)

* WGCNA – weighted correlation network analysis of microarray data.

## [Differential Expression with Limma-Voom](https://ucdavis-bioinformatics-training.github.io/2018-June-RNA-Seq-Workshop/thursday/DE.html)

* Tutorial for using limma-voom with RNA-seq data.
* Doesn't show how to get data.

To do:
* https://aosmith.rbind.io/ , https://aosmith.rbind.io/2018/01/09/simulate-simulate-part1/
*  http://www.page-gould.com/simulation/Guide-to-Simulation-for-R.html
* https://sbresnahan.github.io/RNAseq-to-DEGs/
* https://rstudio-pubs-static.s3.amazonaws.com/329027_593046fb6d7a427da6b2c538caf601e1.html 
* http://mfviz.com/hierarchical-models/
* https://guides.library.upenn.edu/c.php?g=1117669&p=8150225 
* https://github.com/resulumit/rmd_workshop 
* https://www.kaylea.co.uk/talk/funwithfunctions/ 
* https://stats.idre.ucla.edu/other/mult-pkg/whatstat/ 
* https://www.molecularecologist.com/2019/01/03/simple-gantt-charts-in-r-with-ggplot2-and-the-tidyverse/
* https://www.natedayta.com/2019/12/25/owning-outlines-in-rstudio/
* https://blog.codinghorror.com/a-visual-explanation-of-sql-joins/ 
* https://www.pythonforthelab.com/blog/introduction-to-storing-data-in-files/
* http://www.rebeccabarter.com/blog/2019-08-05_base_r_to_tidyverse/ 
* 