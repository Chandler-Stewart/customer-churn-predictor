# Customer Churn Prediction

This project focuses on an end-to-end project of exploring data and creating a binary classifier to .

We have information on over 7000 fake users that have either phone contracts, internet contracts, or contracts that have both a phone plan and an internet plan. We also have information about what is included in those contracts, how the contracts are formatted, and information on the customer demographics.

## What to know about this project:

**The Aim** - The goal of this project is to create a model designed to predict whether or not customers will decide to cancel their contracts based on a sample of a telecom company's current and past customers. AUC-ROC is the applicable metric to aim for, and this project wanted to achieve a score $\ge$ 0.88.

Strategies include:
- Delete duplicate data
- Feature engineering
- Exploratory Data Analysis
- Gradient Boosting model creation
- AUC-Roc evaluation

**The Data** - The data files below is where our input for the project comes from. The files contain different non-identifying information on people associated with their phone and internet contracts. The following characteristics are in the file:

The `contract` table - contract information  
The `internet` table - the client's personal data  
The `personal` table - information about Internet services  
The `phone` table - information about telephone services

The `contract` table:  
`customerID`: unique user identifier  
`BeginDate`: The date that the contract was started  
`EndDate`: The date that the contract was terminated (if applicable)  
`Type`: type of contract (month-to-month, 1 year, or 2 year)  
`PaperlessBilling`: whether the customer has opted for paperless billing  
`PaymentMethod`: Means of payment for the contract  
`MonthlyCharges`: typical monthly charge amount  
`TotalCharges`: Totale charge since the start of billing  

The `internet` table:  
`customerID`: unique user identifier  
`InternetService`: The type of internet service (DSL or Fiber optic)  
`OnlineSecurity`: If online security is included in the internet contract  
`OnlineBackup`: If online backup is included in the internet contract  
`DeviceProtection`: If device protection is included in the internet contract  
`TechSupport`: If tech support is included in the internet contract  
`StreamingTV`: If TV streaming is included in the internet contract  
`StreamingMovies`: If movie streaming is included in the internet contract  

The `personal` table:  
`customerID`: unique user identifier  
`gender`: Whether the customer was male or female  
`SeniorCitizen`: If the customer is a senior citizen  
`Partner`: If the customer has a spouse  
`Dependents`: If the customer has any dependents  

The `phone` table:  
`customerID`: unique user identifier  
`MultipleLines`: If multiple lines are included in the phone plans  
