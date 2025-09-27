# Customer Segmentation and Churn Prediction

This project performs **customer segmentation using KMeans clustering** and builds a **churn prediction model** using machine learning.  
It is based on a marketing campaign dataset and explores customer personas, behavior patterns, and churn risk.

---

## 📂 Project Structure
- `costumer-personality-analyzer.ipynb` → Main Jupyter Notebook containing code, visualizations, and analysis.
- `marketing_campaign.csv` → Dataset file (tab-separated).
- `requirements.txt` → Python dependencies for running the notebook.

---

## 🚀 Workflow
1. **Data Preprocessing**
   - Handle missing and duplicate values.
   - Feature engineering: Age, Tenure, Expenses, Kids, Total Purchases, Campaigns Accepted.
   - Encoding categorical features (Education, Marital Status).
   - Standardization of numerical features.

2. **Customer Segmentation**
   - Applied **KMeans clustering**.
   - Used **Elbow Method** to find the optimal number of clusters.
   - Created cluster personas based on Income, Expenses, Purchases, and Tenure.

3. **Churn Definition**
   - Customers are marked as churn if:
     - They did not respond to campaigns, and
     - Their expenses or purchases were below thresholds.

4. **Churn Prediction**
   - Split dataset into **train/test** with stratification.
   - Built a **Random Forest Classifier** with hyperparameters tuning.
   - Evaluated with ROC-AUC, confusion matrix, and classification report.

5. **Insights**
   - Clusters differ by **income, spending, loyalty (tenure), and churn rate**.
   - Identified high-value customers vs. high-risk churners.
   - Visualized patterns using pairplots, heatmaps, and scatterplots.

---

## 📊 Key Results
- **ROC-AUC** score: ~0.98+ (varies by run).
- **Cluster insights** show distinct customer groups:
  - Low-income + high churn risk.
  - High-income + loyal, low churn.
  - Mid-tier income with moderate engagement.

---

## 🛠️ Installation
Clone the repository and install dependencies:

```bash
git clone <https://github.com/here-2007/Customer-Personality-Analyser.git>
pip install -r requirements.txt
```

## Launch Jupiter Notebook
```bash
jupyter notebook costumer-personality-analyzer.ipynb
```
