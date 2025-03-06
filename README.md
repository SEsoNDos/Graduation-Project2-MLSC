# Graduation-Project2-MLSC
# E-Commerce Customer Segmentation 

## 📌 Project Overview
This project focuses on analyzing customer data from an e-commerce platform to provide insights through a well-structured dashboard and an effective customer segmentation model. The goal is to help stakeholders make data-driven decisions regarding customer engagement, coupon strategies, and marketing efforts.

## Dataset Description
The dataset consists of multiple interrelated tables that contain essential customer, transaction, and business-related information:

1. **Customers Table:** Contains details about customers, including their unique IDs, join dates, cities, and genders.
2. **Genders Table:** Maps gender IDs to gender names (e.g., Male, Female).
3. **Cities Table:** Maps city IDs to city names.
4. **Transactions Table:** Stores transaction details such as transaction dates, coupon statuses (claimed/burnt), and branch information.
5. **Branches Table:** Links branch IDs to merchant IDs.
6. **Merchants Table:** Maps merchant IDs to merchant names.

## Project Requirements

### 1. Dashboard for Stakeholders
A dashboard was developed to visualize key insights, helping business managers and marketing teams understand customer behavior. The following visualizations were included:

- **Customer Demographics:** A breakdown of customers by gender and city using pie charts.
- **Coupon Usage Trends:** A time-series analysis of claimed vs. burnt coupons.
- **Top-performing Cities and Branches:** Bar charts highlighting the cities and branches with the highest number of successful coupon burns.
- **Customer Retention & Loyalty Analysis:** Histograms and line charts illustrating customer coupon usage frequency.

### 2. Customer Segmentation using Machine Learning
To better understand customer behavior, an unsupervised learning model was applied for customer segmentation. The steps included:

#### **Feature Selection & Preprocessing**
- Selected relevant features such as customer demographics (city, gender) and transaction behavior (coupon usage frequency, transaction status).
- Standardized the data using `StandardScaler` for optimal model performance.

#### **Model Development & Clustering**
- Applied **K-Means clustering** to segment customers.
- Used the **Elbow Method** and **Silhouette Score** to determine the optimal number of clusters.
- Visualized customer segmentation using **PCA (Principal Component Analysis)** for dimensionality reduction.

#### **Model Evaluation**
- **Silhouette Score:** Evaluated cluster cohesion and separation.
- **Inertia:** Used to determine clustering effectiveness.

#### **Segment Analysis & Recommendations**
- Analyzed each customer segment based on dominant city and gender distributions.
- Provided insights on which segments should receive more targeted coupons and promotions to enhance customer loyalty and engagement.

## Results & Insights
- The **dashboard** provided clear and actionable insights into customer distribution and transaction trends.
- The **segmentation model** successfully grouped customers based on behavioral patterns, allowing for targeted marketing strategies.
- Key recommendations included increasing promotions in high-engagement cities and personalizing offers based on customer segment characteristics.

## Repository Structure
```
📂 customer_segmentation_project
│-- 📂 data/               # Raw and processed data files
│-- 📂 notebooks/          # Jupyter Notebooks for data analysis and modeling
│-- 📂 reports/            # Visualized reports and dashboard screenshots
│-- README.md             # Project documentation
│-- requirements.txt      # Dependencies and libraries used
```

## How to Run the Project
1. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
2. Run the Jupyter Notebook to preprocess the data and train the model.
3. Open the dashboard file (`dashboard.html` or `dashboard.ipynb`) to explore the visual insights.

## Technologies Used
- **Python** (Pandas, NumPy, Matplotlib, Seaborn, Plotly)
- **Machine Learning** (K-Means Clustering, PCA, Scikit-learn)
- **Data Visualization** (Dashboards with Matplotlib, Seaborn, Plotly)

## Conclusion
This project successfully provided a data-driven approach to understanding customer behavior in an e-commerce setting. By leveraging visualization and machine learning techniques, we identified key customer segments, helping stakeholders improve customer engagement strategies and optimize coupon distribution.

---

## 👨‍💻 Author

**Sondos Sofian**
📧 Contact:sondosso889@gmail.com



