# Finding your dataset

Things to think about:

## What kind of data do you need?

* Microarray
* RNA-seq
* Ribo-seq
* SNPs in a given gene.

## Raw or processed data?

* Do you just need expression data (eg RPKM)? Then you can choose pre-processed data that someone else has quality filtered, aligned, normalised... etc.
* Pre-processed doesn't mean you don't have prep work! Go read the paper, particularly the methods. Understand what has happened to the data, and any weirdness to expect. Did they use exactly the same protocol on the control/treated data? You won't be able to interpret your results effectively unless you really know your dataset.
* Raw data - fastq files. These may need quality checks, adaptor and contaminant removal, alignment, etc. May be relatively straightforward - there are lots of friendly pipelines and tutorials, and you will have a better understanding of what has happened to the data.
* But things can and will go wrong. (They will anyway, welcome to computational biology. If you haven't had a meltdown over a rogue bracket you're doing it wrong) Lots of choices (which software to use), more software to install, more queuing on the cluster. Think about how much time you have.

## What species are you working on?

* Often this will be human - great! Lots of data available, well annotated genome and transcriptome - all of the good things. :dancers:
* Another model species - also great! However, think about the genetic background of your species. For example, lab mice are WEIRD. Most mouse genomes are from lab mice that have had all sorts of inbreeding and oddness - are they going to give a true answer to your question? On the other hand, there are strains bred specifically for cancer research. :mouse:
* A bit of a weird species - do your background. Go find out:
    * Is there a genome annotation?
    * Is it a good annotation? What's the N50? When was it last updated?

## Are you studying a disease, e.g. cancer?

* Exactly what cancer are you interested in?
* What kind of sample do you want? Tumour only, surrounding tissue.
* Treatment/no treatment/both?
* Do you need cancer patients and normal control tissue?
* How many variables are likely to impact your results? Age, tumour grade, sex, etc. Do the datasets you're looking at have this information?

## Availability

* Science and code should be open source and collaborative. Many journals now require that data is uploaded to a publicly accessible repository. However, not everyone sticks to this - everyone has read the words "data available upon reasonable request" :angry:
* If you think it's available... have you checked? These things are often an absolute pain, go test the system and be sure before you commit.
* Did you definitely check?? Go check.

You need to think about all these things and more. Sit down and think about your research question, and what you need to answer it. Then make yourself a list with two sections:

* Key features - what does a data set HAVE to have to be useful?
* Useful extras - what would it be great but not essential? Either for helping you ask more questions, or just to make your work more robust.

Then take your shopping list and go searching for your dream data!

## Data sources

### GEO (Gene Expression Omnibus)

* GEO lets you construct a very specific query for microarray data, with inclusion and exclusion criteria. Lovely stuff.
* [Link to a tutorial](https://www.ncbi.nlm.nih.gov/geo/info/qqtutorial.html).

### TCGA (The Cancer Genome Atlas)

* TCGA has lots of publicly available RNA-seq.
* Some of this requires [access](https://gdc.cancer.gov/access-data/obtaining-access-controlled-data), but most is publicly available.
* You can build a [query](https://docs.gdc.cancer.gov/Data_Portal/Users_Guide/Advanced_Search/) and specify open access only.
* Example query for open access, colon cancer RNA-seq data:

> files.access in ["open"] and files.cases.primary_site in ["colon"] and files.data_category in ["transcriptome profiling"] and files.data_type in ["Gene Expression Quantification"] and files.experimental_strategy in ["RNA-Seq"]
