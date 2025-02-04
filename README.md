# **Student Loan Credit Prediction**

## **Project Overview**
This project utilizes machine learning techniques, specifically deep learning with neural networks, to predict the credit ranking of students based on financial and academic indicators. By analyzing these factors, the model can help assess student loan eligibility and creditworthiness.

## **Dataset Information**
The dataset used in this project is sourced from **student-loans.csv**.

### **Features in the Dataset**
- `payment_history` – Record of past loan payments.
- `location_parameter` – Geographical factor influencing financial opportunities.
- `stem_degree_score` – Score indicating STEM background.
- `gpa_ranking` – Academic GPA-based ranking.
- `alumni_success` – Indicator of post-graduate career success.
- `study_major_code` – Encoded representation of the major field of study.
- `time_to_completion` – Time taken to complete studies.
- `finance_workshop_score` – Score from financial literacy workshops.
- `cohort_ranking` – Rank within the graduating cohort.
- `total_loan_score` – Cumulative score representing total loan burden.
- `financial_aid_score` – Score indicating the amount of financial aid received.
- **`credit_ranking` (Target Variable)** – A classification label for student creditworthiness.

---

## **Project Workflow**
### **1. Data Preprocessing**
- Loaded dataset and explored data types.
- Checked for missing values and performed data cleaning.
- Scaled numerical features using **`StandardScaler()`**.
- Split the dataset into **training (80%)** and **testing (20%)** sets.

### **2. Building the Neural Network Model**
- Defined the input layer with **11 features**.
- Added two **hidden layers**:
  - **Layer 1**: 16 neurons, ReLU activation.
  - **Layer 2**: 8 neurons, ReLU activation.
- Used **Sigmoid activation** in the output layer for binary classification.

### **3. Model Compilation & Training**
- **Loss Function**: Binary Crossentropy
- **Optimizer**: Adam
- **Epochs**: 50
- **Performance**:
  - **Final Accuracy**: **73.5%**
  - **Final Loss**: 0.50

### **4. Model Evaluation**
- Generated **classification report** to analyze precision and recall.
- Visualized model predictions and performance metrics.

---

## **Key Results & Insights**
- The **Neural Network achieved an accuracy of 73.5%**, indicating strong predictive capability for student credit ranking.
- The **confusion matrix** shows the majority of predictions align correctly with actual rankings.
- **Feature importance analysis** suggests `payment_history`, `total_loan_score`, and `gpa_ranking` have significant impact on the model.
- **Future improvements**:
  - Experimenting with different neural network architectures (e.g., more layers, dropout regularization).
  - Testing alternative ML models like **Random Forests, Gradient Boosting, or Logistic Regression**.
  - Incorporating additional external financial data for better generalization.

---