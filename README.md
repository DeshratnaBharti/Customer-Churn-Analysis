
Customer-Churn-Analysis

Project title
-----------------
Customer Churn Analysis (a small beginner project)

What I tried to do (in simple words)
-----------------
I wanted to see why some customers leave a telecom. I used small checks like how long they stayed (`tenure`), how much they pay (`MonthlyCharges`), and what kind of contract they had. This was mostly for learning — not a perfect study.

Dataset source
-----------------
Dataset: Telco Customer Churn (Kaggle)
Link: https://www.kaggle.com/blastchar/telco-customer-churn

Tools I used
-----------------
- Python (pandas, matplotlib, seaborn)
- Jupyter Notebook
- Power BI (I made a simple screenshot of the dashboard)
- Excel for quick checks sometimes

Steps I followed (short)
-----------------
1. Put a small sample CSV in `data/` so notebook runs quickly.
2. Loaded data in a notebook and checked types.
3. Cleaned `TotalCharges` and dropped a few bad rows.
4. Did simple EDA: churn rate, churn by contract, MonthlyCharges distribution, tenure boxplot.
5. Made simple charts and exported a Power BI screenshot.

What I noticed (student notes)
-----------------
- Month-to-month customers seemed to leave more.
- New customers (low tenure) had higher churn.
- Higher monthly bill sometimes linked to churn, but it's not a clear rule.

Problems I faced (real student)
-----------------
- At first I didn't understand `TotalCharges` — it loaded as text and gave errors. I used `pd.to_numeric(..., errors='coerce')` and then cleaned NaNs.
- I tried a fancy chart in Power BI but it looked messy, so I kept simpler charts.
- Sometimes I mixed up axes in plots — a small stupid mistake I fixed.

What I learned
-----------------
- Basic cleaning: convert types, check NaNs, small fixes.
- EDA basics: `groupby`, `value_counts`, simple plots.
- How to prepare a few visuals for a Power BI dashboard.

Files here
-----------------
- `data/` : sample CSV kept small for repo.
- `notebooks/` : simple notebooks with code.
- `dashboard/` : screenshot(s) from Power BI.
- `README.md` : this file.

Quick run (very quick)
-----------------
```bash
pip install -r requirements.txt
jupyter lab
```

Git push (what I ran)
-----------------
If you want to upload to GitHub, these are the basic steps I used:
```bash
git init
git add .
git commit -m "first data analysis project"
git branch -M main
git remote add origin https://github.com/DeshratnaBharti/Customer-Churn-Analysis.git
git push -u origin main
```

Small note
-----------------
I made this as a learning project. If something looks off, it's probably me experimenting — which is the point :)

