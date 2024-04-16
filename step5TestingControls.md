---
title: 'Step 5 - Testing and Controls'
teaching: 15
exercises: 0
---


# Proving Authenticity and Validity

Showing Provenance

::::::::::::::::::::::::::::::::::::::::::::::: spoiler

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

::::::::::::::::::::::::::::::::::::::::::::::: 


This may be a good time for a refresh of Step 1 - [Metadata on your files](https://amandamiotto.github.io/ReproducibleResearch/instructor/step1Folders.html#metadata-of-your-files)

::::::::::::::::::::::::::::::::::::::::::::::: instructor

May be a natural space to ask people what types of data they are working with, where is it coming from?

::::::::::::::::::::::::::::::::::::::::::::::: 



### Tracking your Analysis history

Now that we know where our raw data come from and how it was made, let's think about the changes we make to it.

Let's start with data cleaning. Have you made a log of the changes you have made?

Open Refine, NVIVO and SPSS all have logs of actions that you can download and save.

This is also where R and Python have huge strengths. Writing an R or Python script enables you to rerun with certainty the same analysis every time.

::::::::::::::::::::::::::::::::::::::::::::::: instructor

Insert R and Python service plug here. You've probably already included it elsewhere, just remind people at this point.

::::::::::::::::::::::::::::::::::::::::::::::: 

### Version Control

Retaining a copy of your raw data prior to any cleaning or analysis can be useful here.

If you are using R or Python, your next best friend is Git. 

Git is a program to track changes in your code. You may have heard of Github or Gitlab - these are cloud platforms that use the Git program to track your code as you write it.

To learn more about Git:

[The British Ecological Society](https://www.britishecologicalsociety.org/wp-content/uploads/2017/12/guide-to-reproducible-code.pdf) has a great Git tutorial under 'Version Control'.

[Start your journey in GitHub](https://docs.github.com/en/get-started/start-your-journey/hello-world)


# Testing for Validity

Unintended changes to datasets happen all the time. An added comma in a sentence can throw out a line in a spreadsheet. Missing data can alter a calculation. A broken link or download that didn't complete properly can short us of data without us realising.

But what can we do about this?

There are a few checks we can run to help identify when this has happened.

Is there the expected number of lines?

Are there the expected number of columns?



# Having controls






# Understanding and handling Risks



https://carpentries-lab.github.io/good-enough-practices/06-track_changes.html

::::::::::::::::::::::::::::::::::::::::::::::: instructor


::::::::::::::::::::::::::::::::::::::::::::::: 



# What is your next step?

#### As a Beginning step, a great place to start is....



#### As an Advanced step, your next move can be....


::::::::::::::::::::::::::::::::::::::::::::::: callout

## Resources

https://dmeg.cessda.eu/Data-Management-Expert-Guide/3.-Process/Data-authenticity

::::::::::::::::::::::::::::::::::::::::::::::: 


::::::::::::::::::::::::::::::::::::::::::::::: callout

## References

Wikipedia contributors. (2024, March 12). Provenance. In Wikipedia, The Free Encyclopedia. Retrieved 04:46, April 16, 2024, from https://en.wikipedia.org/w/index.php?title=Provenance&oldid=1213412590 licenced under Creative Commons Attribution-ShareAlike License 4.0


:::::::::::::::::::::::::::::::::::::::::::::::