---
title: 'Step 2 - Keeping your files Tidy and Organized'
teaching: 30
exercises: 1
---


Build your knowledge trust when sharing with collaborators or publication with well organized datasets. This also saves time in data cleaning, and ensures analysis pipelines are robust.

Let's look at a few concepts that can help.




### How to structure Column Data - Tidy data format

Tidy data developed by Hadley Wickham offer a set of rules to record, organise, and maintain data to ensure your analysis is effective, reproducible, and manageable.

The principles of tidy data provide a standard way to organize data values within a dataset.

Tidy data is a standard way of mapping the meaning of a dataset to its structure. A dataset is messy or tidy depending on how rows, columns and tables are matched up with observations, variables and types. 

The fundamental principles of tidy data are:

1. Each variable is a column
   
2. Each row is an observation
   
3. Each cell contains one value



Let's look at an example:

Each variable is in a separate column  i.e. the thing you’re measuring, like ‘age’ or ‘temperature’ or ‘height’. 
Each observation is in a separate row
Each cell contains one value (either a number or character string) 

Let's look at an example:

![First example with full address in one cell](/episodes/fig/TidyDataExample1.png){alt='First Example where full address is in one cell'}

This format could cause a number of issues.
- There is little control or guidance around when to use spaces, new lines or commas in this format. Commas especially can lead to a shift in data across your cells - meaning half of your address may end up in neighbouring cells, overwriting or shifting the rest of the line.
- Searching via State or Postcode would be extremely complicated.
- There is little clarity on what information should be included. One line contained the country, another did not. 
- Difficult to see/check if some part of the address is missing.

Let's look at a tidy example:

![Second example with address across multiple cells](/episodes/fig/TidyDataExample2.png){alt='Second example where information is broken down into individual cells'}

This format includes a lot of benefits:
- It is clear what is expected to include
- Easier to search
- Less likely to get extra whitespace or punctuation that could cause issues with analysis software

When multiple people are entering data manually, it may be beneficial to use a survey that fills in a spreadsheet for you. This can include dropdown menu items to ensure consistancy in certain columns - for example, to eliminate a combination of "Monday, Mon, M, mon".

Other useful concepts:

### Dates:

Where possible, always use the formal YYYY-MM-DD for your dates. It will make searching for dates much easier. In addition, adding the additional zero (for example, March would be 03 ) means that when you sort your file, months and days will be in order. Otherwise, you may have Jan (1), Oct (10), Nov (11), Dec (12), Feb (2). 


### Special Characters:

It is best to avoid punctuation or special characters in your cells or data entry. Some analysis tools may read certain characters incorrectly or produce an error. 

::::::::::::::::::::::::::::::::::::::::::::::: instructor

Point out the resources segment here, there's a really good tutorial in the Data Carpentry for Ecology page that covers a range of spreadsheet things

This is also an opportunity to do a live exercise - you could pull up a bad dataset and ask participants to point out potential improvements.

::::::::::::::::::::::::::::::::::::::::::::::: 


### Interview considerations

When working with interviews, you may choose to only retain transcripts. However, it is also worth recording what non-verbal queues were shown. Is there a part of the interview where the participant expressed a strong emotion? Were they comfortable or nervous? Did they fidget a lot or laugh a lot? Long pauses? 

Including any personal observations alongside a video can become incredibly useful when it comes to analysis time, or to refresh your memory upon review. It could also be important to support your insights when writing your paper.



### How to handle missing data

As a project team, it is important to have a consistant way of managing missing data. 

If data is missing from a cell, are you going to use a blank cell? Or a placeholder such as NA, NULL or N/A ? It's generally unadvisable to use zero, as this can have an effect on any calculations done in those cells.

Should the whole observation be discluded? Has your methodology accounted for how to handle this scenario and any potential skewing of results? When publishing, have you discussed how missing data is handled and accounted for?

A helpful resource can be found here: [Paper on the prevention and handling of the missing data](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3668100/)

How to handle missing data in cells can be covered by this section of [Data Carpentry in Ecology](https://datacarpentry.org/spreadsheet-ecology-lesson/02-common-mistakes.html#null)

Later, we will talk about how to test for missing data.



:::::::::::::::::::::::::::::::::::::::::::::::  callout

## Tools

#### Tools that don't involve programming:

[Open Refine](https://openrefine.org/) is an open source (free) tool that is incredibly useful to clean column data. Your data [doesn't leave your computer](https://openrefine.org/privacy), which makes it safer when working with sensitive data.

Any survey tool may also be of benefit.

#### Programming Tools:
R has the Tidyverse library, also written by Hadley Wickham
Python has the Pandas library, which follows similar principles. You may also find NumPy useful.
:::::::::::::::::::::::::::::::::::::::::::::::


::::::::::::::::::::::::::::::::::::::::::::::: callout
## Resources

[Common formatting problems - Data Carpentry](https://datacarpentry.org/spreadsheet-ecology-lesson/02-common-mistakes.html)

[Paper on the prevention and handling of the missing data](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3668100/)


::::::::::::::::::::::::::::::::::::::::::::::: 



## What is your next step?

#### As a Beginning step, a great place to start is....
- Decide how to handle missing data
- Use YYYY-MM-DD for dates


#### As an Advanced step, your next move can be....
- You can start to work in a data science language such as R or Python. [The Carpentries](https://software-carpentry.org/lessons/) data science lessons are a great place to start, made for researchers who have never coded before. Workshops are held across the world.



::::::::::::::::::::::::::::::::::::::::::::::: callout

## References

Wickham, H. . (2014). Tidy Data. Journal of Statistical Software, 59(10), 1–23. https://doi.org/10.18637/jss.v059.i10 licenced as Creative Commons Attribution License (CC-BY)

Broman, K. W., & Woo, K. H. (2018). Data Organization in Spreadsheets. The American Statistician, 72(1), 2–10. https://doi.org/10.1080/00031305.2017.1375989 licenced as Attribution-NonCommercial-NoDerivatives (CC-BY-NC-ND)

White, Ethan & Baldridge, Elita & Brym, Zachary & Locey, Kenneth & McGlinn, Daniel & Supp, Sarah. (2013). Nine simple ways to make it easier to (re)use your data. 10.7287/peerj.preprints.7v1. 
 licenced as Creative Commons Attribution License (CC-BY)

Kang H. The prevention and handling of the missing data. Korean J Anesthesiol. 2013 May;64(5):402-6. doi: 10.4097/kjae.2013.64.5.402. Epub 2013 May 24. PMID: 23741561; PMCID: PMC3668100. licenced as Creative Commons Attribution Non-Commercial License (CC-BY-NC)

:::::::::::::::::::::::::::::::::::::::::::::::
