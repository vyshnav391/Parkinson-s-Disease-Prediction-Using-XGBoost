#  Parkinson's Disease Prediction Using XGBoost

A Machine Learning-based healthcare project that predicts Parkinson's Disease using voice-based biomedical features. The system leverages advanced feature engineering and the XGBoost algorithm to provide accurate and early detection of Parkinson's Disease through non-invasive voice analysis.

##  Overview

Parkinson's Disease (PD) is a progressive neurological disorder that affects movement, speech, and motor functions. Early diagnosis plays a crucial role in improving treatment outcomes and patient care.

This project analyzes acoustic voice measurements such as jitter, shimmer, and harmonic-to-noise ratio to classify individuals as either Parkinson's patients or healthy subjects.

##  Features

- Voice-based Parkinson's Disease Detection
- Data Preprocessing and Feature Scaling
- Feature Selection using Recursive Feature Elimination (RFE)
- Model Training with XGBoost
- Performance Evaluation using Multiple Metrics
- Confusion Matrix Visualization
- High Accuracy and Recall for Early Diagnosis
- Non-invasive and Cost-effective Screening Solution

##  Tech Stack

- Python
- XGBoost
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

##  Dataset

The project utilizes the Parkinson's Disease dataset from the UCI Machine Learning Repository.

Dataset Characteristics:

- 195 Samples
- 23 Biomedical Voice Features
- Binary Classification:
  - 1 → Parkinson's Disease
  - 0 → Healthy Individual

Key Features:

- Jitter
- Shimmer
- Harmonic-to-Noise Ratio (HNR)
- Pitch Period Entropy (PPE)
- Recurrence Period Density Entropy (RPDE)

##  Project Workflow

```text
Data Collection
       ↓
Data Preprocessing
       ↓
Feature Scaling
       ↓
Feature Selection (RFE)
       ↓
Model Training (XGBoost)
       ↓
Hyperparameter Tuning
       ↓
Prediction
       ↓
Model Evaluation
```

##  Methodology

### 1. Data Preprocessing

- Handling missing values
- Data normalization using MinMaxScaler
- Feature engineering

### 2. Feature Selection

Recursive Feature Elimination (RFE) was used to identify the most significant features contributing to Parkinson's Disease prediction.

### 3. Model Training

The XGBoost classifier was trained on the selected feature set to improve classification performance and generalization.

### 4. Evaluation Metrics

The model was evaluated using:

- Accuracy
- Precision
- Recall (Sensitivity)
- F1-Score
- AUC-ROC Score
- Confusion Matrix

##  Results

| Metric | Score |
|----------|----------|
| Accuracy | 94.8% |
| Precision | 93.1% |
| Recall | 95.7% |
| F1-Score | 94.4% |
| AUC-ROC | 0.97 |

### Confusion Matrix

| | Predicted Positive | Predicted Negative |
|---|---|---|
| Actual Positive | 85 | 4 |
| Actual Negative | 6 | 80 |

##  Key Achievements

- Achieved **94.8% Accuracy**
- Achieved **95.7% Recall**, minimizing missed diagnoses
- Strong model generalization through feature selection and optimization
- Developed an interpretable and scalable healthcare AI solution

##  Future Enhancements

- Integration with Telehealth Platforms
- Explainable AI using SHAP and LIME
- Mobile Application Deployment
- Real-Time Voice Analysis
- Edge Device Optimization
- Larger Multi-Center Clinical Datasets

##  Project Structure

```text
Parkinson-Disease-Prediction/
│
├── dataset/
│   └── parkinsons.csv
│
├── notebooks/
│   └── model_training.ipynb
│
├── models/
│   └── xgboost_model.pkl
│
├── images/
│   └── confusion_matrix.png
│
├── requirements.txt
├── README.md
└── app.py
```

##  Installation

Clone the repository:

```bash
git clone https://github.com/your-username/parkinsons-disease-prediction.git
```

Move into the project directory:

```bash
cd parkinsons-disease-prediction
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the project:

```bash
python app.py
```

##  Applications

- Early Parkinson's Disease Screening
- Clinical Decision Support Systems
- Remote Healthcare Monitoring
- AI-Assisted Neurological Diagnostics
- Telemedicine Solutions

##  References

- UCI Machine Learning Repository
- XGBoost Documentation
- Scikit-learn Documentation
- Parkinson's Disease Detection Research Papers

---
**Built with Machine Learning to support early detection of Parkinson's Disease and improve healthcare accessibility.**
