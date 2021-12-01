# Project-4
Link to our site: http://cc-approval.herokuapp.com/


## **Overview** 👇
Due to COVID-19, many people have lost their jobs, resulting in some strapping for cash and defaulting on their credit card payments. Things have gotten so bad that credit card companies, such as JP Morgan and Citigroup have to set aside an additional reserve to cover their losses from credit card defaults. People’s inability to pay for their credit card bills could be due to different circumstances. However, when it’s deliberate, meaning that customers have no plans in paying the bank back, it would be considered fraud. Either way, this imposes a huge risk on the credit card companies and we need to find a way to flag possible offenders.


To address this issue, we created a machine learning model that can predict potential default accounts based on certain attributes. The idea is that the earlier the potential default accounts are detected, the lower the losses we will embrace. On the other hand, we can be proactive by providing tips to customers to prevent default. This not only protects our customers but also minimizes our risks and potential losses.

- Background
- Goal
- Technologies and Data Source
- Process
- Model Usage
- Data Preparation and Overview
- Machine Learning
- eature Selection
- Website
- Limitations
- Conclusion


## **Background** 💳
Applying for a credit card can be intimidating for some people. Many applications ask for your social security number and your credit may get hit with a hard inquiry. We wanted to use a machine learning model remove this friction.


## **Goal** 🏁
To predict whether a credit card applicant will be approved or denied.


## **Motivation** 💰
There are times when even a seemingly manageable debt, such as credit cards, goes out of control. Loss of job, medical crisis or business failure are some of the reasons that can impact your finances. In fact, credit card debts are usually the first to get out of hand in such situations due to hefty finance charges (compounded on daily balances) and other penalties.

A lot of us would be able to relate to this scenario. We may have missed credit card payments once or twice because of forgotten due dates or cash flow issues. But what happens when this continues for months? How to predict if a customer will be defaulter in next months?

To reduce the risk of Banks, this model has been developed to predict customer defaulter based on demographic data like gender, age, marital status and behavioral data like last payments, past transactions etc.



## **Technologies** 🔨

![image](https://img.shields.io/badge/technologies-Python-blue)
![image](https://img.shields.io/badge/technologies-Pandas-blue)
![image](https://img.shields.io/badge/technologies-SQL-blue)
![image](https://img.shields.io/badge/technologies-PostgreSQL-blue)
![image](https://img.shields.io/badge/technologies-Javascript-blue)
![image](https://img.shields.io/badge/technologies-Flask-blue)
![image](https://img.shields.io/badge/technologies-HTML-blue)
![image](https://img.shields.io/badge/technologies-CSS-blue)
![image](https://img.shields.io/badge/technologies-Bootstrap-blue)
![image](https://img.shields.io/badge/technologies-Machine_Learning-blue)
![image](https://img.shields.io/badge/technologies-SKLearn-blue)


## **Process** ⚙️

1. Data Cleaning
    - Removing extraneous columns
    - Null values
    - Duplicates
    - Merging datasets by grouping shows
2. Produced visualizations for a better understanding
3. Regularization: Coefficient plots with Linear Regression
4. Function to test the familiar Regressors
5. Scaling the data – StandScaler & MinMaxScaler
6. Model Selection & Prediction 
7. Exported the model -> Flask implementation
8. Heroku deployment

## **Archetictural Diagram** 🔧

This flow chart is a big picture view of how our website works. At the top, the data scientist transforms the data in SQL, and then uses jupyter notebook to scale the data and develop the model. The model is then saved into an open source Java Database, or a .H2 file, that is loaded to the server. The user the accesses the server, and our flask app then loads the model for use on the website.

[![Credit-Card-Predictor-Flowchart-Flowchart-3.png](https://i.postimg.cc/zfKwfPj9/Credit-Card-Predictor-Flowchart-Flowchart-3.png)](https://postimg.cc/065KWnhf)

## **Graphs** 📊
These graphs show the features that we used in selecting our machine learning model. Child count by household was a big determining factor in our model. This ranged from households with anywhere from zero children, all the way to one household with 19 children in our dataset.

[![Number-of-people-child-count.png](https://i.postimg.cc/fyVpQvN2/Number-of-people-child-count.png)](https://postimg.cc/H8CBQXjX)

This graph shows the total income distribution in our dataset. This total income of a household, and not necessarily income of a single person. The increments at the bottom are by $200k. In our dataset, the average household income is $186k and the median household income is $157k.

[![income-distribution.png](https://i.postimg.cc/gct1PnB1/income-distribution.png)](https://postimg.cc/Dmsxryhc)

Male vs female was also a major feature in our dataset and machine learning model. As you can see, a vast majority of our dataset is women, coming it at 67%.
[![male-vs-female.png](https://i.postimg.cc/Pr8VsKD8/male-vs-female.png)](https://postimg.cc/HVd9bwBp)

## **Website** 📰

Our website starts by asking you to fill out basic information such as Number of children, household income, family size, etc. Based on all of these inputs, our machine learning model then computes whether or not you're likely to be accepted for a new credit card.

![Alt Text](https://media.giphy.com/media/WAm5zjmtgwncqmGpf9/giphy.gif)

<img src="https://media.giphy.com/media/WAm5zjmtgwncqmGpf9/giphy.gif" height="700">

Our next page then shows the output result of our machine learning model, based on what the inputs were. The outcome will either say "The credit card application is likely to be DENIED*", or "The credit card application is likely to be APPROVED*". We put in the asterisk to let people know that this result is based on a machine learning model, and not always 100% accurate.




## **Contributors** 👨👨👨👩
- [Bradley Barker](https://github.com/brbbrb)
- [Cody Gardner](https://github.com/cgardner1388)
- [David Owens](https://github.com/dowens1186)
- [Marie Prosper](https://github.com/marieprosper77)