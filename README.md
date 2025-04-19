# Email Marketing Campaign - ML Case Study

The ML case study project analyses and optimizes an email marketing campaign using data science and machine learning techniques.

## Objective

The goal is to understand user engagement with marketing emails and build an optimal model that predicts which users are most likely to click on links within emails. This helps improve the Click-Through Rate (CTR) and optimize future campaigns.

---

## Dataset

Three CSV files were used:

1. **email_table.csv**  
   Contains email metadata: user info, email content type, time sent, etc.

2. **email_opened_table.csv**  
   A list of `email_id`s that were opened by users.

3. **link_clicked_table.csv**  
   A list of `email_id`s where users clicked the internal link.

---

## Key Questions Answered

- What percentage of users opened the email and what percentage of users clicked the link within the email?
- Can we build a machine learning model to predict link clicks?
- How much can we improve the click-through rate using our model?
- Are there any patterns in performance across different user segments?

---

## Steps Taken

- Data Merging & Preprocessing
- Exploratory Data Analysis (EDA)
- Categorical Encoding
- Model Training:
  - Logistic Regression
  - Random Forest
- Model Evaluation (Accuracy, AUC)
- CTR Uplift Simulation (Top 20% targeting)
- Segment Analysis by Country, Email Text & Personalization

---

## Results

- **Logistic Regression** had the highest AUC among the models used and was selected as the best model in the particular scenario.
- Simulated targeting of top 20% most likely to click users led to a significantly higher CTR. Potential CTR Uplift found out to be 3.10%.
- Segments with personalized, short text emails in US (country) performed the best.

---

## Tech Stack Used

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Scikit-learn
