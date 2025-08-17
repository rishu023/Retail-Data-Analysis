# Retail Data Analysis (SQL Project)

## 📌 Overview
This project analyzes an online **sports clothing retailer’s** database to extract insights that can help improve **revenue and marketing strategy**.  
The analysis is performed using **SQL queries inside a Jupyter Notebook**, focusing on product pricing, discounts, revenue, brand comparison, and customer engagement.

The database `sports` contains **5 interconnected tables** with `product_id` as the primary key:
- **info** – Product names, descriptions  
- **finance** – Pricing, discounts, revenue  
- **reviews** – Customer ratings & review counts  
- **traffic** – Website visit timestamps  
- **brands** – Brand information (Nike, Adidas, etc.)

---

## ⚙️ Setup & Requirements
- **PostgreSQL** database connection  
- **ipython-sql** extension for running SQL in Jupyter Notebook  
- Jupyter Notebook / JupyterLab  

Install required libraries:
```bash
pip install ipython-sql psycopg2
```

Load SQL extension inside the notebook:
```python
%load_ext sql
%sql postgresql:///sports
```

---

## 📊 Key Analyses & Queries
1. **Data Completeness Check**  
   - Count total rows and identify missing values in product descriptions, prices, and traffic data.  

2. **Nike vs. Adidas Pricing**  
   - Compare product price distributions across brands.  
   - Highlight stock range and customer target segments.  

3. **Price Range Categorization**  
   - Group products into categories: **Budget, Average, Expensive, Elite**.  
   - Compute revenue contributions for each brand and category.  

4. **Discount Analysis**  
   - Calculate **average discount %** by brand.  
   - Investigate discount strategies and their effect on revenue.  

5. **Ratings & Reviews Impact**  
   - Study the correlation between product ratings/reviews and revenue.  
   - Identify which products have high engagement vs. low revenue.  

6. **Website Traffic Trends**  
   - Track product popularity through `last_visited` timestamps.  
   - Evaluate whether frequently viewed products translate to higher sales.  

---

## 🚀 Insights & Recommendations
- **Adidas consistently outperforms Nike in total revenue**, especially in the **Elite price segment**.  
- Increasing stock in high-performing categories (e.g., Adidas Elite) can boost revenue.  
- **Discount strategies differ across brands** and significantly affect revenue.  
- Website traffic & review patterns can help **predict best-sellers**.  

---

## 📂 Project Structure
```
retail_data.ipynb   # Jupyter Notebook with all queries & insights
README.md           # Project documentation
```

---

## 📌 Future Work
- Automate ETL pipeline for regular revenue insights.  
- Extend analysis to include **seasonality & customer demographics**.  
- Build a **dashboard (Tableau/PowerBI/Streamlit)** for real-time business insights.  
