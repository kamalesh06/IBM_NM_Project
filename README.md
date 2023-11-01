# IBM_NM_Project

# COVID-19 Vaccination Data Analysis

## Overview

This repository contains code and documentation for analyzing COVID-19 vaccination data. The analysis includes data preprocessing, exploratory data analysis, statistical tests, and data visualization. This README provides an overview of the project's phases and instructions for running and replicating the analysis.

## Phases

The analysis is divided into five phases:

### Phase 1: Data Preparation

1. Load the vaccination data from the provided CSV file.
2. Inspect the data's structure using `df.info()`, `df.tail()`, and `df.columns`.
3. Remove unnecessary columns ('source_name' and 'source_website') using `df.drop()`.
4. Clean and describe the data using `df.describe()`.
5. Handle missing values by filling them with zero.
6. Convert data types: 'total_vaccinations,' 'people_vaccinated,' 'people_fully_vaccinated,' 'daily_vaccinations_raw,' 'daily_vaccinations' to 'int64' and 'iso_code' to 'string.'
7. Save the preprocessed data to a new CSV file using `df.to_csv()`.

### Phase 2: Exploratory Analysis and Visualization

1. Load the preprocessed data.
2. Perform exploratory analysis and visualization using Python libraries (e.g., pandas, seaborn, matplotlib).
3. Calculate the mean, min, max, and correlations within the dataset.
4. Explore country data, including the number of unique countries.
5. Explore the minimum and maximum values of fully vaccinated people.
6. Explore the minimum and maximum dates in the dataset.
7. Visualize the number of daily vaccinations over time.
8. Visualize the distribution of total vaccinations by vaccine.
9. Visualize the relationship between total vaccinations and people vaccinated.
10. Visualize the comparison between countries and the number of fully vaccinated people.

### Phase 3: Statistical Analysis

1. Import the necessary Python libraries (pandas, numpy, scipy.stats).
2. Select the 'total_vaccinations' data and define an 'expected_mean.'
3. Perform a one-sample t-test to compare the selected data to the expected mean.
4. Print the test statistic (t) and p-value.
5. Check for statistical significance based on a chosen alpha level.
6. Calculate descriptive statistics for the 'total_vaccinations' data (mean, median, standard deviation, variance).
7. Conduct correlation analysis between numeric columns.

### Phase 4: Model Building

1. Split the data into training and testing datasets.
2. Scale the data for better model performance.
3. Choose a model (e.g., simple linear regression) based on problem formulation and dataset characteristics.
4. Fit the data to the selected model.
5. Evaluate model performance, focusing on the R-squared value.

### Phase 5: Visualization using IBM Cognos Analytics

1. Load the preprocessed dataset into IBM Cognos Analytics.
2. Create and customize visualizations using the software:
   - Visualize the number of daily vaccinations over time.
   - Visualize the distribution of total vaccinations by vaccine.
   - Visualize the relationship between total vaccinations and people vaccinated.
   - Visualize the comparison between countries and the number of fully vaccinated people.
