# Sleep, Health, and Lifestyle Data Analysis

## Project Overview

This project analyzes the relationships between sleep patterns, lifestyle habits, and sleep disorders. Using a dataset of 374 individuals, we investigated how demographics and lifestyle choices influence sleep health and built a predictive model to identify sleep disorders.

## Data Processing & Feature Engineering

We performed extensive data preparation to ensure the dataset was suitable for machine learning:

* **Data Cleaning**:
* **Handling Nulls**: The `Sleep Disorder` column originally had 219 null values for healthy individuals. These were filled with the category "None" to accurately represent the data.
* **Value Standardizing**: In the `BMI Category` column, "Normal Weight" was merged into the "Normal" category to ensure consistency across the dataset.


* **Feature Engineering**:
* **Blood Pressure Splitting**: The `Blood Pressure` string (e.g., "126/83") was split into two separate numerical features: `Systolic_BP` and `Diastolic_BP`.
* **Categorical Encoding**: We used **Label Encoding** to transform categorical variables like `Gender`, `Occupation`, `BMI Category`, and the target `Sleep Disorder` into numerical formats.
* **Redundancy Removal**: The `Person ID` and the original `Blood Pressure` columns were dropped to improve model focus.



## Exploratory Data Analysis (EDA) Highlights

Before modeling, we explored the data through various visualizations:

* **Correlations**: Heatmaps were used to identify strong relationships, such as the high correlation between stress levels and heart rate.
* **Lifestyle Impact**: Bar charts and box plots were used to visualize how `Occupation` and `BMI Category` influenced `Sleep Duration`.
* **Gender Analysis**: Count plots revealed gender-specific trends in the prevalence of `Insomnia` vs. `Sleep Apnea`.

## Machine Learning & Performance Metrics

We compared multiple models, with the **Decision Tree Classifier** providing the most robust results. The data was split into **80% training** and **20% testing** sets.

### Decision Tree Performance:

* **Accuracy**: **96.00%**
* **Precision**: **96.00%**
* **Recall**: **96.00%**
* **F1-Score**: **96.00%**

The model proved highly effective at distinguishing between 'None', 'Insomnia', and 'Sleep Apnea', as evidenced by the high scores across all weighted average metrics.

## Technologies Used

* **Pandas & NumPy**: For data manipulation and cleaning.
* **Matplotlib & Seaborn**: For exploratory data visualization.
* **Scikit-learn**: For encoding, model training, and evaluation metrics.

## Team: QHEMA (Section 507-C)

* Qhamar Jahan LNU, Megha Mudigonda, Harini Gaddam, Emil George Mathew, Aditya Deepak Kaushik.
* **Mentor**: Prof. Peng Huang.
