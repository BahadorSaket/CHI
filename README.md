# Data and Task Based Effectiveness of Basic Visualizations
This repository contains all material for a crowdsourced study that evaluates the effectiveness of five basic visualization types (Table, Line Chart, Bar Chart, Scatterplot, and Pie Chart) across 10 different visual analysis tasks, three different data attributes (Nominal, Ordinal, Numerical), and two different datasets (Cars and Movies). 

###Visualizations used in our experiment
![screenshot 2016-10-03 11 21 01](https://cloud.githubusercontent.com/assets/22280917/19043418/0e698c86-895e-11e6-8fb9-5628a6ae0e81.png)

###Tasks used in our experiment

Below, we listed different types of questions we asked participants in our study. Our tasks are based on the low-level task taxonomy proposed by Amar et al[1]. 

####Retrieve Value.  
For this task, we asked participants to identify values of attributes for given data points. For example, what is the value of horsepower for the cars? 

####Filter. 
For given concrete conditions on data attribute values, we asked participants to find data points satisfying those conditions. For example, which car types have city miles per gallon
ranging from 25 to 56?

####Compute Derived Value. 
For a given set of data points, we asked participants to compute an aggregate value of those data points. For example, what is the sum of the budget for the action and the sci-fi movies?

####Find Extremum. 
For this task, we asked participants to find data points having an extreme value of an data attribute. For example, what is the car with highest cylinders?

####Sort. 
For a given set of data points, we asked participants to rank them according to a specific ordinal metric. For example, which of the following options contains the correct sequence of movie genres, if you were to put them in order from largest average gross value to lowest?

####Determine Range.
For a given set of data points and an attribute of interest, we asked participants to find the span of values within the set. For example, what is the range of car prices?

####Characterize Distribution. 
For a given set of data points and an attribute of interest, we asked participants to identify the distribution of that attribute values over the set. For example, what percentage of the movie genres have a average gross value higher than 10 million?

####Find Anomalies. 
We asked participants to identify any anomalies within a given set of data points with respect to a given relationship or expectation. We crafted these anomalies manually so that, once noticed, it would be straightforward to verify that the observed value was inconsistent with what would normally be present in the data (e.g., movies with zero or negative length would be considered abnormal). For example, which genre of movies appear to have abnormal length?

####Find Clusters. 
For a given a set of data points, we asked participants to find clusters of similar data attribute values. For example, how many different genres are shown in the chart below?

####Find Correlation. 
For a given set of two data attributes, we asked participants to determine if there is a correlation between them. To verify the responses to correlate tasks, we computed Pearson’s correlation coefficient (r) to ensure that there was an strong correlation (r ≤ −0.7 or r ≥ 0.7) between the two data attributes. For example, is there a strong correlation between average budget and movie rating?

###Datasets used in our experiment
In our experiment we used Cars and Movies datasets. Both datasets include data attributes of Nominal, Ordinal, and Numerical types. The Cars dataset provides details for 407 new cars and trucks for the year 2004. This dataset contains 18 data attributes describing each car. The Movies dataset provides details for 335 movies released from 2007 to 2012, and contains 13 data attributes.


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
benefit from such an engine are behavior-driven recommendation systems. Such systems often extract analytical tasks
from user interactions. These extracted tasks can be used as input to the engine for these systems to suggest more effective
visualizations. All these applications would also benefit from models trained on the results of the current study (or any
other empirical performance data) that can predict the task performance of “unseen" visualizations

Other Visualization of our results
![screenshot 2016-10-03 12 08 31](https://cloud.githubusercontent.com/assets/22280917/19044424/3a67f9f4-8962-11e6-8d7a-b2bb6bf28677.png)

![screenshot 2016-10-03 12 08 00](https://cloud.githubusercontent.com/assets/22280917/19044427/3d152eba-8962-11e6-87e7-7e67886d1be3.png)



### References
[1]. Robert Amar, James Eagan, and John Stasko. 2005. Low-level components of analytic activity in information visualization. In Information Visualization, 2005. INFOVIS 2005. IEEE Symposium on. IEEE, 111–117.
