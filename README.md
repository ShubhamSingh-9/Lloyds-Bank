<img src="lloyds-bank.png" alt="Banj Image" width="300" height="300" align="center">


![image](https://github.com/ShubhamSingh-9/Lloyds-Bank/assets/111279439/238c0e57-fbbe-4fac-b95e-398a58aaaafd)


Lloyds Bank StepUp Challenge

Task 01: Data Strategy – Customer Profiling

1) Data Loading: The input data contained columns such as Customer ID, Annual Income, Interest Rate, Tenure of EMI, Ownership Type of the house, and Loan Status (whether they paid the loan or defaulted).
2) Handling Missing Values: The missing values in the data were imputed based on the data type. For numerical features like Annual Income and Interest Rate, the missing values were replaced with the mean of the respective columns. For categorical features like Ownership Type, the missing values were replaced with the mode.
3) Outlier Detection: Outliers were identified using the Interquartile Range (IQR) method. The data points lying outside the range of 1.5 times the IQR were considered outliers and removed from the dataset. This step helps in removing extreme values that might affect the model's performance.
4) Skewed Data Transformation: The Loan Amount and Annual Income columns were observed to be skewed. To make the data more suitable for modeling, a log transformation was applied to these columns. This transformation helps in reducing the skewness and approximating the data to a Gaussian distribution, which is commonly assumed by many machine learning algorithms.
5) Data Visualization: Graphs and plots were created to gain insights from the data. A box plot was used to visualize the Loan Status column with respect to other variables. It was observed that customers with higher annual income were more likely to repay their loans on time. Additionally, customers with lower interest rates had a higher repayment rate compared to those with higher interest rates.

![image](https://github.com/ShubhamSingh-9/Lloyds-Bank/assets/111279439/b2b77076-a521-4f91-9329-161b2d81c29d)   ![image](https://github.com/ShubhamSingh-9/Lloyds-Bank/assets/111279439/5b8f42b2-d8a2-4254-afd4-b19f0b70e0f7)



By performing these steps of data preprocessing and visualization, valuable insights were gained regarding the relationship between customer attributes and loan repayment behavior. These insights can be further utilized for customer segmentation, risk assessment, and developing targeted strategies for loan management.

Task 02: Predictive Model Summary:

The goal of this task was to create a predictive model that can classify customers into two groups: those who will repay their loan amount in full and those who will default. 

The following steps were taken to achieve this goal:
1) Data Scaling: The StandardScaler class from the sklearn.preprocessing module was used to scale the input features. This step ensures that the data has a mean of zero and a standard deviation of one, which is required for some machine learning algorithms.
2) Categorical Data Encoding: The home_owner feature, which indicates whether the customer owns a home or not, was encoded using one-hot encoding. This technique transforms categorical variables into binary vectors, which can be used by the model. The first column of the encoded feature was dropped to avoid multicollinearity problems.
3) Feature Selection: Only a subset of features was used as input for the models. This step reduces the dimensionality of the data and focuses on the most important features. The pandas library was used to select the relevant features from the dataset.
4) Model Building: Three models from the sklearn library were used to build the predictive models: Random Forest, Decision Tree, and Gaussian NB. These models are suitable for classification tasks and can handle both numerical and categorical data.
5) Model Evaluation: The accuracy metric was used to measure the performance of the models. The accuracy is the ratio of correctly predicted instances to the total number of instances. The Random Forest model achieved the highest accuracy of about 79%, indicating that it was the best model for predicting loan repayment.

![image](https://github.com/ShubhamSingh-9/Lloyds-Bank/assets/111279439/43df5569-a427-46b0-a42f-65608f5a2a3f)


These steps resulted in a predictive model that can classify customers based on their loan repayment behavior. The Random Forest model showed the best performance with a high accuracy score, suggesting its usefulness for predicting loan repayment.
