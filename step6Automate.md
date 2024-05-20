---
title: 'Step 6 - Automation'
teaching: 10
exercises: 0
---

# Can you automate any repetitive tasks?

Often, tasks that need to be done over and over again by a
human can be opportunities for human error to sneak in. Setting up an automated way of doing this can eliminate this issue. 


***It can save you time, energy and mental load.***


Automation doesn't need to be fancy. Working on small incremental automated improvements over time is perfect.


Coding allows you to be very automated, but there are tools you can use that don't need coding:

 - [MacOS Automator](https://support.apple.com/en-au/guide/automator/welcome/mac)

 - [Microsoft Power Automate](https://powerautomate.microsoft.com/en-us/blog/automate-tasks-with-power-automate-desktop-for-windows-10-no-additional-cost/)

 - Any Spreadsheet Macros and formulas

 - Workflow systems such as [KNIME](https://www.knime.com/) and [Orange Data Mining](https://orangedatamining.com/)


There are many other workflow automation platforms out there.

Even having an automated Sync client for your backups is a form of automation!


::::::::::::::::::::::::::::::::::::::::::::::: challenge

### Idea - Contact me form

It could be a link in your work that directs to a 'Contact me' form or a 'book a time with me' system. 

For example, you may have a 'Contact me' form that asks for 

 - Name

 - Email

 - What organisation are they from? 

 - What paper or resource do they wish to discuss? (URL)

 - Do they want to request [Data, Code, Other]?

 - What are their plans for the Data/Code?

 - If they are reusing the Data/Code, what licence do they plan to use?

This saves you:

- Time and effort sending multiple emails to gather this information

- Have only one place to update your email address if you move organisations or change name

You can even add some commonly requested links in your form, directing them to your protocols and data repositories, your organisation's repositories or somewhere central like an ORCID id page. 

You could automatically send them back an email with some expectation management ("I will get back to you within 10 business days") and information about your work, and have this form save to a spreadsheet, so you can keep a list of people who may be reusing your work. 

You can email them with your preferred citation ([helpful guide](https://the-turing-way.netlify.app/communication/citable/citable-cite)). Knowing how your work has been reused and referenced can be useful when you are applying for the next round of grants.

:::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::: challenge

### Idea - Automated systematic review

There are a number of tools available that can help you to conduct systematic literature reviews, including automation tools. 

Tools are often discipline specific, and your library or graduate school could provide some guidance on the best one to use.

For example, this list of resources from the[ University of North Carolina library](https://guides.lib.unc.edu/automation) has some great papers on different systems available.


::::::::::::::::::::::::::::::::::::::::::::::: 

::::::::::::::::::::::::::::::::::::::::::::::: challenge

### Idea - Photos and Videos

If you are taking photos and want to automatically convert them, it may be worth looking into [MacOS Automate](https://www.apple.com/sg/pro/photo/automation/renameconvertcaption.html) or . There's also plenty of [python scripts](https://github.com/andrewning/sortphotos) that have been published you could use. 

You could also use a command line such as [Windows on Linux Subsystem](https://learn.microsoft.com/en-us/windows/wsl/install) or Linux Terminal with a tool called [FFmpeg](https://ffmpeg.org/ffmpeg.html) or [sips](https://ss64.com/mac/sips.html) on Mac Terminal.

This eliminates potential manual mistakes of converting to the wrong format or different formats. If you have mixed formats in your folder, it may skew your analysis.

This also enables you to migrate to an accessible and open file format.

::::::::::::::::::::::::::::::::::::::::::::::: 


::::::::::::::::::::::::::::::::::::::::::::::: challenge

### Idea - Survey

Does your survey tool allow for automatic reminders to be sent to those who have not completed your survey?

Many survey tools have in-built functionality to speed up your workflow. 

This could potentially encourage more partipants to complete your surveys, growing your sample size. 

::::::::::::::::::::::::::::::::::::::::::::::: 

::::::::::::::::::::::::::::::::::::::::::::::: challenge

### Idea - Automated Sentiment Analysis

You could use a tool such as NLTK and Python to automate your sentiment analysis in a reproducible way.

This paper has a great rundown on how to do this:

Jiawei Yao 2019 J. Phys.: Conf. Ser. 1187 052020 Automated Sentiment Analysis of Text Data with NLTK, Retrieved 2024-04-17 at https://10.1088/1742-6596/1187/5/052020 licenced under Creative Commons Attribution 3.0 licence

::::::::::::::::::::::::::::::::::::::::::::::: 



::::::::::::::::::::::::::::::::::::::::::::::: challenge

### Idea - Take data and automate reports/graphs

If you are regularly taking in new data from external sources (sensor, DNA expression, weather mapping etc), you can use [R](https://kbroman.org/knitr_knutshell/) or [Python with Jupyter](https://docs.jupyter.org/en/latest/) to clean every dataset the same way, graph the datasets and write reports for you. You can even add caveats that your code would only run a report if the findings from that dataset were significant.

You can also use APIs or RSS feeds to automate the downloading of data.

Coding will always make you more reproducible.


::::::::::::::::::::::::::::::::::::::::::::::: 


::::::::::::::::::::::::::::::::::::::::::::::: instructor

This is a good opportunity to ask researchers what they wish they could automate. If you have a research support IT team, local research software developers or eResearch team, this is a good plug for them. 

::::::::::::::::::::::::::::::::::::::::::::::: 

# What is your next step?

::: tab 

### Beginner

A great place to start is:


Automate a single thing. 


### Advanced

Your next move can be:

Keep automating! It may be worth talking to your organisation's technical team to find out what licences are available or tools they could suggest for your workflow.


:::



::::::::::::::::::::::::::::::::::::::::::::::: callout

## References


Data Carpentry Reproducible Research Committee. "Automation for Reproducible Research." Version 2016.1, December 2016. Retrieved on 2024-04-17 at https://datacarpentry.org/rr-automation/ licenced as CC-BY 4.0

The Turing Way Community. (updated 2023) Citing Research Objects . Github.com Retrieved April 11, 2024, from https://the-turing-way.netlify.app/communication/citable/citable-cite licenced under CC-BY 4.0 licence


:::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::::::::::::: keypoints

### In this lesson, we have learnt:

- Why automation can be beneficial

- What tools are useful for automation

- Ideas on what to automate


#### We build trust in our knowledge by:

Showing how we automated work, to eliminate human error


#### We retain knowledge using:

Keeping a copy of these automations



#### We build business continuity by:

Having an automation, so that you are not relying on a staff member to perform this job. 

:::::::::::::::::::::::::::::::::::::::::::::::
