#  Online Retail Customer Analytics and Purchase Prediction

This project focuses on analyzing online retail data to uncover customer behavior, predict purchases, recommend products, segment customers, detect churn, and forecast sales. It uses various machine learning models and techniques to derive actionable insights that help improve customer engagement and sales strategies.

---

## Project Goals

1. **Customer Segmentation** using RFM analysis + K-Means.
2. **Purchase Prediction** using classification models.
3. **Product Recommendation** using Association Rule Mining (Apriori).
4. **Sales Forecasting** using regression models.
5. **Product Category Prediction** based on customer and transaction data.
6. **Churn Detection** to identify lost customers.

---

##  Dataset Description

The dataset consists of e-commerce transaction records with the following fields:

| Column Name         | Description                                                |
|---------------------|------------------------------------------------------------|
| `Transaction_ID`     | Unique identifier for each transaction                    |
| `Product_Code`       | Code associated with a product                            |
| `Product_Title`      | Name of the product                                       |
| `Units_Sold`         | Quantity of product units sold                            |
| `Unit_Cost`          | Cost per unit                                             |
| `Client_ID`          | Unique customer identifier                                |
| `Client_Region`      | Region of the customer                                    |
| `TotalPrice`         | Total amount spent in the transaction (Units × Cost)      |
| `Purchase`           | Whether the transaction resulted in a purchase (0 or 1)   |
| `Transaction_Index`  | Sequential ID used for tracking                           |

> Note: `Transaction_Timestamp` is not consistently available, so time-based tasks are handled using available substitutes where necessary.

---

##  Target Variables

- `Purchase` → Binary classification (purchase or not)
- `TotalPrice` → Regression target (sales forecasting)
- `Product_Title` → Multi-class classification (product category prediction)
- `Client_ID` → For segmentation and churn analysis

---

##  Features Implemented

| Feature               | Technique Used                    |
|-----------------------|------------------------------------|
| Customer Segmentation | RFM Analysis + K-Means Clustering |
| Purchase Prediction   | Random Forest Classifier          |
| Sales Forecasting     | Random Forest Regressor           |
| Product Recommendation| Apriori + Association Rules       |
| Product Prediction    | Random Forest Classifier          |
| Churn Detection       | Rule-based (based on inactivity)  |

---

## Libraries & Tools

- Python 3.x
- pandas, numpy
- scikit-learn
- matplotlib, seaborn
- mlxtend (for association rules)
- Jupyter Notebook (for interactive analysis)

---

##  Getting Started

1. Clone the Repository
2. Install Dependencies
3. Run the Analysis

### Output Visualizations
1.Actual vs Predicted Sales Scatter Plot
2.Purchase Classifier Metrics (Accuracy, Precision, Recall)
3.Clustering visualization for customer segments
4.Association Rules table for product recommendation

