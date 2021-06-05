# Titanic dataset EDA and modelling

## Table of content
   1. [Problem Statement](#problem-statement)
   2. [Exploratory Data Analysis](#EDA)
   3. [Models](#Models)
   4. [Conclusion](#c)

##### Note:
** This is my first ever kaggle participation. If you are looking to get started with Kaggle competion please go over the notebook. I have covered each step from performing the EDA to creating submission file. **

<h2 id="problem-statement"> 1. Problem Statement (https://www.kaggle.com/c/titanic) : </h2>

The sinking of the Titanic is one of the most infamous shipwrecks in history.

On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1502 out of 2224 passengers and crew.

While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.

In this challenge, we need to build a predictive model that answers the question: “what sorts of people were more likely to survive?” using passenger data (ie name, age, gender, socio-economic class, etc).

<h2 id="EDA">2. Exploratory Data Analysis:  </h2>

### Importance of Data Visualization in Data Science

##### Before we proceed any further we need to understand why data visualization is important and why can't we just proceed with model development?

Well, since I created this repository specifically for EDA Analysis let me answer this here once for all. 

The very purpose of Data Science is understanding the data and using it to predict future outcomes. In order for us to be able to apply appropriate algorithms and futher develop Machine learning applications we need to understand the data first.
P.S- Because of Data Visualization I developed interest in data science :smiley:

#### Lets have a quick overview of EDA analysis and understand why the specific plots were applied.

##### 1. The very first thing we do is plot a count plot to visualise number of casualities and survivors.(we obviously cannot count the numbers from the CSV file and this is why we need data visualization plots)
![](https://github.com/aditi-01/Titanic-dataset-EDA-and-modelling/blob/master/images/Titanic1.JPG)


##### 2. Next we apply dist plots to gain an idea about distribution of passenger class of the total titanic voyagers. 
![](https://github.com/aditi-01/Titanic-dataset-EDA-and-modelling/blob/master/images/Titanic2.JPG)
It is apparent that most passengers were travelling 3rd class. 


##### 3. Next we apply count plot to visualise distribution of male and female over the entire Titanic population. 
![](https://github.com/aditi-01/Titanic-dataset-EDA-and-modelling/blob/master/images/Titanic3.JPG)


##### 4. Applied dist plot to undertand how many male and female survived. (Here we are performing Bivate Analysis)
![](https://github.com/aditi-01/Titanic-dataset-EDA-and-modelling/blob/master/images/Titanic4.JPG)


##### 5. Next we visualize number of siblings and spouses over the population with a count plot.
![](https://github.com/aditi-01/Titanic-dataset-EDA-and-modelling/blob/master/images/Titanic5.JPG)


##### 6. Next we perform a bivariate analysis and find out how many people survived vs the number of siblings and spouse they had. 
![](https://github.com/aditi-01/Titanic-dataset-EDA-and-modelling/blob/master/images/Titanic6.JPG)
we have an interesting inference that people who has more sibling and spouses had a better chance at survival.

##### 7. Next we perform a univariate analysis to visualize number of Children and parents aboard. 
![](https://github.com/aditi-01/Titanic-dataset-EDA-and-modelling/blob/master/images/Titanic8.JPG)


##### 8. We also did a bivariate analysis over number of survivors vs number of parents/ children aboard.
![](https://github.com/aditi-01/Titanic-dataset-EDA-and-modelling/blob/master/images/Titanic9.JPG)
We came to the inference that people with more children had a better chance of survival.(We have already seen this in the movie though)

##### 9. We also did a univariate analysis to visualize count of people with respect to ticket fare.

##### 10. Performed a bivariate analysis to visualise how survival can we linked with ticket fare.
(Whether people who paid more had better chance at survival etc)

##### 11. We applied a count plot over embarked column. 


<h2 id="Models"> 3. Models:  </h2>
We have applied following <b>ML Models</b>:
<ul>
<li> Logistic Regression</li> 
<li> K- Nearest Neighbours</li>
<li> Gaussian Naive Bayes</li>
<li> Linear SVC</li>
<li> Stochastic Gradient Descent</li>
<li> Decision Tree Classifier</li>
<li> Gradient Boosting Trees</li>
<li> Catboost model</li>
</ul>

####  Regular Accuracy score of all the applied models


#### Cross validation Accuracy score of all the models 


<h2 id="c"> 4. Conclusion: </h2><br>
From the EDA analysis we concluded that:-<br>
<ul>
<li>Females had the better chance at surviving than the males. </li>
<li>People with children, siblings and spouses had a better chance at survival than those who were travelling solo.</li>
</ul>


P.S- This project I specifically did to learn the implemention of Catboost algorithm. To understand EDA process in more detail head over to a different repository.




