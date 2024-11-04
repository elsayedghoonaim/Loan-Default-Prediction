## Loan Default Prediction Project

### Project Overview

This project aims to predict loan defaults using a comprehensive dataset containing various features related to loan applications. By analyzing historical data, we aim to build a robust machine learning model that can accurately classify loans as either defaulting or non-defaulting.

### Data

The dataset comprises a large number of loan applications, each with features such as:

* **Demographic Information:** Age, income, employment type, marital status, etc.
* **Loan Details:** Loan amount, interest rate, loan term, purpose of the loan, etc.
* **Credit History:** Credit score, number of credit lines, debt-to-income ratio, etc.

### Data Exploration and Preprocessing

* **Exploratory Data Analysis (EDA):**
  - Visualize the distribution of numerical features using histograms and box plots.
  - Analyze categorical features using bar plots and frequency tables.
  - Explore relationships between features using scatter plots and correlation matrices.
* **Data Cleaning:**
  - Handle missing values by imputation or removal.
  - Address outliers using techniques like capping or flooring.
  - Encode categorical features using appropriate encoding techniques (e.g., one-hot encoding, label encoding).
* **Feature Engineering:**
  - Create new features by combining existing ones (e.g., income-to-loan-ratio).
  - Transform numerical features (e.g., log transformation, normalization).

### Model Selection and Training

We experimented with several classification algorithms to determine the most suitable model for our dataset. After careful consideration, we selected **XGBoost** as our primary model due to its strong performance and ability to handle complex relationships within the data.

### Model Evaluation

The XGBoost model was trained on the preprocessed dataset and evaluated using a stratified 10-fold cross-validation. The following performance metrics were obtained:

* **Accuracy:** 89.32%
* **Precision:** 0.90 for the non-default class, 0.59 for the default class
* **Recall:** 0.99 for the non-default class, 0.12 for the default class
* **F1-score:** 0.94 for the non-default class, 0.20 for the default class

The confusion matrix provides a detailed breakdown of the model's predictions:

|                     | Predicted Negative | Predicted Positive |
|---------------------|--------------------|--------------------|
| **Actual Negative** | 5618               | 623                |
| **Actual Positive** | 59                 | 84                 |

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.

## Author

- **Elsayed Ghonaim**
