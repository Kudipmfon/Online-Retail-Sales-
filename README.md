# **Online Retail Sale Forecast and Clustering**  
### **Final Report**  
**Author:** Kudipmfon Paul Okon  
**Date:** March 2025  
**Tools Used:** Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn  

---

## **1. Introduction**  
This project aims to develop a predictive model and clustering analysis for an **online retail sales dataset**. The objective is to **classify transactions, segment customers, and forecast sales trends** to improve business decision-making. The analysis identifies purchasing patterns, key sales drivers, and customer behavior to optimize inventory management and marketing strategies.  

---

## **2. Project Objectives**  
The main objectives of this analysis include:  

1. **Predictive Modeling** – Classify transactions based on purchasing behavior.  
2. **Clustering Analysis** – Identify customer and product segments using machine learning techniques.  
3. **Feature Engineering** – Create meaningful features from transaction data to improve model performance.  
4. **Sales Forecasting** – Predict future sales trends based on historical data.  
5. **Customer Segmentation** – Group customers based on their purchasing behavior to enhance targeted marketing strategies.  

---

## **3. Data Overview**  
The dataset used for this analysis is the **Online Retail Dataset** from the UCI Machine Learning Repository. It consists of **transactional records** from an e-commerce store, including purchase details from various customers.  

### **3.1 Data Features**  
| Feature | Description |
|---------|------------|
| `InvoiceNo` | Unique transaction identifier |
| `StockCode` | Product identifier |
| `Description` | Product description |
| `Quantity` | Number of items purchased |
| `InvoiceDate` | Date and time of purchase |
| `UnitPrice` | Price per unit |
| `CustomerID` | Unique customer identifier |
| `Country` | Customer’s country |

---

## **4. Methodology**  
The following steps were undertaken to conduct the analysis:  

### **4.1 Exploratory Data Analysis (EDA)**  
- **Data Cleaning:** Handling missing values and duplicate records.  
- **Visual Analysis:** Identified trends and seasonal variations.  
- **Outlier Detection:** Removed extreme values affecting analysis.  

### **4.2 Clustering Analysis for Customer Segmentation**  
- **RFM Analysis (Recency, Frequency, Monetary):** Categorized customers based on shopping behavior.  
- **K-Means Clustering:** Applied clustering algorithm to segment customers.  
- **Data Visualization:** Used scatter plots and heatmaps for insights.  

### **4.3 Feature Engineering**  
- Extracted **time-based features** (season, day of the week, hour of purchase).  
- Created **aggregated customer metrics** (total spending, purchase frequency).  

### **4.4 Sales Forecasting Model**  
- **Time Series Analysis:** Examined historical sales trends.  
- **Statistical Models:** Evaluated ARIMA, Prophet, and LSTM for forecasting.  
- **Model Selection:** Chose the best-performing model based on accuracy.  

### **4.5 Predictive Modeling**  
- **Classification Task:** Used ML models to classify transactions.  
- **Hyperparameter Tuning:** Optimized model performance.  

---

## **5. Key Findings**  

### **5.1 Product Sales Insights**  
- **Top-Selling Products:**  
  - **SET 2 TEA TOWELS I LOVE LONDON**  
  - **SPACEBOY BABY GIFT SET**  
  - Both products exceeded **7,000 sales**.  
- **Low-Performing Products:**  
  - **4 PURPLE FLOCK DINNER CANDLES** had significantly fewer sales.  

### **5.2 Seasonal Sales Trends**  
- **Q4 (October – December) had the highest sales**, peaking in November.  
- **Q1 (January – March) had the lowest sales.**  
- **Thursdays had the highest sales activity.**  

### **5.3 Customer Segments**  
Three main customer groups were identified:  
1. **Frequent Buyers (Green Cluster):**  
   - High purchase frequency, fast return rate.  
   - Likely to respond to loyalty programs.  
2. **Moderate Buyers (Orange Cluster):**  
   - Occasional buyers, moderate recency.  
   - Can be engaged through personalized promotions.  
3. **Rare Buyers (Blue Cluster):**  
   - Large population, but low purchase frequency.  
   - Requires re-engagement campaigns.  

---

## **6. Recommendations**  

### **6.1 Inventory Management**  
- **Stock high-demand products** like *SET 2 TEA TOWELS I LOVE LONDON* and *SPACEBOY BABY GIFT SET*.  
- **Reduce inventory for low-selling items** to optimize costs.  
- **Increase stock levels before peak sales months (September–November).**  

### **6.2 Marketing Strategies**  
- **Boost advertising in Q4 (October – December)** for maximum returns.  
- **Increase promotions in low-sales months (April & July).**  
- **Focus marketing on Thursdays**, the highest sales day.  
- **Implement weekend deals** to improve engagement on Saturdays and Sundays.  

### **6.3 Customer Retention**  
- **Frequent Buyers (Green Cluster):**  
  - Introduce **loyalty programs** or exclusive discounts.  
- **Moderate Buyers (Orange Cluster):**  
  - Use **personalized promotions** or email reminders.  
- **Rare Buyers (Blue Cluster):**  
  - **Re-engagement campaigns** with discounts and targeted ads.  

---

## **7. Project Structure**  
```
/Online-Retail-Sales-Analysis
│── data/                     # Raw and processed datasets  
│── notebooks/                 # Jupyter notebooks for EDA, modeling, and visualization  
│── models/                    # Trained machine learning models  
│── src/                       # Python scripts for data preprocessing and analysis  
│── reports/                   # Final report and presentation  
│── README.md                  # Project documentation (this file)  
│── requirements.txt           # Dependencies and package requirements  
│── LICENSE                    # Open-source license  
```

---

## **8. Installation & Usage**  
### **8.1 Clone the Repository**  
```bash
git clone https://github.com/yourusername/Online-Retail-Sales-Analysis.git
cd Online-Retail-Sales-Analysis
```
### **8.2 Create a Virtual Environment**  
```bash
python -m venv env
source env/bin/activate  # Linux/macOS
env\Scripts\activate     # Windows
```
### **8.3 Install Dependencies**  
```bash
pip install -r requirements.txt
```
### **8.4 Run Jupyter Notebook**  
```bash
jupyter notebook
```

---

## **9. Technologies Used**  
- **Python:** Data analysis & modeling  
- **Pandas & NumPy:** Data preprocessing  
- **Matplotlib & Seaborn:** Data visualization  
- **Scikit-learn:** Machine learning & clustering  
- **Statsmodels:** Time series analysis  

---

## **10. Future Work**  
- Add features such as **holiday seasons, discounts, and viral trends** to enhance forecasting accuracy.  
- Explore **advanced clustering techniques (DBSCAN, Hierarchical Clustering)** for better customer segmentation.  
- Implement **deep learning models** for improved sales forecasting.  

---

## **11. Conclusion**  
This project provided valuable insights into **customer behavior, product demand, and sales trends** in online retail. The **clustering models** helped identify different customer groups, and the **sales forecasting models** provided actionable predictions for future sales. The findings and recommendations can be used to enhance **marketing strategies, inventory planning, and customer engagement**.  

---

## **12. License**  
This project is licensed under the **MIT License**.  
