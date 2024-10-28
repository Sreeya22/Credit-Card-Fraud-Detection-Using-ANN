# Credit Card Fraud Detection (CCFD)

This project aims to detect fraudulent credit card transactions using various machine learning models. Given the imbalanced nature of the data, where legitimate transactions vastly outnumber fraudulent ones, we apply techniques like **SMOTE** (Synthetic Minority Over-sampling Technique) to balance the classes and improve model performance. We compare the performance of an Artificial Neural Network (ANN) with other algorithms (SVM, Random Forest, XGBoost) and visualize results to interpret model outcomes effectively.

## Dataset Information

- **Source**: The dataset used in this project is sourced from Kaggle.
- **Columns**:
  - `Time`, `V1` to `V28`: Anonymized features
  - `Amount`: Transaction amount
  - `Class`: Target variable (0 for legitimate transactions, 1 for fraudulent)


## Modeling Approach

1. **Data Preprocessing**:
   - Standardize the `Time` and `Amount` columns.
   - Handle missing values and remove duplicates if any.
   - Balance the data using **SMOTE** to address class imbalance.

2. **Model Building**:
   - **Artificial Neural Network (ANN)**: Built a sequential ANN model with layers tuned for fraud detection.
   - **Comparison Models**: SVM, Random Forest, and XGBoost models for comparison.

3. **Evaluation**:
   - The models are evaluated using accuracy, precision, recall, and F1-score metrics, focusing on minimizing false negatives.

## Evaluation

- **Accuracy**: Measures the overall correctness of the model.
- **Precision and Recall**: Crucial for understanding the model’s effectiveness in fraud detection.
- **Confusion Matrix**: Visualizes the model’s performance by showing true positives, false positives, true negatives, and false negatives.

## Results

### ANN Model Performance:
- **Accuracy**: 99.98%

### Visualization:
1. **Accuracy and Loss**:
   - Plots show the training and validation accuracy and loss for the ANN model over 50 epochs.

2. **Precision and Recall**:
   - Precision and recall curves provide insights into the trade-offs between false positives and false negatives.

3. **Heatmap**:
   - A heatmap of the correlation matrix helps in understanding feature relationships.

4. **Class Distribution**:
   - A bar plot visualizing the balanced class distribution after applying SMOTE.

