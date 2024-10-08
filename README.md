# Assignment Overview
You are going to work on the '5G-Energy consumption' dataset that was provided by the  international telecommunication union (ITU) in 2023 as part of a global challenge or competition for data scientists all over the world to solve the 5G energy consumption modelling using machine learning techniques.

link to the website: https://www.itu.int/en/Pages/default.aspx

Checkpoint problematic : Network operational expenditure (OPEX) already accounts for around 25 percent of the total telecom operator’s cost, and 90 percent of it is spent on large energy bills. More than 70 percent of this energy is estimated to be consumed by the radio access network (RAN), particularly by the base stations (BSs). Thus, the objective is to build and train a ML model to estimate the energy consumed by different 5G base stations taking into consideration the impact of various engineering configurations, traffic conditions, and energy-saving methods.

Dataset description : This dataset is derived from the original copy and simplified for learning purposes. It includes cell-level traffic statistics of 4G/5G sites collected on different days.

---

# Instructions

Import you data and perform basic data exploration phase

1. Display general information about the dataset

        Create a pandas profiling reports to gain insights into  the dataset
        Handle Missing and corrupted values
        Remove duplicates, if they exist
        Handle outliers, if they exist
        Encode categorical features
2.  Select your target variable and the features

3.  Split your dataset to training and test sets

4.  Based on your data exploration phase select a ML regression  algorithm and train it on the training set

5. Assess your model performance on the test set using relevant evaluation metrics

6. Discuss with your cohort alternative ways to improve your model performance

---

## Libraries Used

The following libraries are used in this project:

- **pandas**: For data manipulation and analysis.
- **numpy**: For numerical computations.
- **matplotlib**: For visualizations.
- **seaborn**: For advanced statistical plots.
- **scikit-learn**: For machine learning models and preprocessing.




# Outcome

Mean Squared Error (MSE): 28.222636311295354

Root Mean Squared Error (RMSE): 5.312498123415702

R-squared (R²): 0.8513081801595679

## Interpretation

I had initially used the linear regression model to predict the nenergy consumption but random forest had a better performance and thus it is the model that I will go with.

With an R-squared of 48% the linear regression model was only able to explain 48% of the variability of the energy consumption and that is very poor performance.

The random forest regression showed and R-squared of 85%. This means that 85 % of the variability in energy consumption is explained by the model. This is a strong indication that the model is capturing the relationships between the features and energy consumption quite well. These results show that the Random Forest Regressor model is performing much better than the linear regression model I had.