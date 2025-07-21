# 📦 Swiggy Instamart EDA & Visual Insights

![Python](https://img.shields.io/badge/Python-3.11-blue?style=plastic&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data--Analysis-purple?style=plastic&logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-yellow?style=plastic)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-green?style=plastic)
![Status](https://img.shields.io/badge/Project-Complete-brightgreen?style=plastic)
![License](https://img.shields.io/badge/License-MIT-orange?style=plastic)

> 📌 **By [Farha Kousar](https://www.linkedin.com/in/farhakousar16/)**  
> ⭐ _If you find this useful, don't forget to give it a star on GitHub!_



## 📘 Overview

This project presents an exploratory data analysis (EDA) on Swiggy Instamart’s order data. It covers merging order-level and product-level details, calculating KPIs like revenue and delivery efficiency, and visualizing patterns in sales, product demand, and delivery behavior.



## 📁 Dataset

- `OrderDetails.csv`: Includes individual product orders with quantity and price.
- `Orders.csv`: Includes order-level details such as customer, order time, delivery time, and status.



## 🔧 Technologies Used

- `Python` (v3.11+)
- `pandas` for data manipulation
- `matplotlib` & `seaborn` for visualizations
- Jupyter / Kaggle Notebook


## 🔍 Key Calculations & Features

### ✅ Data Processing

- Merged `order_details` and `orders` using `OrderID`
- Converted `OrderDateTime` and `DeliveryDateTime` to datetime
- Created `DeliveryTime (mins)` and `TotalProductPrice` fields


## 📊 KPIs & Metrics

| Metric                | Value Computed                    |
|-----------------------|-----------------------------------|
| 🧾 Total Orders       | `nunique(OrderID)`                |
| 👥 Total Customers    | `nunique(CustomerID)`             |
| 💰 Total Revenue      | `sum(Quantity * PricePerUnit)`    |
| 📦 Avg Order Value    | `mean(TotalProductPrice per Order)` |
| ⏱️ Avg Delivery Time | `mean(DeliveryTime(mins))`        |



## 📈 Visualizations

### 🛒 Top 10 Most Ordered Products
Bar chart of most frequently ordered products based on total quantity.

### 🚚 Delivery Status Distribution
Shows the proportion of delivered, pending, or canceled orders.

### 📅 Daily Revenue Trend
Line chart of total revenue by order date.

### ⏰ Hourly Order Volume
Line plot showing how order frequency varies by hour of day.

### 🔥 Heatmap: Orders by Day & Hour
Heatmap to visualize order density across weekdays and hours.



## 📌 How to Run

1. Clone the repository or open the Kaggle notebook:  
   👉 [Swiggy Instamart Kaggle Notebook](https://www.kaggle.com/code/farhakouser/swiggy-instamart-ipynb)

2. Run the cells sequentially — data is read from:
   ```python
   pd.read_csv("/kaggle/input/orderdetails-csv/OrderDetails.csv")
   pd.read_csv("/kaggle/input/orders/Orders.csv")


   ## ✨ Author

- 👩‍💻 Farha Kousar  
  [![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/farhakousar16)  
  [![GitHub](https://img.shields.io/badge/-GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/FarhaKousar1601)  
  [![Ko-Fi](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-ko--fi-FF5E5B?style=flat&logo=ko-fi&logoColor=white)](https://ko-fi.com/farhakousar16)


## 🌟 Support

If you found this helpful, please consider giving a ⭐ to the [GitHub repository](https://github.com/FarhaKousar1601)  
and follow for more exciting data science projects.

> 📬 Feel free to connect with me for collaborations, internships, and project guidance.

