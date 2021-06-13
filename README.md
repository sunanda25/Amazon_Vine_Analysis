# Amazon_Vine_Analysis
## Overview
Big Market, a start-up that helps businesses to optimize their marketing effort, has hired me as their first data expert. One of the Big Markets clients, SellBy has requested hefty analytics for their products compared with their competitor products. Upon completing the SellBy project successfully, I have been tasked with another large project. The project is to analyze the Amazon reviews written by members of the paid Amazon vine program. The Amazon vine program is a service that allows manufacturers and publishers to receive reviews for their products. In this project, we have been given access to approximately 50 datasets. To perform the analysis, we choose the “Mobile Apps” dataset from the given datasets. Using PySpark, an ETL process is performed to extract the Mobile App dataset, transform the data, connect it to an AWS RDS instance, and load the transformed data into pgAdmin to calculate different metrics. PySpark has been used to determine if there is any bias towards favorable reviews from vine members in the dataset.

## Results
### Number of Vine and non-Vine Reviews
- There is zero number of vine reviews in the Mobile App dataset.
![image](https://user-images.githubusercontent.com/76491891/121807996-9673ea00-cc24-11eb-9714-d48ea2679b30.png)

- There are 129,516 non-vine reviews in the Mobile App dataset.
![image](https://user-images.githubusercontent.com/76491891/121808051-d76bfe80-cc24-11eb-931c-db95c9e6a077.png)

### Number of 5-Star Vine and non-Vine Reviews
- There are zero 5-star vine reviews in the Mobile App dataset.
![image](https://user-images.githubusercontent.com/76491891/121808127-231ea800-cc25-11eb-98ab-92b6915b49eb.png)

- There are 59,278 5-star non-vine reviews in the Mobile App dataset.
![image](https://user-images.githubusercontent.com/76491891/121808247-8c9eb680-cc25-11eb-86c0-b3ae99d7e536.png)

### Percentage of 5-Star Vine and non-Vine Reviews
- The percentage of 5-star vine reviews is calculated as (number of 5-star reviews) / (the total number of vine reviews) *100.  The number of vine reviews in the Mobile App dataset is zero, which results in ZeroDivisionError.  To resolve this error, try and except blocks were used.
![image](https://user-images.githubusercontent.com/76491891/121808310-d25b7f00-cc25-11eb-85ef-3f68bce3a45c.png)

- 45.76% of non-vine reviews are 5-star in the Mobile App dataset.
![image](https://user-images.githubusercontent.com/76491891/121808350-fd45d300-cc25-11eb-82b2-db1715ea820e.png)

## Summary
- The percentage of 5-star vine reviews is 0, whereas the percentage of 5-star non-vine reviews is 45.76%. This shows there is no positivity bias in the vine program.
- Additional analysis can be performed on the Mobile App dataset by calculating the mean, median, and mode for all star ratings.
