# Matplotlib-challenge
_**Download the raw excel data to help you get started:**_



**This assignment is broken down into the following tasks:**

1) Prepare the data.
2) Generate summary statistics.
3) Create bar charts and pie charts.
4) Calculate quartiles, find outliers, and create a box plot.
5) Create a line plot and a scatter plot.
6) Calculate correlation and regression.
7) Submit your final analysis.

**Prepare the Data**
Run the provided package dependency and data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.

Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned DataFrame for the remaining steps.

Display the updated number of unique mice IDs.

**Generate Summary Statistics**
Create two summary statistics DataFrames:

For the first DataFrame, use the groupby method to generate the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen. This should result in five unique Series objects. Combine these objects into a single summary statistics DataFrame.

For the second DataFrame, use the agg method to produce the same summary statistics table by using a single line of code.

**Create Bar Charts and Pie Charts**
Generate two bar charts. Both charts should be identical and show the total number of time points for all mice tested for each drug regimen throughout the study.

Create the first bar chart with the Pandas DataFrame.plot() method.

Create the second bar chart with Matplotlib's pyplot methods.

Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.

Create the first pie chart with the Pandas DataFrame.plot() method.

Create the second pie chart with Matplotlib's pyplot methods.

**Calculate Quartiles, Find Outliers, and Create a Box Plot**
Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:

Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.

Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.

Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.

Determine outliers by using the upper and lower bounds, and then print the results.

Using Matplotlib, generate a box plot of the final tumor volume for all four treatment regimens. Highlight any potential outliers in the plot by changing their color and style.

**Create a Line Plot and a Scatter Plot**
Select a mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.

Generate a scatter plot of tumor volume versus mouse weight for the Capomulin treatment regimen.

**Calculate Correlation and Regression**
Calculate the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment.

Plot the linear regression model on top of the previous scatter plot.
