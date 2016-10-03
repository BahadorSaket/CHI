# Data and Task Based Effectiveness of Basic Visualizations
This repository contains all material for a crowdsourced study that evaluates the effectiveness of five basic visualization types (Table, Line Chart, Bar Chart, Scatterplot, and Pie Chart) across 10 different visual analysis tasks [1], three different data attributes (Nominal, Ordinal, Numerical), and two different datasets (Cars and Movies). 

![screenshot 2016-10-03 11 21 01](https://cloud.githubusercontent.com/assets/22280917/19043418/0e698c86-895e-11e6-8fb9-5628a6ae0e81.png)


## How to use the data and source code in this repository?

###Experiment-Software

This folder contains all the files for our online experiment. In order to run the code, you need to run a local web server and view the page. 

How to run a local web server?

   Step 1: install python

   Step 2: Run python -m SimpleHTTPServer 8000

   Step 3: Open http://localhost:8000/index.html using any web browser.
   
###Raw-Data

This folder contians data collected from the experiment. All files are in the .xls format. In order to open each of them you need to have microsoft office Excel. If not you can just open them using Google sheet.


###SPSS-Analysis

This folder contains all the analysis we ran to make sense of our data. If you have SPSS installed on your machine you can check the raw data using SPSS as well. We also provided results of the spss in pdf format. You should be able to read the results without requiring SPSS on your machine. 


## What is it useful for?
we believe results of our study has at least two important applications. First, our results can be used as series of theoretical guidelines to inform visualization de- signers and those new to data visualization. Second, as there is an increasing trend in automating the process of visualization design using visualization recommender systems, these results can be applied to advance processes of generating, filtering, and pruning the recommendations. 

An important avenue for continued research is creating a recommendation engine that incorporates the findings of this
study. In particular, we plan to design an engine that takes into account performance time, accuracy, and user preferences when suggesting visualizations. Once we have such an engine, we can use it to develop new visualization recommendation
systems based on user-specified tasks and data attributes. One relevant application area of such a recommendation engine
can be natural language interfaces for data visualization. In such interfaces people tend to specify tasks as a part of their
questions (e.g., “Is there a correlation between price and width of cars in this dataset?”). The engine can be used to leverage this knowledge to suggest more effective visualizations for the given query. Another category of systems that might
benefit from such an engine are behavior-driven recommendation systems [25]. Such systems often extract analytical tasks
from user interactions. These extracted tasks can be used as input to the engine for these systems to suggest more effective
visualizations. All these applications would also benefit from models trained on the results of the current study (or any
other empirical performance data) that can predict the task performance of “unseen" visualizations

Other Visualization of our results

![condense](https://cloud.githubusercontent.com/assets/22280917/19042473/3670bd3e-895a-11e6-8d71-a65a7605bf13.jpg)


### References
[1]. Robert Amar, James Eagan, and John Stasko. 2005. Low-level components of analytic activity in information visualization. In Information Visualization, 2005. INFOVIS 2005. IEEE Symposium on. IEEE, 111–117.
