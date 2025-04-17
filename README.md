# Email-Marketing-Campaign-Optimization


## 📌 Overview
This project explores how an e-commerce company can optimize its email marketing strategy using machine learning. The goal is to:
- Understand user engagement (opens and clicks)
- Build a model to predict click behavior
- Estimate how much the click-through rate (CTR) can be improved
- Uncover insights across different user segments

## 🧾 Dataset Description
The case study uses three CSV files:

### `email_table.csv`
- `email_id`: Unique ID of each email sent
- `email_text`: Version of the email text (long/short)
- `email_version`: Personalized or generic email
- `hour`: Time when the email was sent
- `weekday`: Day of the week
- `user_country`: Country of the user
- `user_past_purchases`: Number of previous purchases

### `email_opened_table.csv`
- `email_id`: Emails that were opened by users

### `link_clicked_table.csv`
- `email_id`: Emails whose links were clicked

## ⚙️ How to Run
1. Clone this repo
2. Place the three CSV files in the root directory
3. Open and run the notebook: `email_campaign_analysis.ipynb`
4. Install required libraries if needed:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## 🔍 Key Tasks Performed
### 1. Open Rate and Click-Through Rate
- Calculated total % of users who opened the email
- Calculated % of users who clicked the link

### 2. ML Model to Predict Click Behavior
- Preprocessed categorical features
- Used Random Forest Classifier
- Evaluated with classification report, confusion matrix, and ROC-AUC

### 3. CTR Improvement Estimation
- Estimated improvement by only targeting users likely to click (based on model probability)

### 4. Segment Analysis
- Analyzed click patterns by:
  - Email text type
  - Personalization
  - Day of week
  - Country

## 📈 Findings
- Personalized emails slightly improve click rates
- Certain countries respond better than others
- Emails sent at specific hours/days perform better
- Model predicts click behavior with promising accuracy

## ✅ Conclusion
Using historical data and a predictive model, companies can significantly improve email marketing performance by targeting only users who are most likely to engage. This reduces wasted emails and enhances user experience.

---

Author: ML Intern - Case Study Task


