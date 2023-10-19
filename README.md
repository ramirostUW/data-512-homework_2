# Data 512 Aut 2023 HW 2 :  Considering Bias in Data

## What Is This?

This repository contains my work for the second Homework Assignment of Data 512, which I am taking in Autumn of 2023 and the University of Washington. This assignment is about considering the biases a dataset may have, especially as it pertains to including or excluding representation of various subsets that would fall into it.

The sample project we are to work on for this assignment involves looking at Wikipedia articles on American cities and towns, and their quality as evaluated by ORES, a model trained on user-made article quality evaluations that tries to produce similar scores to what Wikipedia users may decide on when evaluating an article's quality. The four Jupyter Notebooks in this repository contain code and documentation on my work for this assignment, and the fourth one in particular contains tables that the “Research Implications” section of this ReadMe relies on for considering what was found in the dataset. 

## About this repo/How to use

### Provided files 

The word document in the root directory of this repository contains the directions I was given to complete this assignment. It is not needed for the code to work, and is only provided to give complete context. The are three tabular data files (two Excel and one CSV) file that the Steps 1 and 3 Notebooks take as input and come from external sources. All three are linked to from the Word Document, and are in the "input" folder of this repository. 

### My Work

The code I wrote is all in Python, and is in the three Jupyter Notebooks in the root directory of this repo. They are meant to be executed in the order described by their names (Step 1 first, then Step 2, then Step 3, then Step 4). Steps 1 and 2 each produce one subdirectory of the raw_api_data directory, by querying the PageInfo and ORES APIs respectively for data on each article about an American city. Step 3 produces the CSV in the refined_data directory, which condenses all of the data in the input tables and API JSONs into one file. Step 4 uses the refined dataset to produce a series of tables that give insight into the dataset's biases, which are finally then further explored in the "Research Implications" section of this ReadMe. The Steps 2-4 notebooks each rely on the files produced by the previous notebook, and Steps 1 and 3 are also dependent on the files in each input folder. All of the files that are produced by each Notebook are present in this repository. 

## Permissions and Licensing

This project, in Step 1 and Step 2, uses code made by my instructor for DATA 512 under  Creative Commons license. All original code is made available to to you under the terms described in the LICENSE file of this repository. 

## Research Implications 

The tables produced in Step 4 clearly show that there are biases in which regions of the United States, and their cities, receive the most attention on Wikipedia, with several states and region receiving disproportionately large amounts of attention. My responses to the below questions help illustrate my findings. 

** 1.  What biases did you expect to find in the data (before you started working with it), and why? **

A: I expected the data to illustrate less attention towards central U.S. regions, due to the tendency of some Americans to refer to them as flyover states, and for more rural, smaller states to also be even more underepresented. This ended up not being true; several central regional divisions, such as West North Central U.S., received higher proportions of overall articles and high quality articles, and several smaller states like Vermont and Wyoming also had a proportionally high amount of attention. 

** 2.  What (potential) sources of bias did you discover in the course of your data processing and analysis?**

A: In addition to my previous response, which includes information areas I found to have high representation, I found that the Western and (esepcially) Southern parts of the U.S. seem to have had a lack of representation on Wikipedia. The Pacific regional division was quite low on both its proportion of overall and high quality articles per capita compared to the other divisions, as was the South Atlantic division. Several southern states, like North Carolina and Nevada, also had disproportionately low rates of representation. 

** 3.  How might a researcher supplement or transform this dataset to potentially correct for the limitations/biases you observed? **

A: There's still several aspects of the dataset to be explored. One avenue other researches might want to take is to analyze whether bias on this dataset might have more to do with states having a few central cities rather than a larger amount of smaller ones, which might produce a low amount of articles relative to state population. Incorporating individual city populations into this analysis might be an exciting next step. 