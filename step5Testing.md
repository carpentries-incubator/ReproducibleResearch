---
title: 'Step 5 - Testing and Controls'
teaching: 15
exercises: 0
---


# Proving Authenticity and Validity

Showing Provenance

::::::::::::::::::::::::::::::::::::::::::::::: callout

Provenance can mean different things to different people. 

Archaeology and anthropology researchers use provenience to refer to the exact location or find spot of an artifact, a bone or other remains, a soil sample, or a feature within an ancient site, whereas provenance covers an object's complete documented history. 

Alternatively, in the geologic use of the term, provenance instead refers to the origin or source area of particles within a rock, most commonly in sedimentary rocks. It does not refer to the circumstances of the collection of the rock.


:::::::::::::::::::::::::::::::::::::::::::::::

Today, we'll focus on data provenance, otherwise known as data lineage.

### Data lineage

Data lineage considers the data origin, what happens to it, and where it moves over time.

Consider your research data. What is its original source?

Did you obtain it through:

- Conducting a survey?

- Work in the physical field (such as tree mapping or rock art identification)?

- From a collaborator?

- Open dataset online?

- A physical object (such as paintings)

- A catalogue of images (such as satellite imagery)

::::::::::::::::::::::::::::::::::::::::::::::: discussion

If it is something you haven't created from scratch, such as a trial result or data collecting, have you noted where that source is? 

Have you noted where your source obtained the information?

Your source may not be the data owner - who is?

What copyright and access limitations are on the data?

If you are using a repository that is regularly updated (satellite images, weather patterns, government policies or legislations etc), have you noted the version of the data?

::::::::::::::::::::::::::::::::::::::::::::::: 

***This is all useful information to include in your documentation***


