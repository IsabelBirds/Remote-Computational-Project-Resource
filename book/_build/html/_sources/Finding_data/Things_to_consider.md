# Things to think about when finding data

There is a wealth of data available online, and this will only increase as more journal prioritise open, reproducible science, and as sequencing costs continue to drop.
However, this can also be quite overwhelming.
If you are looking for data to answer a certain research question, thinking about what you need before you start looking can help to narrow and focus your search.

Things to consider:

## What kind of data do you need?

Considering the kind of data you want is a simple way narrow down your search.

For example:

* Microarray
* RNA-seq
* Ribo-seq
* SNPs in a given gene.

## Do you need raw or processed data?

In some cases, you may not need raw data, and can look for data that has already undergone quality filtering, aligning, and normalisation, for example. This could include expression data, where you just need to know the RPKM of certain transcripts.

However, finding pre-processed data doesn't mean you don't have prep work!
You should read the associated paper, particularly the methods.
Try to understand what has happened to the data, and any weirdness to expect.
Did the authors use exactly the same protocol on the control/treated data?
You won't be able to interpret your results effectively unless you really know your data.

Raw data, such as fastq files, will need more work from you, including quality checks, adaptor and contaminant removal, and alignment.
This may be relatively straightforward - there are lots of friendly pipelines and tutorials - but is quite intimidating for a beginner.

The advantage of getting raw data is you will have a better understanding of what has happened to the data, although you will still need to read the paper to understand how it was generated!
However, things can and will go wrong.
There are more choices for you when using raw data, for example which software to use, and more software to install and run.
It is worth considering how much time you have for your project.

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
* How many variables are likely to impact your results? Age, tumour grade, sex, etc. Does the data you're looking at include this information?

## Availability

* Science and code should be open source and collaborative. Many journals now require that data is uploaded to a publicly accessible repository. However, not everyone sticks to this - everyone has read the words "data available upon reasonable request" :angry:
* If you think it's available... have you checked? These things are often an absolute pain, go test the system and be sure before you commit.
* Did you definitely check?? Go check.

You need to think about all these things and more. Sit down and think about your research question, and what you need to answer it. Then make yourself a list with two sections:

* Key features - what does a data set HAVE to have to be useful?
* Useful extras - what would it be great but not essential? Either for helping you ask more questions, or just to make your work more robust.

Then take your shopping list and go searching for your dream data!
