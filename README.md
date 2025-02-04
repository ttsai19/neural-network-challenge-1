Student Loan Credit Prediction
Project Overview

This project leverages machine learning techniques, specifically deep learning with neural networks, to predict the credit ranking of students based on various financial and academic factors. The dataset contains numerical and categorical features related to student loans, education history, and financial behavior.

By training a Neural Network model, we aim to predict whether a student has a good or bad credit ranking, which can be useful for financial institutions in assessing student loan eligibility and risk.
Dataset

The dataset used in this project is sourced from student-loans.csv.
Key Features

    payment_history: Record of past payments.
    location_parameter: Geographical factor affecting financial opportunities.
    stem_degree_score: Indicator of STEM education background.
    gpa_ranking: GPA score-based ranking.
    alumni_success: Measure of post-graduate career success.
    study_major_code: Encoded representation of the student's major.
    time_to_completion: Duration taken to complete studies.
    finance_workshop_score: Score from financial literacy workshops.
    cohort_ranking: Rank within the graduating cohort.
    total_loan_score: Cumulative score representing total loan burden.
    financial_aid_score: Score indicating financial aid received.
    credit_ranking (Target Variable): The predicted label indicating a student's creditworthiness.

Machine Learning Model

We implemented a Deep Neural Network (DNN) using TensorFlow & Keras to predict the credit ranking of students. The model was trained using a structured approach that includes feature scaling, data preprocessing, and evaluation.
Steps Followed

    Data Preprocessing:
        Removed unnecessary columns.
        Scaled numerical features using StandardScaler().
        Split the dataset into training (80%) and testing (20%) sets.

    Building the Neural Network:
        Input Layer: Accepts all numerical features.
        Hidden Layers:
            Layer 1: 16 neurons, ReLU activation.
            Layer 2: 8 neurons, ReLU activation.
        Output Layer: 1 neuron with a Sigmoid activation function (Binary classification).

    Model Compilation & Training:
        Optimizer: Adam
        Loss Function: Binary Crossentropy
        Training Epochs: 50
        Accuracy achieved: 73.5%

    Evaluation & Performance:
        Used classification_report for performance analysis.
        Generated predictions and visualized performance.

Results & Insights

    The Neural Network achieved an accuracy of 73.5%, showing strong predictive capability for credit ranking.
    The classification report highlighted areas for improvement, particularly in precision and recall for specific ranking categories.
    Future improvements could include feature engineering, hyperparameter tuning, and alternative ML models for comparison.

Future Considerations

To improve the model’s predictive power, we can:

    Introduce feature selection techniques to remove unimportant features.
    Experiment with different neural network architectures (more layers, neurons, dropout regularization).
    Test other models like Random Forests, Gradient Boosting, or Logistic Regression for comparison.
    Gather additional external financial data to enhance the model’s ability to generalize across students.