This may be a good time for a refresh of Step 1 - [Metadata on your files](https://amandamiotto.github.io/ReproducibleResearch/instructor/step1Folders.html#metadata-of-your-files)

::::::::::::::::::::::::::::::::::::::::::::::: instructor

May be a natural space to ask people what types of data they are working with, where is it coming from?

::::::::::::::::::::::::::::::::::::::::::::::: 



### Tracking your Analysis history

Now that we know where our raw data come from and how it was made, let's think about the changes we make to it.

Let's start with data cleaning. Have you made a log of the changes you have made?

Open Refine, NVIVO and SPSS all have logs of actions that you can download and save.


 - SPSS analysis pipeline comes as a .sps script file. You may see it referenced as 'Syntax'

 - SAS has a .sas file for pipelines

 - STATA has a .do file for pipelines. You may see it referenced as ‘commandlog’


This is also where R and Python have huge strengths. Writing an R or Python script enables you to rerun with certainty the same analysis every time.


::::::::::::::::::::::::::::::::::::::::::::::: instructor

Insert R and Python service plug here. You've probably already included it elsewhere, just remind people at this point.

::::::::::::::::::::::::::::::::::::::::::::::: 

If you are using a random number generator, take note of the seed number.


***This is a lot of work. What are the benefits to me?***

1. Infinite undo's: Control versions between active,
live and archived.

2. Branching and experimentation: Copy code or other
technical formulae and change to test hypotheses

3. Collaboration: Track changes, merge input.



***These analysis pipelines can be saved as part of your folder structure from lesson 1.***

:::::::::::::::::::::: testimonial

***Publishing these pipelines, either as part of your publication or in a public repository such as OFS, Github or similar improves your reproducibility, and provides others a greater understanding of your work.***

::::::::::::::::::::::::::


::::::::::::::::::::::::::::::::::::::::::::::: instructor

Include links from your institute about where to publish analysis pipelines - your institute may have a preferred place, or your Office of Research or Library may have a good write up on this.

::::::::::::::::::::::::::::::::::::::::::::::: 

::::::::::::::::::::::::::::::::::::::::::::::: discussion

### Resources

[Reproducibility in Excel](https://osf.io/p2bdq/)


::::::::::::::::::::::::::::::::::::::::::::::: 


### Version Control and Tracking


Let's now consider tracking your versions of your analysis pipeline.

You may be making changes to your analysis pipeline as you go

 - How are you taking notes of these changes?

 - What version of software are you using? 

 - Have you noted what version of the libraries you are using are? 

 - Have you noted the name, model and version number of any hardware you may be using (for example, cameras, microscopes, MRI machines, IoT sensors)?

::::::::::::::::::::::::::::::::::::::::::::::: discussion

We have already learnt some skills in [step 1 - Organising your files and folders](step1Folders.html#file-naming-conventions) to track versions of files. We can use the same principles here. Your pipelines can be labelled V1.0, V1.1 etc.

::::::::::::::::::::::::::::::::::::::::::::::: 


#### Using computational tools

If you are using R or Python, your next best friend is Git. 

Git is a program to track changes in your code. You may have heard of Github or Gitlab - these are cloud platforms that use the Git program to track your code as you write it.

Sharing your analysis pipeline then becomes easy. You can even write reports with both plain text, R or Python code and the results in graphs in platforms such as Jupyter.


::::::::::::::::::::::::::::::::::::::::::::::: callout

### To learn more about Git

[The British Ecological Society](https://www.britishecologicalsociety.org/wp-content/uploads/2017/12/guide-to-reproducible-code.pdf) has a great Git tutorial under 'Version Control'.

[Start your journey in GitHub](https://docs.github.com/en/get-started/start-your-journey/hello-world)

The Carpentries has a [Software Carpentry - Version Control with Git](https://swcarpentry.github.io/git-novice/) lesson you can follow.

::::::::::::::::::::::::::::::::::::::::::::::: 

Retaining a copy of your raw data prior to any cleaning or analysis is also useful to version control.

You may even want to try [Containers](https://carpentries-incubator.github.io/docker-introduction/) to publish your workflows. Think about Containers like a machine with all the instructions and installations inside - you can pass this box to others. They can put data into the machine, and processed data comes out the other side, without needing to pull apart and put the box together.

### Using Machine Learning?

The following paper may be useful to learn about ML platforms and reproducibility.

[R. Isdahl and O. E. Gundersen, "Out-of-the-Box Reproducibility: A Survey of Machine Learning Platforms," 2019 15th International Conference on eScience (eScience), San Diego, CA, USA, 2019, pp. 86-95, doi: 10.1109/eScience.2019.00017.](10.1109/eScience.2019.00017)


# Testing for Validity

Unintended changes to datasets happen all the time. An added comma in a sentence can throw out a line in a spreadsheet. Missing data can alter a calculation. A broken link or download that didn't complete properly can short us of data without us realising.

But what can we do about this?

There are a few checks we can run to help identify when this has happened.

Is there the expected number of lines?

Are there the expected number of columns?

Again, R and Python have real strengths here, to have a list of tests you can run as often as you need.



# Having controls






# Understanding and handling Risks



https://carpentries-lab.github.io/good-enough-practices/06-track_changes.html

::::::::::::::::::::::::::::::::::::::::::::::: instructor


::::::::::::::::::::::::::::::::::::::::::::::: 



# What is your next step?

#### As a Beginning step, a great place to start is....

Save your analysis pipeline and store it safely in your organised folders.

#### As an Advanced step, your next move can be....


::::::::::::::::::::::::::::::::::::::::::::::: callout

## Resources

https://dmeg.cessda.eu/Data-Management-Expert-Guide/3.-Process/Data-authenticity

::::::::::::::::::::::::::::::::::::::::::::::: 


::::::::::::::::::::::::::::::::::::::::::::::: callout

## References

Wikipedia contributors. (2024, March 12). Provenance. In Wikipedia, The Free Encyclopedia. Retrieved 04:46, April 16, 2024, from https://en.wikipedia.org/w/index.php?title=Provenance&oldid=1213412590 licenced under Creative Commons Attribution-ShareAlike License 4.0

OFS. Valerie Collins Alicia Hofelich Mohr Samantha T Porter(2023) Reproducible research practices in Excel (yes, Excel) Retrieved on 2024-04-17 from https://osf.io/p2bdq/ licenced as CC-By Attribution 4.0 International 


:::::::::::::::::::::::::::::::::::::::::::::::