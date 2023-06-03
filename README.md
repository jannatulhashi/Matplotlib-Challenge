# Matplotlib-Challenge
Using Matplotlib to a real-world situation and dataset.

## Background

![](Image/Data-analysis.png)

I have recently joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in developing anti-cancer medications.Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

In my role as a senior data analyst at Pymaceuticals, I have been granted access to the comprehensive dataset from their most recent animal study.This study involved 249 mice that were diagnosed with SCC tumors and subjected to various drug regimens. Over a period of 45 days, we observed and measured the progression of the tumors. The main objective of this study was to assess the efficacy of our drug of interest, Capomulin, in comparison to other treatment regimens.

The executive team has entrusted me with the responsibility of creating all the necessary tables and figures for the technical report on the clinical study. Additionally, they have requested a high-level summary of the study results.

### Instructions

This challenge is broken down into the following tasks:
- Prepare the data.
- Generate summary statistics.
- Create bar charts and pie charts.
- Calculate quartiles, find outliers, and create a box plot.
- Create a line plot and a scatter plot.
- Calculate correlation and regression.
- Submit my final analysis.

#### Prepare the Data
1: I will run the package dependency and data imports in order to proceed. Next, I will merge the **mouse_metadata** and **study_results** DataFrames into a single DataFrame.

2: After merging, I will display the count of unique mice IDs in the data. Additionally, I will check for any mouse ID that has duplicate time points. If such a mouse ID is found, I will display the data associated with it. To ensure accuracy, I will create a new DataFrame where this data is removed, resulting in a cleaned DataFrame. I will utilize this cleaned DataFrame for the subsequent steps.

3: Finally, I will display the updated count of unique mice IDs after the removal of the problematic data.

#### Generate Summary Statistics
I will create a DataFrame of summary statistics to analyze the data. Remember, there are multiple methods available to achieve the desired results, so the specific method used is less important than the outcome.

The summary statistics will include:
- A row for each drug regimen. The names of these regimens will be listed in the index column.
- A column for each of the following statistics: mean, median, variance, standard deviation, and standard error of the mean (SEM) of the tumor volume.

#### Create Bar Charts and Pie Charts
To visualize the total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study, I will generate two identical bar charts.
- For the first bar chart, I will use the Pandas **DataFrame.plot()** method.
- I will create the second bar chart using Matplotlib's **pyplot** methods.

Additionally, to visualize the distribution of female versus male mice in the study, I will generate two identical pie charts.
- For the first pie chart, I will utilize the Pandas **DataFrame.plot()** method.
- For the second pie chart, I will use Matplotlib's **pyplot** methods.

#### Calculate Quartiles, Find Outliers, and Create a Box Plot
1: To calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin, the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens I will use the following substeps:
           - Create a grouped DataFrame that displays the last (greatest) time point for each mouse. Then, merge this grouped DataFrame with the original cleaned DataFrame.
           - Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.
           - Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.
           - Determine outliers by using the upper and lower bounds, and then print the results.

2: Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlight any potential outliers in the plot by changing their color and style.

**All four box plots should be within the same figure.**

#### Create a Line Plot and a Scatter Plot
1: I will select a single mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.
2: Generate a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.

#### Calculate Correlation and Regression
1: Calculate the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen.
2: Plot the linear regression model on top of the previous scatter plot.

***References***

Data generated by MockarooLinks to an external site., LLC (2022). Realistic Data Generator.


           
           
