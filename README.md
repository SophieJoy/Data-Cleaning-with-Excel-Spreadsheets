# Data-Cleaning-with-Excel-Spreadsheets

## 1. Access the data 
Data source: student-performance-data (?????)

Cleaning Tool: Microsoft Excel Spreadsheet

## 2. Identify how to clean the data
- It’s important to make sure the data is clean so that the analysis will be correct. 
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

## Conclusion
- 









