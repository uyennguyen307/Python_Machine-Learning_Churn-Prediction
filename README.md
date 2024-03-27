# Introduction
## 1. Business Question
One e-commerce company has a project on predicting churned users to offer potential promotions. The attached file is the dataset that is offered by the company (churn_predict.csv). Using these datasets to answer the below questions:
1. What are the patterns/behavior of churned users? What are your suggestions to the company to reduce churned users?
2. Build the Machine Learning model for predicting churned users.

## 2. About Churn-Prediction
Churn prediction means detecting which customers are likely to leave a service or cancel a subscription to a service. Churn prediction modeling techniques attempt to understand the precise customer behaviors and attributes that signal the risk and timing of customers leaving

**Reference:**  https://www.avaus.com/blog/predicting-customer-churn/

## 3. About Machine Learning - Supervised Learning
Supervised learning is a category of machine learning that uses labeled datasets to train algorithms to predict outcomes and recognize patterns.

**Reference:** (https://cloud.google.com/discover/what-is-supervised-learning#:)

## 4. Dataset
![image](https://github.com/uyennguyen307/uyennguyen307-Python_Machine-Learning_Churn-Prediction/assets/162019618/f6047b1f-7637-4dd4-91c0-e8720b0cdb1c)

Replace the missing value with 0 or the median 

#### Check imbalanced data 

![image](https://github.com/uyennguyen307/uyennguyen307-Python_Machine-Learning_Churn-Prediction/assets/162019618/41e059ca-ad68-44cf-bddf-373458e97b30)

% data labeled 1 on total data is 16.9%, it's quite imbalanced => process Machine Learning model as normal, after processing, if model ko như expect, enhance data labeled 1 on total data rate or input more data

## Business Question Solving

Apply the Exploratory Data Analysis (EDA) method to detect the patterns/behavior of churned users and pick impactful fields for the Machine Learning Model
![image](https://github.com/uyennguyen307/uyennguyen307-Python_Machine-Learning_Churn-Prediction/assets/162019618/58771619-1068-4456-8c56-6e8ff6126074)

#### Tenure fields
![image](https://github.com/uyennguyen307/uyennguyen307-Python_Machine-Learning_Churn-Prediction/assets/162019618/1211975a-90b5-42e9-9e3b-4248ac91d4dc)
![image](https://github.com/uyennguyen307/uyennguyen307-Python_Machine-Learning_Churn-Prediction/assets/162019618/1a9c76ec-06c7-46e1-8c4b-d15cad45b1dc)

#### Complain fields
![image](https://github.com/uyennguyen307/uyennguyen307-Python_Machine-Learning_Churn-Prediction/assets/162019618/4a1d7c95-f1c6-4bf3-b8ea-e9dd6831da6e)
![image](https://github.com/uyennguyen307/uyennguyen307-Python_Machine-Learning_Churn-Prediction/assets/162019618/2ace8160-2b2d-444f-870a-39ef9761679d)

#### Satisfaction Score
![image](https://github.com/uyennguyen307/uyennguyen307-Python_Machine-Learning_Churn-Prediction/assets/162019618/0d02ce93-7089-4eab-8d18-8111b17d7eb8)
![image](https://github.com/uyennguyen307/uyennguyen307-Python_Machine-Learning_Churn-Prediction/assets/162019618/7f233c9d-6bbe-4538-8f7d-58cb52c39c77)

#### Order Amount Hike from Last Year
![image](https://github.com/uyennguyen307/uyennguyen307-Python_Machine-Learning_Churn-Prediction/assets/162019618/a4fd0a22-2fc4-4bee-b302-32d61e67ff28)
![image](https://github.com/uyennguyen307/uyennguyen307-Python_Machine-Learning_Churn-Prediction/assets/162019618/e6ca0409-3625-4768-b15c-933d7866f029)

#### Number of Device Registered
![image](https://github.com/uyennguyen307/uyennguyen307-Python_Machine-Learning_Churn-Prediction/assets/162019618/394a2bf2-e5e3-4f09-b092-2f4d2d4d6c01)
![image](https://github.com/uyennguyen307/uyennguyen307-Python_Machine-Learning_Churn-Prediction/assets/162019618/280f3330-b226-4a93-8e54-95a89f80ccaf)

#### Prefered Order Category
![image](https://github.com/uyennguyen307/uyennguyen307-Python_Machine-Learning_Churn-Prediction/assets/162019618/020924d8-aea4-4c89-a141-4114835568de)
![image](https://github.com/uyennguyen307/uyennguyen307-Python_Machine-Learning_Churn-Prediction/assets/162019618/316aadff-3979-49b8-bc64-2f38d8fd969e)

#### Marital Status
![image](https://github.com/uyennguyen307/uyennguyen307-Python_Machine-Learning_Churn-Prediction/assets/162019618/2da5a337-ed6a-46f8-92fd-ddceef5d9e53)
![image](https://github.com/uyennguyen307/uyennguyen307-Python_Machine-Learning_Churn-Prediction/assets/162019618/54179c07-dd4d-465e-bfff-217ec97f6df7)

#### Cashback Amount
![image](https://github.com/uyennguyen307/uyennguyen307-Python_Machine-Learning_Churn-Prediction/assets/162019618/d1d374a1-8e81-44da-9634-2a53a3d1a50c)

### 1. What are the patterns/behaviors of churned users? What are your suggestions to the company to reduce churned users?
#### The behavior of churned users
- The new customers who have transactions after creating an account 0-1 day have been ability to churn
- People who have a complaint
- Customers who buy mobile phones tend to churn
- The higher the City Tier, the lower the churn level
- The more accounts a customer registers, the more likely it is to churn
- The closer the customer's last order date gets, the higher the churn rate
- Single people are more likely to churn than married status
- The less cashback customers receive, the higher the churn rate

#### There are some solutions

- Sending emails, reminding customers about upcoming promotions and offering special discounts to new customers
- Building a complaint-handling process, receiving, find the cause and resolving complaints
- With people who complained => Reaching out to them to get their feedback, identify and analyze common complaints, fix underlying problems and offer solutions as well as offer them voucher
- Offer customers other products for cross-selling or up sell customer



