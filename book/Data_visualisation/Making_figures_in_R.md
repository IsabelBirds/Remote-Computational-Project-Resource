
# Making figures in R

Here are some of the resources and tutorials I like to refer to when visualising my data using R.

## General resources

* [The R Graph Gallery](https://www.r-graph-gallery.com/)

    If you want to make a graph in R, The R Graph Gallery is the place to start.
It has lots of different ideas for plots, and simple to complex tutorials.

* [A ggplot2 tutorial for beautiful plotting in R](https://cedricscherer.netlify.app/2019/08/05/a-ggplot2-tutorial-for-beautiful-plotting-in-r/#toc)

    Lots of information and resources to help you make pretty plots.
    
* [Data Visualisation](https://datavizs21.classes.andrewheiss.com/)

    Content from PMAP 8921: Data Visualization (Summer 2021) by Dr Andrew Heiss

## Colour palettes

* [viridis](https://cran.r-project.org/web/packages/viridis/vignettes/intro-to-viridis.html)

    My favourite colour palette. Pretty and colour-blind friendly!

* [ggsci](https://cran.r-project.org/web/packages/ggsci/vignettes/ggsci.html)

    ggsci has some colour palettes based on various journals if you're feeling fancy, or some based on things like star trek if you're more like me...

## Graph types

* [Eulerr](https://github.com/jolars/eulerr)

    A personal pet hate is venn diagrams that aren't proportional.
    Euler fixes this by making area-proportional diagrams, or if that is impossible, a good approximation with included goodness-of-fit stats!
    (Euler diagrams are very similar to venn diagrams, they just don't require every set to interact.)

* [Heatmaps](http://www.opiniomics.org/you-probably-dont-understand-heatmaps/)

    A useful primer on what heatmaps actually tell us.

* [Upset plots](https://github.com/hms-dbmi/UpSetR)

    I'm a big fan of Upset plots.
    If you have lots of groups in your data, and venn diagrams turn into a massive confusing mess, that's the time to try an upset plot.
    They use a matrix to represent different intersections, and a bar plot to visualise the number of elements in each intersection.
    You can also get fancy and introduce queries or extra plots that describe different features of your data.

* [ggstatsplot](https://indrajeetpatil.github.io/ggstatsplot/)

    Another package I'm a fan of.
    This package runs statistical tests, and creates plots with them included.
    It also makes lovely violin/box plot combinations which are much more informative than a straightforward box plot.

* [ggbeeswarm](https://github.com/eclarke/ggbeeswarm)

    Are the points in your violin scatter plots overlapping so you can't see all the data?
    Ta-da, ggbeeswarm fixed it!

* [ggplot2 extensions](https://exts.ggplot2.tidyverse.org/gallery/)

    All the extensions I've mentioned above and more!

## Online Textbooks

* [ggplot2: elegant graphics for data analysis](https://ggplot2-book.org/) - A  guide to the Grammar of Graphics used by ggplot2 - for understanding theory.
* [R Graphics Cookbook](http://www.cookbook-r.com/Graphs/) - The whole book isn't available online, but some useful information is on the site about making data graphics in R.
* [Fundamentals of Data Visualisation](https://clauswilke.com/dataviz/) - A guide to effectively communicating your data using figures.

## Some other pointers

Some of these pointers may not make sense until you're trying to make a certain plot, but I've put them here in the hopes they are useful (also so I don't forget...).

* If you use xlim/ylim or scale_y_continous() to zoom in on a boxplot, ggplot recalculates the range etc based on that limit. If you want to include the outliers but just zoom in without recalculation, use coord_cartesian() to change the limits.
* In ggplot, discrete missing values are displayed. Adding `scale_color_discrete(na.translate = FALSE)` removes them. See [tweet source](https://twitter.com/MaiaPelletier/status/1357079168249458691/photo/1) for details.
