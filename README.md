# Credit Card Fraud Detection Using Anomaly Detection Models

This project demonstrates the detection of fraudulent transactions in a credit card dataset using anomaly detection techniques, specifically Isolation Forest and Local Outlier Factor (LOF). The dataset contains transactions made by credit cards in September 2013 by European cardholders, and the goal is to build a model that can accurately identify fraud cases.

## Project Overview

### 1. Exploratory Data Analysis (EDA)
- **Dataset Overview**: The dataset consists of 284,807 transactions, with 492 cases of fraud (0.172% of the data).
- **Data Cleaning**: The dataset was cleaned by removing duplicate records to ensure accurate analysis.
- **Data Visualization**: Histograms were plotted to visualize the distribution of transaction amounts and the time elapsed since the first transaction of the day. Correlation heatmaps were used to understand the relationships between different features.

### 2. Anomaly Detection Models
Two models were trained and evaluated to detect fraudulent transactions:
- **Isolation Forest**: An unsupervised learning algorithm used to detect anomalies by isolating outliers.
- **Local Outlier Factor (LOF)**: Another unsupervised method that identifies anomalies by measuring the local deviation of a data point's density relative to its neighbors.

### 3. Model Evaluation
- The dataset was split into training and testing sets using an 80-20 ratio with stratified sampling to maintain the class distribution.
- The models were evaluated using accuracy, precision, recall, and F1-score. The results showed that while both models performed similarly in terms of accuracy, the Isolation Forest model had a superior F1-score, making it the better choice for this dataset.

## Dataset
The dataset used in this project can be found on Kaggle:

[Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

## Files in the Repository
- `Credit Card Fraud Detection.ipynb`: The Jupyter notebook containing the full analysis, from EDA to model training and evaluation.
- `requirements.txt`: A file listing the Python libraries required to run the notebook.

## How to Use
1. **Clone the repository**:
    ```bash
    git clone https://github.com/sarfaraj-mohammad/Credit-Card-Fraud-Detection-Using-Machine-Learning.git
    cd Credit-Card-Fraud-Detection-Using-Machine-Learning
    ```

2. **Install necessary libraries**:
    Install all required Python libraries using the `requirements.txt` file:
    ```bash
    pip install -r requirements.txt
    ```

3. **Download the dataset**:
    Download the dataset from Kaggle using the link provided above, and place it in the repository directory.

4. **Run the Jupyter Notebook**:
    Launch the Jupyter notebook server and open `Credit Card Fraud Detection.ipynb` to run the analysis step by step.

5. **Analyze Results**:
    Review the visualizations, model performance metrics, and conclusions to understand the behavior of the models and the dataset.

## Conclusion
This project demonstrates that the Isolation Forest model, due to its high F1-score, is the best choice for detecting fraudulent transactions in this dataset. It is an effective and efficient method for anomaly detection, especially in scenarios with a highly imbalanced class distribution like credit card fraud.
