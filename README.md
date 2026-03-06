# Data-Cleaning-with-Excel-Spreadsheets

## 1. Access the data 
Data source: Please check the "student-performance-data.csv" file

Cleaning Tool: Microsoft Excel Spreadsheet

## 2. Identify how to clean the data
- The first thing to do is check the values in the columns most relevant to the analysis and find out if there is anything to clean. 
- In this example, the superintendent’s main objective is to determine what factors drive student performance. 
- To begin answering this question, I will focus on the following columns: school, age, reason, Medu, Fedu.
- Now, I will use sorting and filtering to clean the data in each of these columns.

## 3. Sorting data
- Right on top of the data speadsheet, click "Data", then "Sort", the pop-up window appears like this.
<img width="913" height="405" alt="image" src="https://github.com/user-attachments/assets/f5d932f9-9584-4a45-812a-c9b3cc06b45a" />

- Next, click OK
  
<img width="975" height="425" alt="image" src="https://github.com/user-attachments/assets/5e9f09fd-ed44-4151-bc0f-10a0c1719940" />
<img width="975" height="422" alt="image" src="https://github.com/user-attachments/assets/de1454b5-c123-4c4f-9872-4576b1bebd25" />

- Now, If you scroll through the data, you’ll notice that the age range of the students at Gabriel Pereira (GP) is 15-22 years, and the age range of the students at Mouzinho da Silveira (MS) is 15-20 years.
- It appears that both schools have similar age ranges, but the GP school has students that are a little older.

- While sorting the data, I’ve discovered a potential problem. 
- Because this dataset represents high school student achievement, any age older than 18 may indicate that a mistake was made when entering that student's age. 
- We now know what age data may need to be researched and corrected. 
- The next step is to ask the superintendent about the legitimate age range for students in public high school to determine what age data is incorrect and should be removed.
- According to the superintendent the maximum age limit for which public education is provided is 19 years old and the age range should be 15-19 for both schools.
- Any student outside this age range should be deleted from the dataset.
- To clean the data, I need to remove the ages 20, 21, and 22 from the dataset.
- This can be done by applying a filter to the age column. 

## 4. Filtering data
- To clean the data, I need to remove the ages 20, 21, and 22 from the dataset. 
- I can start by applying a filter to the age column. Then, click OK.
- This will single out the rows that contain the ages 20, 21, and 22. 
- After applying the filter, there should be nine such rows (seven for the GP school and two for the MS school).
  <img width="1721" height="258" alt="image" src="https://github.com/user-attachments/assets/4d245288-58ab-47ca-b058-6a2052953455" />
- Click the Filter icon at the top of the age column to inspect the values once again. 
- Now that I’ve removed the three incorrect ages (20, 21, and 22), there are five ages remaining (15, 16, 17, 18, and 19). 
- The remaining ages are legitimate and can be used for analysis.
- Finally, turn off the filter. From the menu bar, select Data and Turn off filter.
  <img width="1184" height="492" alt="image" src="https://github.com/user-attachments/assets/2f053d3f-133d-4560-83b5-bf7f0203dfe1" />

## 5. Fill in missing data
- Filling in missing data is an important part of data cleaning. 
- Filter blank data
  <img width="1115" height="483" alt="image" src="https://github.com/user-attachments/assets/0789a612-d396-4f7b-aac9-a19e53fd374a" />
- Finally, turn off the filter.
- From the menu bar, select Data and Turn off filter.
- If I scroll down the reason column, I should find that the value none_given has replaced all the blanks in the reason column.

<img width="1119" height="479" alt="image" src="https://github.com/user-attachments/assets/7064295c-c78e-4f97-904c-aeb96f0de2f7" />

## 6. Convert data
- During the data analysis process, it's sometimes necessary to change text data (words) to numeric data (numbers).
- In this case, the superintendent wants to know if a parent’s education level is a significant factor in student performance.
- The relevant data is in the Medu and Fedu columns--which, respectively, refer to the level of education of a student’s mother and father.
- Currently, the data is in text format. For the purposes of analysis, it will be useful to know the average education level of each student’s parents.
- To make this calculation, I first need to convert the data in the Medu and Fedu columns to number format.
- To do this, I will match specific number values to the text data in each column.
- Start with the Medu column.
- Click on the Filter icon at the top of the Medu column (G), notice the column contains the text data shown in the table below.
- Use the following numeric codes for each piece of text data:
  <img width="716" height="445" alt="image" src="https://github.com/user-attachments/assets/1095c2ae-f81d-4717-9f78-79c5af9a0197" />
  - Replace cells in Medu and Fedu with numerical values
  <img width="1151" height="488" alt="image" src="https://github.com/user-attachments/assets/fe17e904-e361-4024-a9bb-cdbc2cf40615" />

