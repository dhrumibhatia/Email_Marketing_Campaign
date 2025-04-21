# Email Marketing Campaign – ML Optimization

**A data-driven approach to maximizing click-through rates in email marketing campaigns**

---

## 📖 Overview
This project analyzes and optimizes an email marketing campaign for an e-commerce platform. By leveraging user and email metadata, we build predictive models to target users most likely to click promotional links, driving higher engagement and ROI.

## 🗂 Project Structure
```
├── .gitattributes
├── Email_Marketing_Campaign.ipynb
├── basic_analysis_without_documentation.ipynb
├── email_table.csv
├── email_opened_table.csv
├── link_clicked_table.csv
└── README.md
```


## 🧠 Methodology
1. **Merge & Clean**: Combine email, open, and click tables; handle missing values.
2. **EDA**: Uncover trends by email format, timing, and user demographics.
3. **Feature Engineering**: Encode categorical data; derive time and behavioral features.
4. **Modeling**: Train classification models (Logistic Regression, Random Forest, XGBoost).
5. **Evaluation**: Use accuracy, precision, recall, F1-score, and ROC-AUC; estimate CTR uplift.
6. **Segment Insights**: Identify high-value user groups for targeted campaigns.

## 📊 Email Marketing Campaign Analysis Summary

## 📋 Key Questions Answered

1. **📈 Email Performance Metrics:**
   - **Open Rate:** 10.35% of users opened the email
   - **Click-Through Rate (CTR):** 2.12% of users clicked the link

2. **🤖 Model Effectiveness:**
   - Multiple models were built (Logistic Regression, Random Forest, Gradient Boosting)
   - Models faced challenges due to class imbalance in the dataset
   - Random Forest showed best performance among tested models

3. **⚡ Potential CTR Improvement:**
   - Based on segment analysis, targeted campaigns could potentially double CTR
   - Testing method: A/B testing between random targeting (control) and model-driven targeting

4. **👥 User Segment Patterns:**
   - **Email Content:** Personalized emails (2.73% CTR) outperformed generic emails (1.51% CTR)
   - **Geography:** UK/US users showed higher engagement than Spain/France users
   - **Timing:** Wednesday emails performed best; Friday emails performed worst
   - **User History:** Strong correlation between past purchase frequency and engagement
   - **Email Format:** Shorter emails generated higher CTR

## 🔍 Key Insights

| Segment | Finding | Opportunity |
|---------|---------|-------------|
| **Content** | Personalized emails drove 81% higher CTR | Expand personalization efforts |
| **Geography** | UK/US audiences were most responsive | Tailor messaging by region |
| **Timing** | Wednesday was top performing day | Optimize send schedule |
| **Engagement** | High-purchase users were 3x more likely to click | Prioritize engaged customers |
| **Format** | Brevity improved performance | Keep messages concise |

## 🚀 Next Steps

1. **Address Data Challenges:**
   - Implement SMOTE or class weights to handle imbalanced data
   - Improve model performance through balanced sampling techniques

2. **Enhance Feature Engineering:**
   - Focus on top-performing features identified by tree-based models
   - Create interaction features between high-performing segments
   - Develop more granular time-based features

3. **Implement Targeting Strategy:**
   - Deploy segment-specific campaigns based on identified patterns
   - Establish continuous A/B testing framework to validate improvements
   - Develop automated segmentation system for optimal targeting

By implementing these recommendations, we estimate potential to double the current 2.12% CTR through strategic targeting of high-probability user segments.



*This README provides a snapshot of the project. For detailed code and analyses, refer to the Jupyter notebook in the `notebooks/` directory.*


