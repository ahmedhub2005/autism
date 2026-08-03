#  Autism Spectrum Disorder (ASD) Prediction

##  Project Description
This project aims to predict the likelihood of Autism Spectrum Disorder (ASD) in individuals using machine learning and deep learning models.  
We explored **traditional ML models** (Random Forest, Logistic Regression, XGBoost, SVC, Gradient Boosting) and a **Neural Network** with multiple layers.  

The goal is to assist early detection of ASD traits using structured questionnaire data.

---

##  Dataset
- Source: [Autism Screening Dataset](https://www.kaggle.com/competitions/autismdiagnosis/data)  
- Records: ~700 samples  
- Features:  
  - 10 Behavioral Score Questions (A1–A10)  
  - Demographics: Age, Gender, Ethnicity, etc.  
  - Target: **Class/ASD (0 = No, 1 = Yes)**  

Missing and unknown values were handled by replacing them with **0/1 encoding**.

---

##  Models Used
- Logistic Regression  
- Random Forest Classifier  
- Gradient Boosting Classifier  
- Support Vector Classifier (SVC)  
- XGBoost Classifier  
- Deep Learning (Neural Network with 3 Dense Layers + Dropout + Batch Normalization)  

---

##  Model Performance
| Model                  | Accuracy | Precision | Recall | F1-Score |
|-------------------------|----------|-----------|--------|----------|
| Logistic Regression     | 0.87     | 0.85      | 0.83   | 0.84     |
| Random Forest           | 0.91     | 0.90      | 0.89   | 0.89     |
| Gradient Boosting       | 0.90     | 0.89      | 0.88   | 0.88     |
| SVC                     | 0.88     | 0.86      | 0.85   | 0.85     |
| XGBoost                 | 0.92     | 0.91      | 0.90   | 0.91     |
| Neural Network (NN)     | 0.93     | 0.92      | 0.91   | 0.91     |

✅ The **Neural Network** achieved the **best performance** with strong generalization.

---





##  How to Run

```bash
# Clone repo
git clone https://github.com/username/autism-prediction.git
cd autism-prediction

# Install dependencies
pip install -r requirements.txt

# Run training
python model_training.py
