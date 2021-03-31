# Visualising your data

At any point in your analysis, visualising your data is massively important! 

At the start, it can help you understand your data, see trends and spot outliers. Throughout your project you will have to discuss your resarch with supervisors and peers - diagrams make this so much easier. And when it comes to writing up/presenting your work, hopefully you will already have lots of diagrams ready to go.

When working computationally, you also may go many days without feeling like you've made tangible progress like you would in wet lab. Making a diagram to describe an aspect of your work can help with this feeling, and help you prove to yourself that you have made progress! This doesn't have to be complicated - for example you could just make a flowchart to describe the pipeline you've spent days reading up on, planning and installing.

## Accessibilty

A really key part of making figures is their accessibility. It's all well and good making a beautiful figure, but if some of your audience can't understand it then you're both missing out!

* Colour choice - you can use a site like [accessible colours](https://accessible-colors.com/) or [colour contrast checker](https://colourcontrast.cc/) to make sure everyone can access your work. 
* Font size - make sure all text is large enough to be clear (even from a distance if you're presenting a poster).
* Language - If you're presenting a poster to a mixed audience, they may not all understand the jargon you use everyday.
* Microphones - slightly off the topic of data vis, but if you're presenting at a conference, never say no to the microphone. Even if you think your voice is loud enough to be heard throughout the room, there may be people present who need the microphone to be used to be able to hear you.

## [viridis](https://cran.r-project.org/web/packages/viridis/vignettes/intro-to-viridis.html)

My favourite colour palette. Pretty and colour-blind friendly!

## [ggsci](https://cran.r-project.org/web/packages/ggsci/vignettes/ggsci.html)

ggsci has some colour palettes based on various journals if you're feeling fancy, or some based on things like star trek if you're more like me...

## [The R Graph Gallery](https://www.r-graph-gallery.com/)

If you want to make a graph in R, The R Graph Gallery is the place to start. It has lots of different ideas for plots, and simple to complex tutorials.

## [A ggplot2 tutorial for beautiful plotting in R](https://cedricscherer.netlify.app/2019/08/05/a-ggplot2-tutorial-for-beautiful-plotting-in-r/#toc)

Lots of information and resources to help you make pretty plots.

## [Eulerr](https://github.com/jolars/eulerr)

A personal pet hate - venn diagrams that aren't proportional! Euler fixes this by making area-proportional diagrams, or if that is impossible, a good approximation with included goodness-of-fit stats!
(Euler diagrams are very similar to venns, they just don't require every set to interact.)

## [Heatmaps](http://www.opiniomics.org/you-probably-dont-understand-heatmaps/)

A useful primer on what heatmaps actually tell us.

## [Upset plots](https://github.com/hms-dbmi/UpSetR)

I'm a big fan of Upset plots. If you have lots of groups in your data, and venn diagrams turn into a massive confusing mess, that's the time to try an upset plot. They use a matrix to represent different intersections, and a bar plot to visualise the number of elements in each intersection. You can also get fancy and introduce queries or extra plots that describe different features of your data. The only downside is I think there is currently a limit of 16 groupings per plot.

## [ggstatsplot](https://indrajeetpatil.github.io/ggstatsplot/)

Another package I'm a fan of. This package runs statistical tests, and creates plots with them included. Also makes lovely violin/box plot combinations which are much more informative than a straightforward box plot.

## [ggbeeswarm](https://github.com/eclarke/ggbeeswarm)

Are the points in your violin scatter plots overlapping so you can't see all the data? Ta-da, ggbeeswarm fixed it!

## [ggplot2 extensions](https://exts.ggplot2.tidyverse.org/gallery/)

All the extensions I've mentioned above and more!

## Online Textbooks

* [ggplot2: elegant graphics for data analysis](https://ggplot2-book.org/) - A guide to the Grammar of Graphics used by ggplot2 - for understanding theory.
* [R Graphics Cookbook](http://www.cookbook-r.com/Graphs/) - The whole book isn't available online, but some useful information is on the site about making data graphics in R.
* [Fundamentals of Data Visualisation](https://clauswilke.com/dataviz/) - A guide to effectively communicating your data using figures.

## [Biorender](https://biorender.com/)

If you need to make a figure to describe the biology behind your work or a potential mechanism, Biorender is a great resource - much easier than messing about in excel for hours! You'll need a license to use the figures in publications or download figures in the highest quality, so worth mentioning to your supervisor.

## [Draw.io](https://www.draw.io/index.html)

For making flowcharts to describe your pipelines.

## [The Pudding](https://pudding.cool/)

Not necessarily work related... but if you want a break and fancy looking at some cool uses of data vis, check The Pudding out.

## Some other pointers

Some of these pointers may not make sense until you're trying to make a certain plot, but I've put them here in the hopes they are useful (also so I don't forget...).

* If you use xlim/ylim or scale_y_continous() to zoom in on a boxplot, ggplot recalculates the range etc based on that limit. If you want to include the outliers but just zoom in without recalculation, use coord_cartesian() to change the limits.

