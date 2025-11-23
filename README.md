# diwali-returns-prediction-2025
This project analyzes Diwali sales data for 2025 to understand customer buying patterns and return behavior.

**Dataset**
https://www.kaggle.com/datasets/anandshaw2001/amazon-product-sales-2025

**How to Run**

1.Download the dataset from the link above

2.Place the CSV file in the same folder as the notebook

3.Open the notebook (.ipynb)

4.Run all cells one by one — no extra setup required

**Project Goal**

To predict whether an order will be Delivered or Returned, and to understand whether customer sentiment (Positive / Neutral / Negative) affects the return rate.

Steps Performed

1.Loaded and explored the dataset (EDA)

2.Created a new column Return_Flag — 1 for Returned, 0 for Delivered

3.Selected features for prediction:

    1)Quantity

    2)Unit Price

    3)Total Sales

    4)Product Category

    5)Payment Method

4.One-hot encoded categorical columns

5.Trained ML models to predict return status

6.Converted review ratings into sentiment (Positive / Neutral / Negative)

7.Compared return rates across sentiment categories

**Why Logistic Regression Performed Best**

 To improve the prediction performance, I also tested Random Forest and XGBoost along with Logistic Regression. The Random Forest model reached an accuracy of about 0.5060, and XGBoost achieved around 0.5025, but both showed very minimal improvement and required more tuning. Logistic Regression performed slightly better with an accuracy of 0.5120, and because it is simple, stable, and easy to explain, I chose it as the final model for this project.

**Conclusion**

Even though the sentiment of customers was mostly positive, many high-rated products were still returned.
This shows that returns are not always due to dissatisfaction — factors like size, product mismatch, delivery issues, or late expectations may also play a major role.
