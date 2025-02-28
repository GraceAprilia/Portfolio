# Portfolio
Hi! I'm Grace, a recent graduate majoring in Mathematics with an interest at data analytics and machine learning. I have developed skills in programming languages such as Python. During my studies I learnt how to clean, process, train, and visualize data with Python to anlyze and idenify trends or patterns. Furthermore, I joined Bangkit, a Google-led academy designed to produce high-caliber tech talents, to gained knowledge about machine learning such as Neural Network, Natural Language Processing (NLP), and Convolutional Neural Network (CNN). More Recently, I independently learned Excel to clean, manage, and manipulate data. In my free time, I try to improve my skills and knowledge by watching free courses. 

I'm seeking opportunities in data analysis, data science, and machine learning. Skilled in both collaborative teamwork and independent work, I adapt seamlessly to diverse work environments. This portfolio highlights my skills and showcases the projects I have completed.

## Table of Contents
* [Project 1: Time Series Forecasting With Long Short-term Memory Multi Period Using Transfer Learning](https://github.com/GraceAprilia/Portofolio/edit/main/README.md#project-1-time-series-forecasting-with-long-short-term-memory-multi-period-using-transfer-learning)

## Project 1: Time Series Forecasting With Long Short-term Memory Multi Period Using Transfer Learning
This is a project I completed for my bachelor's degree, where I built LSTM model to predict the stock price of Ultrajaya Milk Industry & Trading Co PT (ULTJ) using transfer learning. In this project, I did two approaches: predicting ULTJ stock with and without transfer learning. Both approaches were used to compare the prediction results of the multi-period LSTM model for the stock price of ULTJ with and without transfer learning. 

#### Dataset & Tools
All stock data in this project are gathered from [yahoo finance](https://finance.yahoo.com). The data used include a 5-year period of adjusted close stock price from 14 March 2019 to 14 March 2024. All process from data cleaning, processing, training, to visualization are done by using Python.

### First Approach: Predicting ULTJ stock data without transfer Learning
In the first approach I use ULTJ stock data with the input data of 40 days to predict the next 20 days.
#### Data Cleaning and Processing 
In this proces, I performed the following tasks:
1. Remove N/A values
2. Formating data
3. Split the data into training and testing sets (70% training and 30% testing)
4. Convert the data into supervised data (40 input data and 20 target data)

### Training
The processed data are trained using this LSTM model with architecture:
| Layers        | Neurons |
| ------------- | -------:|
| LSTM      | 128 |
| Dense     |   32 |
| Dense     |    20 |




