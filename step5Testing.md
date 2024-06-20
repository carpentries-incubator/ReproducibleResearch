---
title: 'Step 5 - Testing and Controls'
teaching: 20
exercises: 0
---


## Testing for Validity and Integrity

Unintended changes to datasets happen all the time. An added comma in a sentence can throw out a line in a spreadsheet. Missing data can alter a calculation. A broken link or download that didn't complete properly can short us of data without us realising.

But what can we do about this?

There are a few checks we can run to help identify when this has happened.

 - Is there the expected number of lines?

 - Are there the expected number of columns?

 - If you sort a column and find the unique entries, do those entries make sense? For example, in a column that you're expecting to find months, is there the word "Monday" in it? If so, there may have been some movement in your cells.

 - Do the calculations make sense? If you have a range of 1-100 for an attribute, is the mean of that column an impossible number such as 254?

 - Does an analysis fail to run? If you look into it, there may be an unexpected value, such as a letter where it was expecting a number.

[Open Refine](https://openrefine.org/) is a good tool for inspecting your data.

Again, R and Python have real strengths here, to have a list of tests you can run as often as you need. For example, R has a function called 'head' that prints the first 6 lines of any file, so you can do a visual check of the data quickly.

::::::::::::::::::::::::::::::::::::::::::::::: callout


### Coding Resources for testing the integrity of data


 - [Testing for Python](https://github.com/ADACS-Australia/good-code-etiquette/blob/master/Testing.ipynb)

 - The [Carpentries software programming courses](https://software-carpentry.org/lessons/) also run through some basic tests in their workshops

 - [Testing for R](https://r-pkgs.org/testing-basics.html)

 - [The Turing Way](https://the-turing-way.netlify.app/reproducible-research/code-quality/code-quality-robust) has a great tutorial on how to write robust code.



::::::::::::::::::::::::::::::::::::::::::::::: 


::::::::::::::::::::::::::::::::::::::::::::::: discussion

## Microsoft Excel changing Gene names

As per the following paper:
Ziemann, M., Eren, Y. & El-Osta, A. Gene name errors are widespread in the scientific literature. Genome Biol 17, 177 (2016). https://doi.org/10.1186/s13059-016-1044-7 licenced as CC-BY 4.0

" The spreadsheet software Microsoft Excel, when used with default settings, is known to convert gene names to dates and floating-point numbers. A programmatic scan of leading genomics journals reveals that approximately one-fifth of papers with supplementary Excel gene lists contain erroneous gene name conversions."


In a follow up story:
Abeysooriya M, Soria M, Kasu MS, Ziemann M (2021) Gene name errors: Lessons not learned. PLoS Comput Biol 17(7): e1008984. https://doi.org/10.1371/journal.pcbi.1008984

"[The previous] article on this topic led the Human Gene Name Consortium to change many of these gene names to be less susceptible to autocorrect."


To remedy this, there is now an option to turn off automatic data conversion - but you need to be aware of it.

It was suggested to reviewers and editorial staff:

"the kind of errors we describe can be spotted by copying the column of gene names and pasting it into a new sheet, and then sorting the column. Any gene symbols converted to dates will appear as numbers at the top of the column."


::::::::::::::::::::::::::::::::::::::::::::::: 

::::::::::::::::::::::::::::::::::::::::::::::: instructor

Can do this next challenge in the class, either pen and paper, on the board or in the chat.

::::::::::::::::::::::::::::::::::::::::::::::: 

::::::::::::::::::::::::::::::::::::::::::::::: challenge

# Where did the pizza go wrong?

We've shared our pizza recipe with our friend, who attempted to cook it last night. They've called you up today and said "It didn't work out... why?"

What questions can we ask to discover what could have gone wrong?

:::::::::::::::::::::::::::::::: solution

***Questions could include:***

Was it burnt? Or did the cheese not melt?

Is the base too thick/tough?

Does the ingredients taste 'off'?



::::::::::::::::::::::::::::::::

Now for each question, let's develop a test. We want to offer a way for our friend at each step to 'test' that their pizza is on the correct track.

:::::::::::::::::::::::::::::::: solution

***Tests could include:***

Was the oven on 190 degrees celsius, for 20 minutes?

Did the cheese melt?

Did the dough double in size when it rose?

Were the ingredients still in their use by or due date?



::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::: 



### Physical Testing and Quality Assurance

Consider your 'hardware'- the machines and devices you use in your research. Are they callibrated? For your control samples, are you getting the expected outcomes?

Consider your 'consumables' - Have your reagents gone out of date? Stored and labelled correctly? Did your blood samples heat up during transportation?

***Document how you have checked and accounted for Quality Assurance***


::::::::::::::::::::::::::::::::::::::::::::::: callout

### Quality Assurance

[Baker, M. How quality control could save your science. Nature 529, 456–458 (2016). https://doi.org/10.1038/529456a](https://doi.org/10.1038/529456a)


::::::::::::::::::::::::::::::::::::::::::::



# Providing Authenticity and Validity


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

::::::::::::::::::::::::::::::::::::::::::::::: challenge

Pizza test

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

A good time for suggestions on where to learn R and Python. You've probably already included it elsewhere, just remind people at this point.

::::::::::::::::::::::::::::::::::::::::::::::: 


<!-- Got any organisation information on where to learn R or Python? Does your institute run carpentries training or data science help? Include it below.

It will appear at https://[YourRepository]/ReproducibleResearch/instructor/step5Testing.html#tracking-your-analysis-history

-->


If you are using a random number generator, take note of the seed number.


***This is a lot of work. What are the benefits to me?***

1. Infinite undo's: Control versions between active,
live and archived.

2. Branching and experimentation: Copy code or other
technical formulae and change to test hypotheses

3. Collaboration: Track changes, merge input.



***These analysis pipelines can be saved as part of your folder structure from lesson 1.***



:::::::::::::::::::::::::::::::::::::::: testimonial

***Publishing these pipelines, either as part of your publication, as a protocol or in a public repository such as OSF, Github or similar improves your reproducibility, and provides others a greater understanding of your work.***



[Step 3 - Publishing Protocols link.](step3MethodStats.html#publishing-your-protocol)

:::::::::::::::::::::::::::::::::::


::::::::::::::::::::::::::::::::::::::::::::::: instructor

Include links from your institute about where to publish analysis pipelines - your institute may have a preferred place, or your Office of Research or Library may have a good write up on this.

::::::::::::::::::::::::::::::::::::::::::::::: 


<!-- Got any organisation information on publishing analysis pipelines? Do you suggest github etc? Do you have a licencing person? Include it below.

This will appear on https://amandamiotto.github.io/ReproducibleResearch/instructor/step5Testing.html#tracking-your-analysis-history

-->



::::::::::::::::::::::::::::::::::::::::::::::: discussion

### Standard Operating Procedures

We talked about [Standard Operating Procedures](
step4Doco.html#standard-operating-procedure) in Step 4 - Documentation. This is where a SOP is really powerful - your pipeline can even be part of your SOP.

:::::::::::::::::::::::::::::::::::::::::::::::


### Version Control and Tracking


Let's now consider tracking your versions of your analysis pipeline. 

You may be making changes to your analysis pipeline as you go

 - How are you taking notes of these changes?

 - What version of software are you using? 

 - Have you noted what version of the libraries you are using are? 

 - Have you noted the name, model and version number of any hardware you may be using (for example, cameras, microscopes, MRI machines, IoT sensors)?

Version control is keeping track of each change you have made, so that if you need to go back to a previous version of your analysis pipeline, you can!

Think of version control as an 'undo' button.

::::::::::::::::::::::::::::::::::::::::::::::: discussion

We have already learnt some skills in [step 1 - Organising your files and folders](step1Folders.html#file-naming-conventions) to track versions of files. We can use the same principles here. Your pipelines can be labelled V1.0, V1.1 etc.

You can use the first number as a major step in versions (for example, Draft v1.0 to Reviewed v2.0), and the second number as a minor step in versions to indicate a change has occured (from v1.1 to v1.2).

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

### Containers

You may even want to try [Containers](https://carpentries-incubator.github.io/docker-introduction/) to publish your workflows. Think about Containers like a machine with all the instructions and installations inside - you can pass this box to others. They can put data into the machine, and processed data comes out the other side, without needing to pull apart and put the box together.

Containers also build automation into our workflows - we'll talk more about automation in our next lesson.

### Using Machine Learning?

The following paper may be useful to learn about ML platforms and reproducibility.

[R. Isdahl and O. E. Gundersen, "Out-of-the-Box Reproducibility: A Survey of Machine Learning Platforms," 2019 15th International Conference on eScience (eScience), San Diego, CA, USA, 2019, pp. 86-95, doi: 10.1109/eScience.2019.00017.](https://10.1109/eScience.2019.00017)



# What is your next step?

::: tab 



### Beginner

A great place to start is:

Save your analysis pipeline and store it safely in your organised folders.



### Advanced

Your next move can be:

 - Ensure your data is well described (As per Step 2).

 - Check that it is clear which of your datasets pair with your Analysis pipelines and in what order.

 - Publish your protocols and code.

:::

::::::::::::::::::::::::::::::::::::::::::::::: callout

## Resources

[Data authenticity](https://dmeg.cessda.eu/Data-Management-Expert-Guide/3.-Process/Data-authenticity)

[Tracking Changes in Research](https://carpentries-lab.github.io/good-enough-practices/06-track_changes.html)

[Reproducibility in Excel](https://osf.io/p2bdq/)

ADACS-Australia/good-code-etiquette. Manodeep Sinha, Paul Hancock, Rebecca Lange (2019, October 18). GitHub. Retrieved on 2024-04-17 from https://github.com/ADACS-Australia/good-code-etiquette/tree/master licenced as Creative Commons Attribution-ShareAlike 4.0 International License.


R-Pkgs Hadley Wickham and Jennifer Bryan (2024) '13 Testing basics' Retrieved on 2024-04-17 https://r-pkgs.org/testing-basics.html licenced as CC BY-NC-ND 4.0

::::::::::::::::::::::::::::::::::::::::::::::: 


::::::::::::::::::::::::::::::::::::::::::::::: callout

## References

OFS. Valerie Collins Alicia Hofelich Mohr Samantha T Porter(2023) Reproducible research practices in Excel (yes, Excel) Retrieved on 2024-04-17 from https://osf.io/p2bdq/ licenced as CC-By Attribution 4.0 International 

The Turing Way Community. (updated 2023) Writing robust code . Github.com Retrieved April 11, 2024, from https://the-turing-way.netlify.app/reproducible-research/code-quality/code-quality-robust licenced under CC-BY 4.0 licence

Ziemann, M., Eren, Y. & El-Osta, A. Gene name errors are widespread in the scientific literature. Genome Biol 17, 177 (2016). https://doi.org/10.1186/s13059-016-1044-7 licenced as CC-BY 4.0

Abeysooriya M, Soria M, Kasu MS, Ziemann M (2021) Gene name errors: Lessons not learned. PLoS Comput Biol 17(7): e1008984. https://doi.org/10.1371/journal.pcbi.1008984 licenced as CC-BY 4.0

:::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::: keypoints

### In this lesson, we have learnt:

- Why we should be checking our data for validity and integrity during processing

- What we should be looking for when inspecting our data

- Tools for inspecting data

- Physical testing and hardware QA plays an important part too

- Our data may have a lineage of origin, and we need to be aware and document the provenance of our data

- It is important to track our analysis history (and how to record it)

- That version control is a way to track changes over time


#### We build trust in our knowledge by:

- We are testing our data for validity and integrity - and being able to show how we are testing!

- We are tracking our versions of software, hardware and analysis pipelines, so that it is easier to reproduce later


#### We retain knowledge using:

- Tracking metadata about our data (for example, where did an image come from? Who originally made the dataset?) for later reference

- Recording the different versions of software and hardware, so we can go back to previous versions for reproducibility.

- Tracking the different versions of our analysis pipelines



#### We build business continuity by:

- Keeping versions of our analysis pipeline, so that it is clear what the latest version of the analysis pipeline was

- Recording the different version hardware and software

- Sharing where the data originated from via its data lineage information

:::::::::::::::::::::::::::::::::::::::::::::::
