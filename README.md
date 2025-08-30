# Should We Build a Pipeline?  
### Data Pipeline Readiness Assessments  

This repository contains structured assessments of multiple datasets to evaluate their readiness for production-grade data pipelines. Each assessment considers **data quality**, **model performance**, and **leakage risk**, leading to actionable recommendations for deployment.  

---

## 📊 Assessments Included

### 1. Employee Promotion Data Pipeline  
- **Dataset Size:** 100 records, 17 fields  
- **Readiness Score:** 66.1 / 100  
- **Key Insights:**  
  - Excellent data quality (100.0) but significant leakage risks (25.0).  
  - Logistic Regression accuracy: 73.3% (AUC: 0.614).  
  - Promotion heavily influenced by **advanced degrees (40.1%)** and **department bias (31.7%)**.  
- **Recommendation:** Conditional implementation — expand dataset size, mitigate bias, and refine model before deployment.  

---

### 2. Student Admissions Data Pipeline  
- **Dataset Size:** 100,000 records, 12 fields  
- **Readiness Score:** 80.6 / 100  
- **Key Insights:**  
  - High data quality (90.0), solid predictive performance (81.9% accuracy, AUC: 0.682).  
  - **Early Decision status** dominates predictive power (83.3%).  
  - Minor socioeconomic bias risk linked to **Application Fee**.  
- **Recommendation:** Ready for production. Proceed with phased rollout and fairness audits.  

---

### 3. eBay Price Prediction Data Pipeline  
- **Dataset Size:** 1,000 records, 8 fields  
- **Readiness Score:** 100.0 / 100  
- **Key Insights:**  
  - Perfect data quality, predictive performance (R² = 1.000), and no leakage risks.  
  - **Shipping price** explains ~99.95% of predictive power.  
  - Strong category diversity (Art, Electronics, Fashion, Antiques, Automotive).  
- **Recommendation:** Immediate production deployment.  

---

## 🧩 Methodology  
Each pipeline was scored across three key dimensions:  
1. **Data Quality** – completeness, cleanliness, structure.  
2. **Model Performance** – accuracy, AUC, R², RMSE.  
3. **Leakage Risk** – redundancy, bias, or variables leaking target information.  

---

## ✅ Conclusion  
- **Employee Promotion Pipeline**: Needs refinement before use.  
- **Student Admissions Pipeline**: Ready for phased deployment.  
- **eBay Price Prediction Pipeline**: Fully production-ready.  

This repository provides a repeatable framework for **data pipeline readiness assessments**, balancing **data integrity, fairness, and operational scalability**.  

---

### 🔗 Authors
Cedric Lambert  
