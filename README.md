# Youth Tobacco Survey Data Analysis

This repository contains a Jupyter Notebook for analyzing the Youth Tobacco Survey (YTS) data.  The notebook explores trends in tobacco use among youth, identifies potential risk factors, and provides visualizations to understand the data.

## Project Goal

The primary goal of this project is to analyze the YTS data to understand patterns of tobacco use among youth, focusing on demographic trends, risk factors, and changes over time. The data set spans two decades and provides insights into the prevalence of different types of tobacco use, including cigarette smoking, smokeless tobacco use and cessation efforts.

## Data Source

The data used in this project is the Youth Tobacco Survey (YTS) dataset.  This dataset is publicly available.


## Data Description

The YTS dataset includes comprehensive information about tobacco use, exposure to tobacco smoke, cessation attempts, school curricula, and related factors.  Key attributes include:

* **Demographics:** Year, location (state/territory), gender, race/ethnicity, age, education level
* **Tobacco Use:** Type of tobacco product used (cigarettes, smokeless tobacco, etc.), current user status, quit attempts
* **Survey Measures:** Data values, confidence limits, sample size, etc.
* **GeoLocation:** Geographic location of surveyed students.

## Analysis Steps

The analysis in the Jupyter notebook follows these general steps:

1. **Data Loading and Preprocessing:** The notebook loads the CSV data from Google Drive, handles missing values, converts datatypes, and addresses outliers.


2. **Exploratory Data Analysis (EDA):** Descriptive statistics, frequency distributions, and visualizations (histograms, box plots, bar charts, pie charts) are used to explore the data and understand the relationship between different attributes. 

3. **Trend Analysis:** Time-series analysis of tobacco use trends over the years is conducted.

4. **Demographic Analysis:** The analysis investigates the relationship between tobacco use and demographic factors.

5. **Data Visualization:** Interactive visualizations are created to present the findings clearly.

## Technologies Used

* **Python:** The core programming language for data analysis and visualization.
* **Pandas:**  For data manipulation and analysis.
* **NumPy:** For numerical operations.
* **Seaborn & Matplotlib:** For data visualization.
* **Google Colab:** The development environment (Jupyter Notebook).

## Getting Started


1. **Clone the Repository:** Clone this repository to your local machine.
2. **Google Drive Setup:**  Upload the YTS dataset to your Google Drive. The script assumes the file is named `Youth_Tobacco_Survey__YTS__Data.csv` and is located in your MyDrive folder. 
3. **Run the Notebook:** Open the Jupyter Notebook and execute the code cells.  You will need to authorize the notebook to access your Google Drive in order to read in the data.



## Future Work

Potential extensions of this project include:

* More sophisticated statistical modeling to predict tobacco use.
* Machine learning techniques to identify risk factors.
* Development of interactive dashboards for visualizing the results.

## Contributing

Contributions are welcome!  Feel free to open issues or submit pull requests.
