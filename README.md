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
3. Normalize data (using min-max normalization)
4. Split the data into training and testing sets (70% training and 30% testing)
5. Convert the data into supervised data (40 input data and 20 target data)

### Training
The processed data are trained using 40 epoch with ADAM optimizer and MSE loss function. The architecture model are as below:
| Layers    | Neurons |
| ----------| -------:|
| LSTM      | 128 |
| Dense     |   32 |
| Dense     |    20 |

### Prediction
Images below are the result of ULTJ stock prediction with (a) first iteration, (b) second iteration, (c) third iteration, and (d) fourth iteration. The prediction results from four iterations of ULTJ stock data produced an average MAPE value of 10.219%.
![Screenshot 2025-03-01 163759](https://github.com/user-attachments/assets/1cf96197-b325-4511-8758-3d1f69167791)
![Screenshot 2025-03-01 163937](https://github.com/user-attachments/assets/7865a0cb-1447-48d7-ab21-bfd2a768b83d)

### Second Approach: Predicting ULTJ stock data without transfer Learning

In this approach the ULTJ stock data will be predicted using transfer learning. In this approach, the data cleaning and processing steps remain unchanged. Two models are used: the first model is trained on 20 stock data, and its weights and biases are transferred to the second model, which is then trained on ULTJ stock data to predict ULTJ stock prices.

#### First Model Architechture
This model is trained using 20 stock data with various trends.

| Layers    | Neurons |
| ----------| -------:|
| LSTM      | 256 |
| LSTM      | 128 |
| Dense     |   64 |
| Dense     |    20 |

#### Second Model Architechture
This model are used to predict ULTJ stock data using the weight and biases gained in the first model. 

| Layers    | Neurons |
| ----------| -------:|
| Taken from the fist layer of the first model|256|
| LSTM      | 128 |
| Taken from the third layer of the first model|64|
| Dense     |    32 |
| Dense     |    20 |

### Prediction
Images below are the result of ULTJ stock prediction with transfer learning whereas (a) first iteration, (b) second iteration, (c) third iteration, and (d) fourth iteration. The prediction results from four iterations of ULTJ stock data with transfer learning produced an average MAPE value of 7.599%.
![Screenshot 2025-03-01 180117](https://github.com/user-attachments/assets/63addc48-f6f7-4082-9f6c-657c9f96ece4)
![Screenshot 2025-03-01 180215](https://github.com/user-attachments/assets/80c19fd4-317d-4b61-b1c5-ec1e38a2f36e)



