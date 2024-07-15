# Porter-Delivery-Time-Estimation
Capstone Project for delivery time prediction 
In this article, we cover the construction of a model to predict the relationship between order information and delivery time using
the Porter Delivery Time Estimation dataset. To accomplish this, we employed two approaches.
Firstly, we opted for a regression model to predict the continuous target variable (delivery time).
Secondly, we chose a classification model to predict the categorical target variable (fast, moderate, slightly slow, slow) after
converting it.
In this article, we will cover the second approach, which involves handling the Porter Delivery Time Estimation dataset using a
classification model.
To achieve this, we created a new target variable for delivery time ("How_Long") by utilizing "created_at" and
"actual_delivery_time" and established the following criteria to convert this variable into categorical data.
1 to 30 minutes: Fast
30 to 60 minutes: Average.
60 to 90 minutes: Slightly Slow.
More than 90 minutes: Slow.
By categorically transforming the target variable in this manner, a classification model was constructed. This Model is expected to
provide customers with intuitive delivery time information for new orders and contribute to efficiently managing the delivery
process.
1.1 Objective:
Porter has a number of delivery partners available for delivering the food, from various restaurants and wants to get an estimated
delivery time that it can provide the customers on the basis of what they are ordering, from where and also the delivery partners.
