# Water Potability

## Table of Contents
1. Introduction
2. Import Libraries
3. Exploratory Data Analysis (EDA)
4. Data Cleaning
5. Removing Outliers
6. Splitting Data and Model Building
7. Predictive System
8. Conclusion

## 1. Introduction
The goal of this project is to determine the potability of water based on various physicochemical attributes. The dataset contains information about water samples and their respective potability status, which is either potable (1) or non-potable (0). The analysis involves data preprocessing, exploratory data analysis, model training, and evaluation.

## 2. Import Libraries
We begin by importing standard libraries for data analysis such as Pandas, NumPy, Seaborn, and Matplotlib. Additionally, we use modules from Scikit-learn for data preprocessing, model training, and evaluation. The `imblearn` library is used for handling imbalanced datasets.

## 3. Exploratory Data Analysis (EDA)
Exploratory Data Analysis helps in understanding the data distribution and identifying any patterns or anomalies. Key steps include:
- Loading the dataset and checking its structure.
- Examining summary statistics for each feature.
- Visualizing correlations between features using a heatmap.
- Analyzing the distribution of the target variable (Potability) and identifying class imbalances.

## 4. Data Cleaning
Data cleaning involves handling missing values and ensuring the dataset is ready for model training. Steps include:
- Identifying columns with missing values and filling them with appropriate statistics (mean in this case).
- Checking for duplicate rows and removing them if necessary.

## 5. Removing Outliers
Outliers can significantly affect model performance. We handle outliers using:
- Box plots to visualize outliers in different features.
- Applying the Interquartile Range (IQR) method for skewed distributions and capping technique for normally distributed features to remove or adjust outliers.

## 6. Splitting Data and Model Building
This section involves:
- Splitting the dataset into features (X) and target (y).
- Standardizing the features to ensure all have a mean of 0 and standard deviation of 1.
- Addressing class imbalance using SMOTE (Synthetic Minority Over-sampling Technique) to balance the classes.
- Splitting the data into training and testing sets.
- Training various machine learning models including Logistic Regression, Decision Tree, Random Forest, K-Nearest Neighbors (KNN), and Support Vector Machine (SVM).
- Evaluating the performance of each model using accuracy, confusion matrix, and classification reports.

## 7. Predictive System
After training and evaluating multiple models, the best-performing model is selected to build a predictive system. This system can predict the potability of new water samples based on their physicochemical attributes.

## 8. Conclusion
The project demonstrates a comprehensive approach to analyzing water potability using machine learning techniques. Key takeaways include the importance of data cleaning, handling outliers, and addressing class imbalances to improve model performance. The Random Forest classifier was observed to perform the best among the tested models, providing a robust solution for predicting water potability.
