# Youth Tobacco Survey Data Analysis Project

This project analyzes data from the Youth Tobacco Survey (YTS), a comprehensive dataset providing insights into tobacco use among middle and high school students across the United States.  The goal is to identify trends, behaviors, and risk factors associated with tobacco use in youth.

## Project Overview

The Youth Tobacco Survey (YTS) dataset offers valuable information on youth tobacco use, covering demographic details, geographic locations, and various aspects of tobacco-related behaviors and attitudes. This analysis leverages data science techniques to uncover patterns and trends within this rich dataset.


## Data Description

The dataset includes information collected from middle school (grades 6-8) and high school (grades 9-12) students regarding:

* **Tobacco Use:**  Cigarette smoking, smokeless tobacco use, e-cigarette use, and cessation efforts.
* **Demographics:** Gender, race, age, education, and geographic location.
* **Attitudes and Knowledge:** Perceptions of tobacco use and related media influences.
* **Environmental Factors:** Exposure to environmental tobacco smoke and access to tobacco products.

**Key Attributes:**

* `YEAR`: Year of data collection.
* `LocationDesc`: Location (state or territory).
* `TopicDesc`: Specific topic related to tobacco use (e.g., "Cigarette Use (Youth)").
* `Response`: Student's responses to survey questions.
* `Gender`: Gender of the respondent.
* `Education`: Education level of the respondent.
* `GeoLocation`: Geographic coordinates.
* `High_Confidence_Limit`, `Low_Confidence_Limit`: Confidence intervals for data values.
* **Other attributes**:  Various identifiers and detailed measures related to tobacco use.


## Data Preprocessing and Cleaning

1. **Handling Missing Values:**  The 'Response' column has a substantial number of missing values. Instead of simply removing these rows, the analysis uses imputation techniques. Missing values in 'Response' were imputed based on patterns observed in the 'MeasureDesc' column, and missing values in numerical columns (e.g. `High_Confidence_Limit`, `Low_Confidence_Limit`) were imputed using median.


2. **Outlier Detection:** Box plots were used to identify outliers in numerical data, particularly in the 'High_Confidence_Limit' and 'Low_Confidence_Limit' columns, but no outlier removal was performed.


3. **Feature Selection:** Irrelevant columns (single-value columns, redundant information, those with limited predictive power) were removed to improve efficiency and focus the analysis on the most relevant variables.


4. **Data Transformation:** The 'Gender' and 'Education' attributes were analyzed. No further transformation was performed on these attributes.

## Exploratory Data Analysis (EDA)

The EDA uses a variety of visualizations and summary statistics to understand the data:

1. **Histograms:** Used to visualize distributions of numerical data like 'High_Confidence_Limit' and 'Low_Confidence_Limit'.


2. **Bar Charts:** Examine the prevalence of different tobacco use topics across different survey years, and the relationship between education level and gender.


3. **Pie Charts:** Visualizes the distribution of responses by gender.

4. **Countplots:**  Shows the relationship between 'Response' and 'Gender'.


## Results and Insights

The analysis reveals key trends in youth tobacco use, including:

* **Prevalence of different tobacco products**:  Visualizations show the changing patterns of different tobacco use in the youth.
* **Gender differences**:  The role of gender in tobacco use trends is highlighted.
* **Geographic variations**: This can be observed by analyzing `LocationDesc`
* **Temporal trends**:  Trends of tobacco use over time.


## Future Work

* **Advanced statistical modeling**:  More sophisticated machine learning methods could uncover more in-depth insights.
* **Geographic analysis**:  Explore the geographical distribution of tobacco use with more advanced geospatial data visualization and analytics.
* **Integration with additional datasets**:  Combining data from other relevant sources may provide deeper insights.

## Setup and Dependencies

* **Python Libraries:** pandas, NumPy, seaborn, matplotlib, SciPy
* **Google Colaboratory:** The code was originally developed and executed in a Google Colab environment, though it can be adapted for other environments.

