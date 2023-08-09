# Disaster Detection from Tweets.

# Project Overview.

In the digital age, real-time communication via social media platforms like Twitter play a vital role in distributing information about events, including disasters. However, distinguishing between tweets that truly indicate emergencies and those that use related keywords is a significant challenge. This project relates to machine learning techniques in order to automatically classify tweets as disaster-related or not. The goal is to assist disaster relief organizations and news agencies with factual and efficient information sorting.


# Dataset.

The project relies on a dataset that contains 10,000 tweets. Each tweet is manually labeled to show whether it relates to an actual disaster. This dataset serves as the foundation for training, evaluating, and fine-tuning the machine learning models.


# Code Description.

The project code consists of the following essential sections:

1. Data Loading and Preprocessing: This phase involves loading the training and testing datasets. Data checks are performed to ensure consistency, and any missing values are replaced with the 'unknown' placeholder.

2. Text Preprocessing: As an important step, this phase involves converting all text to lowercase and removing hyperlinks, HTML tags, punctuation, and words containing numbers. This transformation helps create consistent and structured text data.

3. Feature Extraction: Text data is transformed into numerical features using the TF-IDF (Term Frequency-Inverse Document Frequency) vectorization. This transformation adds value to word importance and aids in model training.

4. Model Training and Evaluation: Multiple machine learning models are employed, including Logistic Regression, Random Forest, Naive Bayes, K-Nearest Neighbors, and XGBoost. The models are evaluated using metrics like precision, recall, and F1-score.

5. Explainability with SHAP: My project incorporates SHAP (SHapley Additive exPlanations) to assess model predictions. SHAP offers insights into feature contributions, making model decisions interpretable.

6. Hyperparameter Tuning: The Random Forest classifier undergoes hyperparameter tuning with GridSearchCV. This process optimizes model parameters to improve predictive performance.

7. Predictions and Submission: The best-performing model generates predictions on the test dataset, resulting in a submission.csv file.


# Running the Project.

Follow these steps to run the project:

1. Ensure you have the necessary libraries installed.

2. Download the training and testing datasets, placing them in the script directory.

3. Execute the script `M6Proj.ipynb` using Jupyter Notebook or Jupyter Lab.


# Exploring Results and Visualizations.

The project includes exploratory data analysis (EDA). Visualizations such as histograms displaying text length distributions in training and testing data provide insights into tweet lengths. Also, target class distribution visualizations offer valuable context on disaster-related tweet prevalence.

SHAP summary plots present a visualization of the model's prediction rationales. This feature is important in understanding the model's decision-making process.


# Contributing.

Contributions to this project is encouraged and appreciated. If you encounter issues or have suggestions for improvement, please submit an issue in the project repository.


# Contact.

For inquiries, feedback, or collaboration opportunities, feel free to reach out to Deon Archary at deon.archary@elu.nl

