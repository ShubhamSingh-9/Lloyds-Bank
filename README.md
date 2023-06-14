![image](https://github.com/ShubhamSingh-9/Lloyds-Bank/assets/111279439/238c0e57-fbbe-4fac-b95e-398a58aaaafd)

Lloyds Bank StepUp Challenge

Task 01: Data Strategy – Customer Profiling

1) Data Loading: The input data contained columns such as Customer ID, Annual Income, Interest Rate, Tenure of EMI, Ownership Type of the house, and Loan Status (whether they paid the loan or defaulted).
2) Handling Missing Values: The missing values in the data were imputed based on the data type. For numerical features like Annual Income and Interest Rate, the missing values were replaced with the mean of the respective columns. For categorical features like Ownership Type, the missing values were replaced with the mode.
3) Outlier Detection: Outliers were identified using the Interquartile Range (IQR) method. The data points lying outside the range of 1.5 times the IQR were considered outliers and removed from the dataset. This step helps in removing extreme values that might affect the model's performance.
4) Skewed Data Transformation: The Loan Amount and Annual Income columns were observed to be skewed. To make the data more suitable for modeling, a log transformation was applied to these columns. This transformation helps in reducing the skewness and approximating the data to a Gaussian distribution, which is commonly assumed by many machine learning algorithms.
5) Data Visualization: Graphs and plots were created to gain insights from the data. A box plot was used to visualize the Loan Status column with respect to other variables. It was observed that customers with higher annual income were more likely to repay their loans on time. Additionally, customers with lower interest rates had a higher repayment rate compared to those with higher interest rates.

By performing these steps of data preprocessing and visualization, valuable insights were gained regarding the relationship between customer attributes and loan repayment behavior. These insights can be further utilized for customer segmentation, risk assessment, and developing targeted strategies for loan management.
