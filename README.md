# 📧 Email Spam Classification Project

## 📌 Project Overview
This project focuses on the classification of emails into spam and not-spam categories using a dataset comprised of 5172 emails. Utilizing the power of machine learning and data analysis, we dive deep into a CSV dataset that contains detailed information for each email, including the presence of the 3000 most common words, enabling a comprehensive approach to spam detection.

## 📊 Dataset Description

### Introduction
The dataset is a meticulously curated collection of email data, designed specifically for the task of spam classification. It encompasses a diverse range of emails, randomly selected to ensure a broad representation of potential email types one might encounter.

### Composition
- **Total Emails:** `5172`
- **Columns:** `3002`
  - **Email Name:** The first column represents the email identifier, anonymized to safeguard privacy.
  - **Word Columns:** The following 3000 columns correspond to the most common words found in the email collection, focusing solely on meaningful text data.
  - **Labels:** The final column contains labels for each email, with `1` indicating spam and `0` representing not-spam.

### Data Representation
Each row in the CSV file corresponds to a single email, with columns detailing the frequency of each of the 3000 listed words. This structured data approach enables a detailed analysis of text characteristics that distinguish spam emails from legitimate ones.

## 🔍 Analysis

The `SpamEmail.ipynb` Jupyter notebook takes you through a series of data preprocessing, exploratory data analysis (EDA), and machine learning models to classify emails accurately. From initial data cleaning to the final model evaluation, the notebook provides a comprehensive understanding of the methodology and findings.

### 📝 Pandas Queries in the Analysis
Extensive use of pandas for data manipulation and analysis highlights the project's analytical backbone. Key operations include:

- **🔢 Loading the Dataset:** Prepares the email dataset for analysis.
- **🔍 Displaying DataFrame Column Titles:** Offers insights into the dataset's structure.
- **📈 Identifying 20 Most Frequent Words:** Uncovers the top words prevalent across emails.
- **📊 DataSet Overview:** Provides statistical summaries of the dataset.
- **📉 Visualization of Top 20 Most Frequent Words:** Employs bar charts for a visual representation of word frequencies.
- **🔝 Showing Top 15 Records:** Gives an initial glimpse into the dataset.
- **🔚 Showing Bottom 15 Records:** Offers insights into the dataset's tail.
- **📐 Finding the Shape of the Data:** Reveals the dataset's dimensions.
- **🚫 Identifying Columns with Null Values:** Aids in understanding data completeness.
- **🔄 Forward Filling Null Values:** Addresses missing values for data integrity.
- **🔎 Filtering Data for Spam Emails (100 to 200):** Focuses analysis on a subset of spam emails.
- **👓 Filtering Based on 'the' Count and Grouping by Prediction:** Refines the dataset for deeper insights into word usage patterns.

### 🤖 Machine Learning Operations

The ML component of the analysis incorporates random forest (RF) and decision tree (DT) algorithms for training and prediction. Key operations include:

- **🌳 Training Models:** Utilizes random forest and decision tree algorithms for model training.
- **🔍 Feature Importance Analysis:** Identifies the 50 most important features (words) for classification using RF.
- **📊 Model Evaluation:** Compares original and predicted labels using confusion matrices.
- **📉 Analysis of Misclassifications:** Identifies and analyzes misclassified emails to understand model performance.
- **🔎 Potential New Spam Words:** Identifies potential new spam words not present in the dataset.

## 📖 Citation
The dataset utilized in this project is sourced from Kaggle. For further details and to access the dataset, please refer to the [original dataset page](https://www.kaggle.com/datasets/balaka18/email-spam-classification-dataset-csv/data).

## 🚀 Conclusion and Future Work
Insights into the effectiveness of various classification algorithms in distinguishing between spam and not-spam emails conclude the project. Future work could explore more complex model architectures and incorporate additional features, such as email metadata, for improved classification accuracy.
