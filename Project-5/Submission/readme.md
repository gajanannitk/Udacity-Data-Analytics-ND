# Titanic Dataset - Exploration and Visualizations
## by Sayan Chakraborty


## Dataset
Data source is Kaggle: https://www.kaggle.com/c/titanic/data.  
It contains 891 values and 12 columns which are as follows:  

`PassengerId      int64`   
`Survived         int64`  
`Pclass           int64`  
`Sex             object` 
`Age            float64`  
`SibSp            int64`  
`Parch            int64`  
`Fare           float64`  
`Embarked        object`  

## Summary of Findings
This analysis will contain an analysis of the tragic titanic event of 1912. The whole dataset is divided into 2 parts. The training and testing data. In general these are data for building a machine learning model. But in my case I will be doing a visualization of the analysis to come up with some idea on the tragic event without applying any regression models or any ML algorithms to do any kind of predictive analysis, since that is out of scope right now.  

> To summarize my findings from the univariate analysis:  
- There were more number of survivers than the ones who couldn't. To be more specific: around 38% of the people were unfortunate enough to not make it through.  
- There were more people in the general class (class 3) than that of the other passenger classes.
- There were more male passengers than females.
- There were more passengers with 0 sibligs/spouses on-board.
- There were more passengers with 0 parents on-board.
- Most of the passengers onboarded from Southampton.
- The fares distribution is mostly right skewed. Most of the people were paying around 8.05 bucks. There were 43 such fare counts. 
- The age is somewhat normally distributed with slight deviations as seen from the kde distribution below. Most of the people are aged between 25-40.  

> To summarize my findings from the bivariate analysis:  
- There were more number of survivers than the ones who couldn't. To be more specific: around 38% of the people were unfortunate enough to not make it through.  
- People belonging to passenger class 1 were basically more lucky than the lower tier ones.
- There were more females who survived that the males.
- Passengers with 1-2 sibligs seemed to be more lucky
- Passengers with around 3 parents onboard had a greater survival chance
- It seems like people who were fortunate enough were on the age group of 0-80 with the IQR around 20-38.
- Other than that it seems like higher you paid, a slight higher were the chances of you surviving. For the people who survived the fares ranged from 0 to all the way 512. For the unfortunate ones the fares ranged from 0 to around 290.  

> Finally to summarize from the final multivariate analysis:  

1. There is a positve coorelation between the fares and the number of people who survived.  
2. There is a negative coorelation between the passenger class and the number of people who surived.
3. There is a negative coorelation between the fares and the passenger class. 
4. There is also a negative coorelation between the ages and the passenger classes.



## Key Insights for Presentation

In this analysis I mainly try to find out what might be the factors which can be linked to a person losing their life in the tragic event. There were several factors which were some way or the other linked to survival. There were the passenger classes, there were fares for the seats, there were factors like relatives who onboarded with you. There were certain people who sufferred the most- there were more female survivers from the males, the age group of 25-40 sufferred the most and several other relations which I tried to capture as much as possible. In case of multivariate analysis though, since the relation metrics were not much. I thought only a coorelation heatmap would be sufficient to depict my finds and coorelations of each feature set with another. 
