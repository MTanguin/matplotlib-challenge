#### "Analyzing Anti-Cancer Drug Regimens for Squamous Cell Carcinoma Treatment"

Python Data Visualization | Matplotlib | Pandas | Numpy | Scipy | Statistics | 

# Background

Pymaceuticals, Inc. is a pharmaceutical company specializing in anti-cancer medications. They have conducted an animal study to screen potential treatments for squamous cell carcinoma (SCC), a common form of skin cancer. The study involved 249 mice with SCC tumors, which were treated with various drug regimens. Over a 45-day period, the development and measurement of tumor sizes were recorded. The primary objective of the study was to compare the performance of Pymaceuticals' drug of interest, Capomulin, against other treatment regimens.

As a senior data analyst at Pymaceuticals, you have been given access to the complete dataset from the animal study. Your task is to generate the necessary tables and figures for the technical report of the clinical study. Additionally, you are required to provide a top-level summary of the study results.

# Methods

To accomplish the objectives of the assignment, the following tasks are to be performed:

1. **Prepare the Data:** Merge the `mouse_metadata` and `study_results` DataFrames into a single DataFrame. Check for any duplicate mouse IDs with duplicate time points and create a cleaned DataFrame by removing such data.

2. **Generate Summary Statistics:** Create a DataFrame of summary statistics for each drug regimen. Calculate the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen.

3. **Create Bar Charts and Pie Charts:** Create bar charts to visualize the total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study. Generate pie charts to display the distribution of female and male mice in the study.

4. **Calculate Quartiles, Find Outliers, and Create a Box Plot:** Calculate the final tumor volume for each mouse across the four most promising treatment regimens (Capomulin, Ramicane, Infubinol, and Ceftamin). Calculate the quartiles and interquartile range (IQR) to identify potential outliers. Create a box plot to visualize the distribution of the final tumor volume for each treatment group, highlighting any potential outliers.

5. **Create a Line Plot and a Scatter Plot:** Select a mouse treated with Capomulin and generate a line plot of tumor volume versus time point for that specific mouse. Generate a scatter plot to depict the relationship between mouse weight and the average observed tumor volume for the entire Capomulin treatment regimen.

6. **Calculate Correlation and Regression:** Calculate the correlation coefficient and perform linear regression analysis to evaluate the relationship between mouse weight and average observed tumor volume for the Capomulin treatment regimen. Plot the linear regression model on top of the scatter plot.

7. **Submit Your Final Analysis:** Prepare and submit a comprehensive analysis report, including all the generated tables, charts, and findings from the data analysis.

By following these methods, you will gain insights into the efficacy of various treatment regimens and provide valuable information to Pymaceuticals, Inc. for further analysis and decision-making.


# Results

Total Number of Mice Per Treatment
![Total Number of Mice Per Treatment](https://github.com/MTanguin/matplotlib-challenge/assets/114210481/5e6b452b-d419-4ab3-9987-41686d9d9dc3)


Male V Female Mouse Population
![Male vs Female Mouse Population](https://github.com/MTanguin/matplotlib-challenge/assets/114210481/e2f1b633-3de3-4fb5-8ebb-74c348707a84)

Tumor Volume for each Selected Mouse
![Tumor Volume for each Selected Mouse](https://github.com/MTanguin/matplotlib-challenge/assets/114210481/1a12f844-12d7-4d6a-8f23-b6fe9b5825f5)

Capomulin Treatment of Mouse l509
![Capomulin treatment of mouse l509](https://github.com/MTanguin/matplotlib-challenge/assets/114210481/1ea92edf-245d-4d73-bbcb-aab3f5d631b2)

Mouse Weight vs Average Tumor Volume
![Mouse Weight vs Average Tumor Volume](https://github.com/MTanguin/matplotlib-challenge/assets/114210481/a9edeb85-99c9-49bd-83a2-06874ab535de)

Regression Plot of Mouse Weight vs Average Tumor Volume
![Regression Plot of Mouse Weight vs Average Tumor Volume](https://github.com/MTanguin/matplotlib-challenge/assets/114210481/8c347cf8-e007-42d3-9655-65393a4adf31)

# Analysis

Based on the data generated 230 mice were treated using drug regimen Capomulin which is the highest count, followed by Ramicane, 228; Ketapril, 188; Naftisol, 186; Zoniferol, 182;Placebo, 181; Stelasyn, 181; Ceftamin, 178; Infubinol, 178; and last is Propriva, 148. 

By removing the duplicates, the sample population of mice treated was down to 248. 
It can be observed that the mice sample population treated were 123 females (49.6%) and 125 males (50.4%)

Out of four of the most promising treatment regimens:Capomulin, Ramicane, Infubinol, and Ceftamin; 
Capomulin and Ramicane showed that they have the lowest final tumor volume(mm3) after the duration of the treatment as shown on boxplot(Tumor Volume for each Mouse).
The median of Capomulin tumors: 38.1251644. The median of Ramicane tumors is: 36.56165229 

As shown on figure 'Capomulin Treatment of Mouse l509', where a single mouse l509 was treated with drug regimen Capomulin, it divulged that the tumor size growth declines as it approach the end of the duration of treatment(45 days)

The linear correlation, also called Pearson’s Correlation Coefficient(r) between mouse weight and the average tumor volume is 0.84.
Based on Pearson's Correlation table, 0.84 is > 0.7, means there is a strong positive correlation between two variables (mouse weight and the average tumor volume). As the mouse weight changes, the average tumor volume changes. 

Relying on the regression analysis, it helped to determined how the average tumor volume influenced the weight of mice change. 
The R-squared value is 0.70, which indicates that the model closely tracks the data, wich is fairly  good. 

Source:

https://courses.bootcampspot.com/courses/2799/assignments/42947?module_item_id=802914
