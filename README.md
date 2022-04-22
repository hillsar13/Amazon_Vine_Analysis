# Amazon_Vine_Analysis

## Purpose
In this project, we were tasked with analyzing Amazon reviews written by members of the paid Amazon Vine program. We needed to pick one of the available datasets (Video Games) and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. We then used PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in the dataset.

## Results
- Total Paid Vine Reviews : The Total Paid Vine Reviews had a significantly smaller total participation size (94 Total, 48 - 5 Star Reviews, 51% 5 Star Rating)

<img width="577" alt="Screen Shot 2022-04-21 at 8 16 47 PM" src="https://user-images.githubusercontent.com/95551195/164583227-00935e06-9f9c-40f0-b4a0-b89b5ec64fbf.png">

- Total Unpaid Vine Reviews: The Total UnPaid Vine Reviews had a significnatly larger total participation size (40471 Total, 15663 - 5 Star Reviews, 38% 5 Star Rating)

<img width="550" alt="Screen Shot 2022-04-21 at 8 17 40 PM" src="https://user-images.githubusercontent.com/95551195/164583327-aadb6c65-cff8-494c-85d5-9c86c92c656e.png">

## Summary
On initial look, it would appear that the total paid reviews show over a 51% percentage - an encouraging number! However, after looking closely at the numerics, it would appear that the Paid Vine Review is suffering from a small sample bias. Looking at the Total Unpaid Vine Reviews - it is clear quickly that there is a much large sample size reporting fewer 5 star ratings than the Paid. In order to make a proper comparison, it is recommended to complete anlayses on two similarly sized samples to see if there is a true differentiation between Paid & Unpaid (random sample selected to avoid cherry picking bias on the Unpaid Reviews). 
