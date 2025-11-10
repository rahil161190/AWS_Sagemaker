# AWS SageMaker Demo 🚀

## 📌 Overview
Amazon SageMaker is a managed ML platform to **build, train, and deploy models** at scale.  

**Key benefits:**
- Jupyter‑style notebooks with GPU/large RAM options  
- Pre‑built optimized algorithms (XGBoost, PCA, Seq2Seq, etc.)  
- Seamless integration with **S3 & other AWS services**  
- Cost‑efficient when data is stored in S3  

---

## 🛠️ What I Did
1. **Setup**
   - Created S3 bucket `bucketrahil7nov`  
   - Defined output path for model artifacts  

2. **Data Prep**
   - Downloaded **Bank Marketing dataset** (`bank_clean.csv`)  
   - Split into train/test, uploaded to S3  

3. **Training**
   - Used **XGBoost built‑in algorithm** on `ml.m5.2xlarge`  
   - Tuned hyperparameters (`max_depth=5`, `eta=0.2`, etc.)  
   - Training logloss reduced from **0.57 → 0.27**  

4. **Deployment**
   - Deployed endpoint: `sagemaker-xgboost-2025-11-07-11-34-01-578`  
   - Invoked predictions via `CSVSerializer`  

5. **Evaluation**
   - Accuracy: **90%**  
   - Precision (class 1): **0.66**  
   - Recall (class 1): **0.21**  

---

## 📊 Key Takeaways
- End‑to‑end ML pipeline: **data → training → deployment → evaluation**  
- Hands‑on with **S3, SageMaker Estimator, and endpoint testing**  
- Scope for improving recall with class balancing/tuning  

---
