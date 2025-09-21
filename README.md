# Healthcare Fraud Detection  
Machine Learning Models for Identifying Fraudulent Providers in Medicare Claims  

<img width="979" height="637" alt="image" src="https://github.com/user-attachments/assets/4ff6b113-5b34-474f-9ffb-b26ce26c5d31" />

## Overview  
This project applies machine learning and anomaly detection to identify fraudulent healthcare providers using claims data.  
The study integrates unsupervised and supervised models, evaluates their performance, and highlights the key fraud indicators in provider behavior.  
It also demonstrates how insurers and policymakers can benefit from hybrid pipelines that balance recall, interpretability, and scalability.  

## Project Structure  
The repository includes the following:  

- **Healthcare_Fraud_Detection.ipynb**: Complete Jupyter Notebook with data processing, visualizations, model training, and evaluation.  
- **Data/**: Training and testing datasets (providers, inpatient, outpatient, beneficiaries).  
- **Visuals/**: High-resolution figures including model performance comparisons, ROC and PR curves, and feature importance plots.  
- **Article.pdf**: Research-style article summarizing findings, implications, and future directions.  

## Methodology  

### Data Sources  
- Medicare provider claims datasets (train/test splits of inpatient, outpatient, and beneficiary files).  
- Labels on fraudulent vs non-fraudulent providers.  

### Techniques Used  
- **Exploratory Data Analysis (EDA):** Distribution analysis, reimbursement trends, fraud vs non-fraud comparisons.  
- **Unsupervised Models:** Isolation Forest, Local Outlier Factor, Autoencoders.  
- **Supervised Models:** Logistic Regression, Random Forest, XGBoost.  
- **Evaluation Metrics:** Accuracy, ROC-AUC, PR-AUC, Recall, Precision.  
- **Interpretability:** Feature importance, model coefficients, SHAP insights.  

## Key Findings  
- Fraudulent providers tend to submit **unusually high inpatient and outpatient reimbursements**.  
- **Anomaly detection** generates useful early warnings but misses many fraud cases.  
- **Random Forest** consistently outperformed other models (Accuracy = 0.982, ROC-AUC = 0.989, Recall = 0.855).  
- **Hybrid pipelines** that combine anomaly detection with supervised learning provide the best balance between coverage and precision.  

## Why It Matters  
- **For Insurers:** Improves fraud detection efficiency, saving millions in losses.  
- **For Policymakers:** Highlights how recall should be prioritized to reduce systemic waste.  
- **For Practitioners:** Offers interpretable models that scale to millions of claims.  

## Looking Ahead  
- Scaling models for **big data** environments (Spark, distributed ML).  
- Integration with **business intelligence tools** for real-time investigation dashboards.  
- Use of **deep learning and graph-based methods** to detect fraud rings.  
- Adoption of **active learning** pipelines to improve models continuously with auditor feedback.  

## Usage  

To explore the project locally:  

```bash
# Clone the repository
git clone https://github.com/your-handle/Healthcare-Fraud-Detection.git
cd Healthcare-Fraud-Detection
