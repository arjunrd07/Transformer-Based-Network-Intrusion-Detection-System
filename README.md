# 🛡️ Transformer-Based Network Intrusion Detection System

## 📌 Overview
This project is a **cybersecurity tool** that uses a **Transformer-based deep learning model** to detect malicious network traffic. It applies the **Linformer architecture**, which is a faster and more efficient version of the Transformer, to classify traffic as either **Normal** or **Attack**.

---

## 📊 Datasets
The system is trained and tested on two well-known benchmarks:
- **UNSW-NB15** → Main dataset with modern attack types.  
- **NSL-KDD** → Used to check how well the model generalizes to new environments.  

---

## 🛠️ Workflow
1. **Data Preprocessing**  
   - Clean missing values.  
   - Encode categorical features (protocol, service, etc.).  
   - Scale numerical features for consistency.  

2. **Model**  
   - **Linformer layer** for efficient attention.  
   - **MLP classifier** for final prediction.  

3. **Training**  
   - GPU acceleration with mixed precision.  
   - Balanced class weights to handle data imbalance.  

---

## 📈 Results
- **UNSW-NB15**: ~88% accuracy, F1-score ~0.90.  
- **NSL-KDD**: ~74% accuracy, showing good generalization.  

---

## 🚀 Usage
1. Open the notebook:  
   `Transformer-Based Network Intrusion Detection System.ipynb`  
2. Place the dataset files (`.parquet`) in the working directory.  
3. Run the cells step by step to:  
   - Preprocess data  
   - Train the model  
   - Evaluate performance  
