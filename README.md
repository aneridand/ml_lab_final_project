# Machine Learning Lab Final Project

## About me
I am Aneri Dand, studying Masters in Data Science at the University of San Francisco. 

## Project Overview
This project is part of the MSDS 699 course at the University of San Francisco.
Here's the [Deepnote link](https://deepnote.com/project/ddc61a58-e71d-4541-81d3-ede4d6669fe3) to the project.

### Research Problem: 
To predict whether a hotel booking will be cancelled using current and prior booking information.  

### Why is this important?
Hotels get multiple bookings throughout the year and several of these bookings are cancelled. Cancelled bookings mean lost revenue for the business - if the management could predict whether a hotel booking is likely to get cancelled, it would be in their best interest to allocate the room to someone else and earn their business. This project aims to utilize curent and prior booking information in order to predict whether a hotel booking is likely to get cancelled.

### Data Source:
For this project, data has been sourced from [Kaggle](https://www.kaggle.com/jessemostipak/hotel-booking-demand)

### Overview of data:
The dataset contains several columns which inform about the hotel type, length of stay, number of adults/children staying, previous cancellations, deposit type, etc.  

### Findings:
In this project, I fit two models (Random Forest and Logistic Regression) on the training data. Using `RandomizedSearchCV` to cross validate and Balanced Accuracy Score, Precision, Recall and F1 scores as evaluation metrics, the Logistic Regression model fared better than the Random Forest model. While the balanced accuracy score of the random forest model was quite close to that of Logistic Regression, I believe the l2 penalty used for regularization in logistic regression resulted in model which was more general and avoided overfitting. When the logistic regression model was used on the test dataset, the precision, recall, and f1 scores were around 80% which indicated that the model did reasonably well on an unseen dataset. 

### Future directions:
By engineering more features, the number of days within which a booking is cancelled (if at all it is) can be predicted. This would enable the hotel management to devise their cancellation policies and aid in calculating cancellation fees. Real time weather data can also be used to improve model predictions.

