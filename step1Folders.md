---
title: 'Step 1 - Organising your files and folders'
teaching: 10
exercises: 0
---


Having a standard folder structure can keep your files organised and save you time looking for data. 




# Planning to be organised


#### Data Management Plan

A data management plan (DMP) is a living document for a research project, which outlines data creation, data policies, access and ownership rules, management practices, management facilities and equipment, and who will be responsible for what.

You can find [example templates here](https://ardc.edu.au/resource/data-management-plans/)


::::::::::::::::::::::::::::::::::::::::::::::: instructor


Link to your institutional Data Management Planning Page


:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::


### Folder Structures

Having your folders structured in a hierarchical format can be one of the best ways to stay organised.

There are benefits to this:

 - It is harder to lose files

 - When working with collaborators, it is easier to understand where everything is

 - If you need to go into your previous projects, you can quickly see where files are


While you can create your own folder templates, there are templates you can use:


[A simple example by the Turing Way project](https://the-turing-way.netlify.app/reproducible-research/compendia#basic-compendium)

[Project TIER](https://www.projecttier.org/tier-protocol/protocol-4-0/root/)


It is worth checking with your research group and local librarians if there is a pre-existing folder structure template that you can use.

Once your projects have finished, you may want to consider archiving your project folder.

#### Raw data

Keep a copy of your raw data backed up elsewhere, and never alter it. This means if you realise early in your work, there has been an error introduced into the data, you can retrieve a raw copy and reanalyse it.

::::::::::::::::::::::::::::::::::::::::::::::: instructor


This is a good time to talk about what research data storage options you have at your institute. Cover how backups work (and the difference between backup and whole system recovery, which are two different things).


:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::


:::::::::::::::::::::: testimonial

Don't forget - backups are your friend here. 

:::::::::::::::::::::::::::::::::::::::



### File naming conventions

There are a number of things to consider when naming files:

- Name folders in a meaningful way. 

- Don't use staff names

- Decide on a standard vocabulary across the research group and stick to it.  For example, will everyone call a location by Town name, town initials, postcode, state etc. 

- Instead of using 'Draft' in a filename, consider using version numbers. Your first version may be 1.0, so your filename may be ProjectReportv1.0 , then when someone edits it and sends it back, it may then become ProjectReportv1.1 .You could use a date and initials to mark it as well. So a report edited on 1st May 2024 by Amanda Miotto could be ProjectReportv1.1_20240501_AM

- Label any dates as YYYYMMDD . This can save confusion across international collaborators, and it makes it easier to search. We'll talk about this more in the next lesson.

There is an excellent list [of 13 rules for naming conventions](https://www.ed.ac.uk/records-management/guidance/records/practical-guidance/naming-conventions) worth the read.


#### Who is reading your file names?

Three principles for file names:
There are three key principles to guide file naming convention development, as defined by Data Carpentry and Martinez (2015):

 - Machine readable

 - Human readable

 - Plays well with default ordering


Lets discuss each key principle below.

##### ***Machine readable***

Within the context of file naming conventions, being machine readable means:

 - Spaces have been avoided. Ideally there are no spaces in any file names.

 - Special characters are used in lieu of spaces i.e. _ or -

 - Case sensitivity is consistent

::::::::::::::::::::::::::::::::::::::::::::::: discussion

#### Windows and mounted drive file name limits

If you are working in a Windows system and mounting a drive on your computer, there is an upper limit to how long your file names can be. The joined file name and file path is limited to 256 characters.

For example, if you have on a hard drive a file called 

\mainDrive\ProjectWildMappingAcrossAust\Australia\Queensland\GoldCoast\SiteHinesDam\WildlifeMapping_2022_04_20\Collected_by_Amanda_Miotto\Griffith_UniversityQld\Dataset_WildIbis\Ibis_Observed_on_2022_4_20\Sector_35_x_328\Upper_Water_Level\Hourly_Count_of_organisms\2024_04_20_13h_53min.csv

And you wanted to map this \mainDrive folder onto your computer, this would fail.

A way to handle this is by mapping one of the folders further into the filepath. So for example, you may choose to mount the folder GoldCoast instead of mainDrive.

:::::::::::::::::::::::::::::::::::::::::::::::

***Globbing***

Another concept in machine readbilty is globbing.

Globbing is the concept of using a wild card symbol, typically a * followed by an extension or consistent string. This wildcard tells the computer to search for all files with that extension or string. For example * .jpg will search for all JPEG files in a directory. An example is shown below

![Source: Carpentry, D. and Martinez, C. (2015) File organization: Naming, File Organization: File Organization: Naming. The Carpentries. Available at: https://datacarpentry.org/rr-organization1/01-file-naming/index.html (Accessed: January 24, 2023).](episodes/fig/globbing.jpeg){Shows files in a column with parts of the names that are the same or align}



##### ***Human readable***

Ensuring your file naming convention is human readable will depend on the context, background knowledge of research user(s), and character spaces availability. In short, use descriptive words. There will be examples of this further below.



##### ***Plays well with default ordering***


Default ordering is best achieved with numbers. This can be chronological i.e. date, or logical i.e. 01, 02, 03…

Depending on the research and your teams preference, a common word could prefix the numeric ordering system. For example:

lake01_depth.r
lake02_depth.r
lake03_depth.r
so on….

#### Benefits

If implemented early and consistently, a standardised system or convention for naming files can:

 - Make file naming easier

 - Facilitate access, retrieval and storage of files

 - Make it faster to navigate files

 - Guard against misplacing or losing files

 - Assist with version control

 - Identify obsolete or duplicate records

 - Avoid backlogs or project delays by presenting a clear and real-time display of the current or completed work.



### Metadata of your files

Are you collating photos, images, videos or other media? It is important to note information about each file alongside the files themselves.

The university of Chicago has [this useful guide to building a catalogue of information about your research images](https://vrc.uchicago.edu/guide-cataloging-your-images)

You could also look into a format such as [Dublin Core](https://en.wikipedia.org/wiki/Dublin_Core). Learn about [Dublin Core metadata basics](https://www.dublincore.org/resources/metadata-basics/).

Or you could use your own format, and cover simple metadata such as:

 - Publisher – "An entity responsible for making the resource available".

 - Rights – "Information about rights held in and over the resource, Copyright etc".

 - Source – "A related resource from which the described resource is derived. Where did this media come from?".

 - Subject – "The topic of the resource".

 - Title – "A name given to the resource".


## What is your next step?


::: tab 


### Beginner

A great place to start is:

 - Download a folder template and start using it!

 - Another idea is to put a copy of your raw data somewhere secure and backed up for safekeeping.

 - Come up with a plan on how you are going to name your files.

 - Check your folders are being backed up.


### Advanced

Your next move can be:


 - Ensure all your projects are well organised. This could extend to projects across your research group.

 - Educate others in your space on good naming conventions and build a reference guide to be used across your group.

 - Get a metadata file set up for your media.

 - If you are working in Python, you can use a [python package](https://github.com/vukovicnikola/templateproject) developed by researcher Nikola Vukovic to generate a logical, standardised, and flexible directory hierarchy for academic research.

:::




::::::::::::::::::::::::::::::::::::::::::::::: discussion

## Further Resources

[Project TIER](https://www.projecttier.org/tier-protocol/protocol-4-0/)

[File naming and folder structures by CESSDA](https://dmeg.cessda.eu/Data-Management-Expert-Guide/2.-Organise-Document/File-naming-and-folder-structure)

[Data Carpentry - Organization - File naming](https://datacarpentry.org/rr-organization1/01-file-naming/index.html)



:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::





::::::::::::::::::::::::::::::::::::::::::::::: callout

## References


TIER Protocol 4.0 | Project TIER | Teaching Integrity in Empirical Research. (n.d.). Www.projecttier.org. Retrieved April 16, 2024, from https://www.projecttier.org/tier-protocol/protocol-4-0/ licenced as CC-BY-NC


DCMI: Home. (2019). Dublincore.org. https://www.dublincore.org licenced under Creative Commons Attribution 4.0 International License 

Data Carpentry (2018) File Organization Retrieved on 2024-04-18 at https://datacarpentry.org/rr-organization1/01-file-naming/index.html licenced under CC BY 4.0 license.

:::::::::::::::::::::::::::::::
