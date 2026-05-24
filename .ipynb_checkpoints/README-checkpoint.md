# Real Estate Tweet Analysis Using Feature Importance

## Project Overview

This project analyzes a real estate-related Twitter dataset to identify the most important text features associated with user-reported locations. Rather than focusing on maximizing prediction accuracy, the primary objective is to determine which words and phrases contribute most strongly to location prediction.

The dataset contains tweets related to real estate, property investment, housing advertisements, and property sales, along with user-reported location information.

A Logistic Regression model combined with TF-IDF vectorization was used to transform tweet text into numerical features and evaluate feature importance.

---

## Research Question

Which words and phrases are most important for predicting user-reported locations in a real estate-related Twitter dataset?

---

## Dataset Description

The dataset contains:

- Tweet text
- User-reported location
- Record identifier

### Dataset Summary

| Metric | Value |
|----------|----------|
| Total Records | 259,560 |
| Total Features | 3 |
| Missing Locations | 58,162 |
| Records After Cleaning | 96 |
| Number of Location Classes | 5 |

The final dataset was filtered to retain the five most common user-reported locations.

---

## Project Structure

### Part 1: Problem Statement

Defined the research objective and project scope.

### Part 2: Data Understanding

Performed exploratory analysis, including:

- Dataset dimensions
- Data types
- Missing values
- Duplicate detection
- Location distribution

### Part 3: Data Preparation

Prepared the data by:

- Removing unnecessary columns
- Handling missing values
- Standardizing location labels
- Removing duplicate tweet texts
- Selecting the most frequent locations

### Part 4: Model Development

Built a text classification pipeline using:

- TF-IDF Vectorization
- Logistic Regression

The dataset was split into training and testing sets before model training.

### Part 5: Feature Importance Analysis

Extracted and ranked important text features using Logistic Regression coefficients.

This section represents the primary focus of the project.

### Part 6: Discussion and Interpretation

Interpreted the most influential features and their relationship to different geographic locations.

### Part 7: Conclusion

Summarized key findings and project outcomes.

---

## Technologies Used

- Python
- JupyterLab
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## Machine Learning Approach

### Text Vectorization

TF-IDF (Term Frequency-Inverse Document Frequency) was used to convert tweet text into numerical features.

### Classification Model

Logistic Regression was selected because:

- It is simple and interpretable
- It performs well on text classification tasks
- Model coefficients can be directly used for feature importance analysis

---

## Model Performance

| Metric | Value |
|----------|----------|
| Accuracy | 66.7% |

Although predictive performance was not the primary objective, the model achieved reasonable classification performance while providing interpretable feature importance scores.

---

## Top Important Features

The most influential features identified by the model included:

| Feature | Importance |
|----------|----------|
| شقة | 0.359 |
| شقة_للبيع | 0.285 |
| شقة_للبيع شقة | 0.285 |
| أن | 0.276 |
| شقق | 0.267 |
| مشروع | 0.261 |
| الخصائص_للبيع | 0.258 |
| من | 0.257 |
| مطبخ | 0.247 |
| شقق_للبيع شقق | 0.246 |

These features demonstrate that apartment listings, property advertisements, housing characteristics, and city-specific terminology play a significant role in location prediction.

---

## Key Findings

- Property-related words were the strongest predictors of location.
- Different regions exhibited distinct advertising and marketing language.
- Housing specification terms such as rooms, kitchens, and living areas were especially important for Saudi Arabian locations.
- Investment-related terminology was more common in Turkish locations.
- Logistic Regression coefficients provided a clear and interpretable measure of feature importance.

---

## Future Improvements

Potential enhancements include:

- Larger and more diverse datasets
- Advanced text preprocessing
- Arabic-specific natural language processing techniques
- Alternative machine learning models
- Explainable AI methods such as SHAP or LIME

---

## Author

This project was completed as a feature importance analysis study using machine learning techniques for text classification and interpretation.