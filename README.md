# Midterm Task 2 -  Data Cleaning and Preparation using POWER QUERY
- This portfolio shows how to use Power Query for data preparation and cleansing. The dataset is made up of several connected tables, and before analysis, cleaning methods are used to enhance the consistency and quality of the data.


## Step 1 Download and Load Data
- Download the dataset (Uncleaned_DS_jobs.csv)  
- Open Excel  
- Go to Data → New Query → Open File → Text/CSV
- Click Load and then Edit using Power Query Editor
### Duplicate Raw Data
- Right-click the dataset in the Queries pane  
- Select Duplicate
### Clean Salary Data
- Select the Salary Estimate column  
- Go to Transform Menu → Extract → Text Before Delimiter  
- Type "(" and click OK  
- Create two new columns: Min Salary and Max Salary  
   - Select Salary Estimate column → Add Column Menu → Column from Examples → From Selections  
   - Type the first min salary value and press Enter (all rows will auto-fill)  
   - Rename the column to "Min Sal"  
   - Repeat the process for Max Salary  
  

## Step 2 Add Role Type Column
- Go to Add Column Menu → Custom Column  
- Rename the column to "Role Type"  
- Use this logic:  
   - If Job Title contains "Data Scientist" → Assign "Data Scientist"  
   - If Job Title contains "Data Analyst" → Assign "Data Analyst"  
   - If Job Title contains "Data Engineer" → Assign "Data Engineer"  
   - If Job Title contains "Machine Learning" → Assign "Machine Learning Engineer"  
   - Otherwise, assign "Other"  
- Change the column type to Text  
