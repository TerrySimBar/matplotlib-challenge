# Matplotlib-Challenge

A pandas/matplotlib project for analyzing a study of 249 mice that were treated with 10 drug-regimens, to give preliminary insights to trends about how squamos cell carcinoma (SCC) tumor volumes changed over the study period.

## Table of Contents
#### Introduction
#### Requirements & Dependencies
#### Analysis and Results
#### Usage
#### Contributing
#### License


#### Introduction
This project uses a Jupyter Notebook (ipynb) script with pandas and matplotlib/pyplot to analyze two csv files: one that has data about mice in a study, and another that has the results of the study. The analysis yields a statistical summary of the tumor volumes for each drug regimen. There is also a delineated discussion about some limitations of the study and key calculations, to make a prleiminary conclusion about how one of the drug regimens, Capomulin, fares as a promising treatment for SCC. Results and summaries are visualized in-line, consistent with ipynb files. 


#### Requirements & Dependencies
Python (version 3.10.9)
Pandas (version: 2.0.3)
Matplotlib (3.7.1.)


#### Analysis
Two datasets were provided as csv files: 
- Mouse data with columns: "Mouse ID","Drug Regimen","Sex","Age_months", and "Weight (g)".
- Study results with columns: Mouse ID,Timepoint,Tumor Volume (mm3), and Metastatic Sites. 
The following results were generated:
##### 1. Merged Data 
The data tables were merged left on "Mouse ID".
###### Output
<img src = "/images/merged_data_screenshot.png" alt="merged_data_screenshot" width="600"/>

---
##### 2. Total Number of Mice 
The total number of mice  in the study was calculated.
###### Output
<img src = "/images/mice_in_study_screenshot.png" alt="mice_in_study_screenshot" width="200"/>

---
##### 3. Duplicate mouse
A duplicated mouse was identified
###### Output
<img src = "/images/dupli_mouse_screenshot.png" alt="dupli_mouse_screenshot" width="400"/>

---
##### 4. Duplicate Rows
The duplicated mouse g989 was found to have 13 rows.
###### Output
<img src = "/images/duplicate_rows_screenshot.png" alt="duplicate_rows_screenshot" width="600"/>

---
##### 5. Clean Merged Data 
The merged data was cleaned by dropping all rows of data for the duplicated mouse g989.
###### Output
<img src = "/images/clean_merged_data_screenshot.png" alt="clean_merged_data_screenshot" width="600"/>

---
##### 6. Total Mice in Clean Data 
The merged data was cleaned by dropping all rows of data for the duplicated mouse g989.
###### Output
<img src = "/images/no_dupli_mice_in_study_screenshot.png" alt="no_dupli_mice_in_study_screenshot" width="200"/>

---
##### 7. Summary Statistics
A summary table was created to include all ten drug regimens with Mean, Median, Variance, Std Dev, and SEM of the tumor volumes treated by each drug.
###### Output
<img src = "/images/summary_stats_screenshot.png" alt="summary_stats_screenshot" width="600"/>

---
##### 8. Bar Graphs
Two identical bar graphs were generated using both pandas and pyplot to show the number of observed mouse timepoints for each drug.
###### Pandas Output
<img src = "/images/mouse_timepoints_bargraph_screenshot.png" alt="/images/mouse_timepoints_bargraph_screenshot" width="300"/>

###### Pyplot Output
<img src = "/images/pyplot_bar_screenshot.png" alt="/images/pyplot_bar_screenshot" width="300"/>

---
##### 9. Pie Charts 
Two identical pie charts were generated using both pandas and pyplot to show the distribution of the sexes of the mice in the study.
###### Pandas Output
<img src = "/images/mouse_sex_piechart_screenshot.png" alt="mouse_sex_piechart_screenshot" width="300"/>

###### Pyplot Output
<img src = "/images/mouse_sex_pie_screenshot.png" alt="mouse_sex_piechart_screenshot" width="300"/>

---
##### 10. Final Tumor Volume 
A DataFrame was created to show the tumor volume at the last timepoint for each mouse in the cleaned DataFrame. 
###### Output
<img src = "/images/final_tumor_vol_screenshot.png" alt="final_tumor_vol_screenshot" width="600"/>

---
##### 11. Potential Outliers
Potential outlier(s) were identified.
###### Output
<img src = "/images/outliers_screenshot.png" alt="outliers_screenshot" width="600"/>

---
##### 12. Multiple Box Plot
A multiple box plot was created to show the distributions of final tumor volumes for the four most promising drug regimens (Capomulin, Ramicane, Infubinol, and Ceftamin). A potential outlier is shown as red circle. 
###### Output
<img src = "/images/multi_boxplot_screenshot.png" alt="multi_boxplot_screenshot" width="600"/>

---
##### 13. Line Graph
A line graph was created to show the tumor volumes of a mouse treated with Capomulin over the study period. 
###### Output
<img src = "/images/linegraph_screenshot.png" alt="linegraph_screenshot" width="600"/>

---
##### 14. Scatter Plot
A scatter plot was created to show the relationship/correlation between mouse weight and average tumor volume. 
###### Output
<img src = "/images/scatterplot_screenshot.png" alt="scatterplot_screenshot" width="600"/>

---
##### 15. Regression Line with Correlation Coefficient
A regression line was added to the scatter plot, and the correlation coefficient is printed, to show the fit and strength of the relationship between mouse weight and average tumor volume. 
<img src = "/images/regression_screenshot.png" alt="regression_screenshot" width="600"/>


#### Usage
Here's how to use the Pymaceuticals Jupyter Notebook with pandas/pyplot script:
- ##### Ensure that the CSV files contain the specified data in the appropriate format
- Mouse data with columns: "Mouse ID","Drug Regimen","Sex","Age_months", and "Weight (g)".
- Study results with columns: Mouse ID,Timepoint,Tumor Volume (mm3), and Metastatic Sites.


- ##### Distribute the code appropriately across Jupiter Notebook cells to display the desired output

- ##### Run the code.
- The script will analyze the mouse and study data and display the specified elements in-line 

#### Contributing

Contributions to this project are highly encouraged! If you wish to contribute, please follow these guidelines:

- Fork the respective repository for the Pymaceuticals Jupyter Notebook script and clone it locally.
- Create a new branch for your feature or bug fix.
- Commit your changes with descriptive commit messages.
- Push your branch to your forked repository.
- Submit a pull request to the original repository.
- Please ensure that your code adheres to the project's coding style and conventions.


If you encounter any issues or have suggestions for improvements, please open an issue on the GitHub repository.

### License
This project is licensed under the MIT License. Feel free to use, modify, and distribute the code as per the terms of the license. 
