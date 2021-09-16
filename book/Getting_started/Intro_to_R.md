# Introduction to R

R is a free programming language and environment which is particularly popular for working with data in biology.
This means that there are lots of packages and tutorials out there for you to try.

R can often be more popular with women and other marginalised genders due to its strong, diverse community.
This includes [R-ladies](https://rladies.org/), a super friendly community for minority genders.
R-Ladies chapters around the world run events, help with troubleshooting codes, and share jobs, so it's worth taking a look at their site.

## Running R

Most programming languages have some sort of GUI - a graphical user interface. For R this is RStudio.
This means that instead of typing straight into the terminal like this:

```{figure} ../assets/images/Terminal_example.png
---
name: Terminal_example
alt: A screenshot of the terminal on a Mac computer, with R open.
width: 500px
---
```

You get a nice friendly set up like this:

```{figure} ../assets/images/RStudio_example.png
---
name: R_studio
alt: A screenshot of Rstudio, showing an example Rmarkdown document.
---
```

Using Rstudio means you can easily edit and run your code and see what files and packages you have loaded all at the same time.

A great trick you can use in Rstudio is rename in scope.
This changes all occurrences of a given variable name at once.
To access it, you highlight the variable name you want to change, and go to the Code menu, then rename in scope.
All occurrences of this variable will now be highlighted, and you can begin typing your new variable name!

```{figure} ../assets/images/rename_in_scope.gif
---
name: Rename_in_scope
alt:  A gif showing rename in scope used on some example code.
width: 400px
---
```

## Installing R and Rstudio

R and Rstudio have to be installed separately, and the exact process will depend on what operating system you use.

First you will need to download and install R from [CRAN](https://www.stats.bris.ac.uk/R/), The Comphrehensive R Archive Network.

Then download and install Rstudio Desktop from [Rstudio](https://www.rstudio.com/products/rstudio/download/).

## Installing Packages

There are lots of packages available for R, so they don't all come pre-installed - you will often need to install packages as you need them.

A lot of packages are easily accessible from CRAN, and can be installed using the ```install.packages()``` function.
You will then need to use the ```library()``` function to load the package into your R environment.

```r
#Install ggplot2 from CRAN
install.packages("ggplot2")

#Load ggplot
library(ggplot2)
```

To install packages that aren't on CRAN, you will need devtools.

```r
#Install devtools from CRAN
install.packages("devtools")

#Load devtools
library(devtools)

#Install and run praise
devtools::install_github("gaborcsardi/praise")
library(praise)
praise()

#> [1] "You are super-excellent!"
```

## Recording your work

You can record all of your work in R in [Rmarkdown](https://rmarkdown.rstudio.com/lesson-1.html) files - a lot like this file you're reading right now, which is created in markdown.
Rmarkdown files contain plain text and snippets of code. This makes it really easy to keep note of what your code does and why.

Writing this information properly is super important - think of your Rmarkdown documents as a computational lab book.
If you don't annotate your work well, it will almost certainly come back to bite you. Look at your work, and think - in 18 months, if I opened this document will I know what I did, why, and where I got the data from?
If not, fix it right away - I guarantee your future self is already thanking you.

As you get more confident with Rmarkdown files you will find more and more ways to use them - you can make reports, presentations, interactive dashboards, all sorts!

## Useful resources

* [Data Carpentry](https://datacarpentry.org/lessons/)

    Data Carpentry is fantastic project aimed at teaching researchers fundamental data skills, with lots of resources!
    The [Data Analysis and Visulation in R](https://datacarpentry.org/R-ecology-lesson/index.html) course would be a good place to start.
    They cover a lot of the information I've shared in a lot more detail, including how to get R and Rstudio set up, and lots more.

* [Introduction to R](https://bioinformatics-core-shared-training.github.io/r-intro/index.html)

    Introduction to R is an ongoing (as of 2020) work from home course run by the Bioinformatics Core at CRUK Cambridge Institute.
    Includes an introduction to R, RStudio, data manipulation and plots.
    You can’t access their video chat but all materials and solutions are available.

* [R, Open Research, and Reproducibility](https://r-openresearch-reproducibility.netlify.app/)

    Great resources from masters courses by Andrew stewart at the University of Manchester on R, Open Research, and Reproducibility.

* [R Cheatsheets](https://rstudio.com/resources/cheatsheets/)

    Not every R package has a cheatsheet, but key packages like dpylr and ggplot2 do, as well as some more niche packages.
    These are super useful - I have the dplyr cheat sheet printed out and refer to it all the time.

* [RStudio Projects and Working Directories: A Beginner's Guide](https://martinctc.github.io/blog/rstudio-projects-and-working-directories-a-beginner's-guide/)

    A guide to setting up and structuring RStudio projects.

* [r-statistics](http://r-statistics.co/R-Tutorial.html)

    A great site aimed at people working on machine learning and stats in R. Also has some great ggplot2 information.
    Includes a beginner friendly guide to starting out in R.

* [LURNblind](https://r-resources.massey.ac.nz/LURNblind/LURNBlindch2.html#x4-50002)

    An introduction to R aimed at blind users. Includes information about the BrailleR package.

* [What They Forgot to Teach You About R](https://rstats.wtf/index.html)
  
## Online Textbooks

* [Hands-On programming with R](https://rstudio-education.github.io/hopr/)
* [R for Data Science](https://r4ds.had.co.nz/)
* [Computational Genomics with R](https://compgenomr.github.io/book/)
* [R Markdown: The Definitive Guide](https://bookdown.org/yihui/rmarkdown/)
* [RMarkdown for Scientists](https://rmd4sci.njtierney.com/)
* [The Big Book of R](https://www.bigbookofr.com/index.html)

    An enormous collection of R-related programming books! 
    All the ones collected here and so many more.
