# Amazon_Vine_Analysis
## Overview
Big Market, a start-up that helps businesses to optimize their marketing effort, has hired me as their first data expert. One of the Big Markets clients, SellBy has requested hefty analytics for their products compared with their competitor products. Upon completing the SellBy project successfully, I have been tasked with another large project. The project is to analyze the Amazon reviews written by members of the paid Amazon vine program. The Amazon vine program is a service that allows manufacturers and publishers to receive reviews for their products. In this project, we have been given access to approximately 50 datasets. To perform the analysis, we choose the “Mobile Apps” dataset from the given datasets. Using PySpark, an ETL process is performed to extract the Mobile App dataset, transform the data, connect it to an AWS RDS instance, and load the transformed data into pgAdmin to calculate different metrics. PySpark has been used to determine if there is any bias towards favorable reviews from vine members in the dataset.

## Results
### Number of Vine and non-Vine Reviews
- There is zero number of vine reviews in the Mobile App dataset.
![image](https://user-images.githubusercontent.com/76491891/121807996-9673ea00-cc24-11eb-9714-d48ea2679b30.png)