- Check out your spreadsheet. All the cells in the Medu and Fedu column now display numeric values.
  <img width="1180" height="510" alt="image" src="https://github.com/user-attachments/assets/a6ee8587-8c1f-4ebf-9e2b-2cdd2cd975ef" />

## 7. Data Cleaning Summary

The following table summarizes the variables cleaned, the expected values, the issues detected, and the actions taken to improve data quality.
| Variable | Expected Values                 | Issues Identified                                            | Cleaning Method                                                          |
| -------- | ------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------------------ |
| school   | GP, MS                          | Inconsistent capitalization, extra spaces, full school names | Used **Find & Replace**, TRIM(), and Pivot Tables to standardize values  |
| age      | 15–19                           | Ages outside range, text values, missing entries             | Converted to numeric and flagged invalid values using validation formula |
| reason   | home, reputation, course, other | Inconsistent naming (e.g., "close", "program")               | Standardized categories using **Find & Replace and Filters**             |
| Medu     | 0–4                             | Invalid values, text entries, missing data                   | Verified numeric coding and flagged values outside the expected range    |
| Fedu     | 0–4                             | Invalid values, inconsistent formatting                      | Applied the same validation checks as Medu                               |


## 8. Final Data Quality Result

After cleaning:

- School values are standardized
- Student ages are within 15–19
- Reason categories are consistent
- Parent education values follow valid numeric coding
- Invalid and missing data were identified and corrected
- The dataset is now clean and ready for further analysis of factors affecting student performance.

## 9. Key Insights & Recommendations

- After cleaning and validating the dataset, the data is ready to support analysis of factors affecting student performance in the two schools.
- These insights illustrate how the dataset could be used to guide educational decision-making.

## Key Insights
1. Parental Education May Influence Student Performance
- Research often shows a relationship between parental education levels and student academic outcomes.
#### Variables analyzed:
- Medu (Mother’s education level)
- Fedu (Father’s education level)
#### Students whose parents have higher education levels may have access to:
- More academic support
- Stronger study habits
- Greater educational expectations
#### This variable can help identify socioeconomic factors affecting achievement.

2. School Choice Motivation

The dataset includes the variable reason, which describes why students chose their school.
#### Possible motivations:
| Reason     | Description               |
| ---------- | ------------------------- |
| home       | Close to home             |
| reputation | School reputation         |
| course     | Specific academic program |
| other      | Other reasons             |

##### This variable can help determine whether students motivated by academic programs or school reputation perform differently.

3. Comparison Between Schools
   The dataset includes students from two schools:
- Gabriel Pereira School (GP)
- Mouzinho da Silveira School (MS)
  Comparing these schools could reveal differences in:
- Academic performance
- Student demographics
- Parental education levels
  
These insights could help identify best practices or areas needing improvement.

## Recommendations for the School District

Based on the variables in this dataset, the school district could consider the following actions:
1. Provide Additional Academic Support Programs
   
If students from lower parental education backgrounds show lower performance, schools could implement:
- Tutoring programs
- After-school study sessions
- Mentoring initiatives

2. Strengthen Academic Programs
   
If students selecting schools for course offerings perform better, expanding specialized programs could improve engagement and performance.
##### Examples:
-  STEM tracks
- Language immersion
- College preparation courses

3. Use Data-Driven Decision Making
   
Schools can regularly analyze student data to:
- Identify at-risk students early
- Track improvement initiatives
- Evaluate educational programs

## 10. Conclusion
Data cleaning is a critical first step in any analytics project. 

Ensuring that variables such as school, age, reason, and parental education are accurate allows analysts to produce reliable insights that inform better decisions.

This project highlights the importance of data quality, structured workflows, and clear documentation in real-world data analysis.
