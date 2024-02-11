**Problem Statement**

In the telecom industry, customers are able to choose from multiple service providers and actively switch from one operator to another. In this highly competitive market, the telecommunications industry experiences an average of 15-25% annual churn rate. Given the fact that it costs 5-10 times more to acquire a new customer than to retain an existing one, customer retention has now become even more important than customer acquisition.

For many incumbent operators, retaining high profitable customers is the number one business goal.

To reduce customer churn, telecom companies need to predict which customers are at high risk of churn.

In this project, you will analyse customer-level data of a leading telecom firm, build predictive models to identify customers at high risk of churn and identify the main indicators of churn.



**Definitions of churn**

There are various ways to define churn, such as:

- Revenue-based churn: Customers who have not utilised any revenue-generating facilities such as mobile internet, outgoing calls, SMS etc. over a given period of time. One could also use aggregate metrics such as ‘customers who have generated less than INR 4 per month in total/average/median revenue’.
The main shortcoming of this definition is that there are customers who only receive calls/SMSes from their wage-earning counterparts, i.e. they don’t generate revenue but use the services. For example, many users in rural areas only receive calls from their wage-earning siblings in urban areas.

- Usage-based churn: Customers who have not done any usage, either incoming or outgoing - in terms of calls, internet etc. over a period of time.
A potential shortcoming of this definition is that when the customer has stopped using the services for a while, it may be too late to take any corrective actions to retain them. For e.g., if you define churn based on a ‘two-months zero usage’ period, predicting churn could be useless since by that time the customer would have already switched to another operator.

 


**High-value churn**

In this project, you will define high-value customers based on a certain metric (mentioned later below) and predict churn only on high-value customers.

**Understanding the business objective and the data**

The dataset contains customer-level information for a span of three consecutive months - June, July, August. The months are encoded as 6, 7, 8  respectively. 
The objective is to identify the high valued customer churn 




The data dictionary contains meanings of abbreviations. Some frequent ones are loc (local), IC (incoming), OG (outgoing), T2T (telecom operator to telecom operator), T2O (telecom operator to another operator), RECH (recharge) etc.

The attributes containing 6, 7, 8 as suffixes imply that those correspond to the months 6, 7, 8 respectively.

**Steps**
1. Reading the data set
2. Understanding the data set
3. Dropping columns which are of not much use for analysis
4. Missing value imputation
5. Identifying the high valye customers
6. Perform EDA to understand the influence of predictor variables on the target variable
7. Handling the data imbalance using SMOTE
8. Logistic regression, Decision tree, Random forest, XGBoost for getting the feature importance and prediction
9. Using PCA building the models Logistic regression, Decision tree, Random forest, XGBoost targetting Accuracy, Recall, Precision
10. Model evaluation and Prediction using the best model


**Conclusion**

### Decrease in Total data recharge amount and Maximum recharge amount in month 8 is a strong indicator of churn.

### Decrease in incoming and outgoing minutes of usage in month 8 shows high churn probability.

### Decrease in local and roaming minutes of usage in month 8 shows high churn probability

### Decrease in ARPU in month 8 shown high churn probability

### New customers tend to churn easily.

### Random Forest produced the best prediction scores(among logistic regression, Decision tree and Random forest)