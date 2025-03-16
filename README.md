# Case-Study-EDA-Depression
Case Study: EDA Depression Survey Data

## Introduction
This notebook is a case study for the Google Data Analystics Professioanl Course at Cousera. Its purpose is to present the analytical skills I have gained through the course. As outlined in the course's Case Study Roadmap, I will follow the key steps of the data analysis process: Ask, Prepare, Process, Analyze, Share, and Act.

## Ask Phase

### Business Task: 
Identify key factors contributing to student depression and how they vary across demographic groups, to guide targeted interventions and improve mental health outcomes.

### The stakeholders:
1. University Administrators: department heads, student affairs directors.
   - Relevance: Responsible for student well-being and campus programs.
   - Understanding depression factors helps inform policies, resource allocation, and support structures.
2. Mental Health Professionals: On-campus counselors, psychologist
   - Relevance: Directly involved in student mental health
   - Using insights to tailor interventions and enhance support programs.

### Questions

1. What are the key factors most strongly associated with depression among students?

2. Which age group should be prioritized for mental health interventions?

3. Which programs could be implemented based on the results in order to   reduce depression among high-risk student groups?


### Metrics

- Chi-squared Test Results: Analyze the relationships between potential factors and depression to identify significant associations.
- Distribution of depression for each age group

## Prepare Phase:
- The *“Depression Survey/Dataset for Analysis"* was collected during an anonymous survey conducted between January and June 2023. The survey was included various cities and targeted individuals from diverse backgrounds and professions. Its aim was to provide insights into how different factors might contribute to depression risk among adults.

- This dataset is stored in Kaggle and it contains **2,556 rows and 19 columns**. Each row corresponds to an individual, while the columns capture the factors that might contribute with depression:

- *Note: All scales used in this dataset are on a 1–5 range, where 1 represents minimal and 5 represents maximum, except for CGPA, which follows a 1–10 scale.*

    1. Numerical Columns (8 factors):
       - Age: Age of the individual in years.
       - Academic Pressure: Self-reported academic pressure, on a 1-5 scale
       - Job Pressure: Self-reported job pressure, on a 1-5 scale 
       - Study Satisfaction: Satisfaction with academic studies, on a 1-5 scale
       - Job Satisfaction: Satisfaction with job, on a 1-5 scale 
       - Work/ StudyHours: Average daily study or work hours.
       - Financial Stress: Self-reported financial stress, on a 1-5 scale
       - CGPA: Cumulative Grade Point Average (CGPA), on a 1-10 scale 

    2. Categorical Columns (11 factors):
       - Name: Name of the participant
       - Gender: Gender of the individual (Male, Female).
       - City: City of residence.
       - Working Professional or Student
       - Profession: Occupation
       - Degree: Academic degrees that the individuals may hold.
       - Sleep Duration: Average sleep duration (Less than 5 hours, 5-6 hours, 6-7 hours, 7-8 hours and More than 8 hours).
       - Dietary Habits: Self-reported dietary habits (Healthy, Moderate Unhealthy).
       - Suicidal Thoughts: History of suicidal thoughts (Yes, No).
       - Family History: Family history of depression or suicide (Yes, No).
       - Depression: Current state of depression (Yes, No).
       

- Participants self-reported their responses without undergoing professional mental health assessments or diagnostic tests.

- This dataset has been released under the Creative Commons Zero (CC0) license by Suman Sharma. This licensing signifies: no copyright restrictions, free to use and no Attribution Required.

## Process Phase  

For the dataset analysis I will use R because it offers a powerful and flexible environment for statistical analysis, handling large datasets and creating insightful visualizations.

- First, clean the data by renaming column headers and ensuring that the variables have the correct data types.
- Next, filter the dataset to include only student-related data and remove unnecessary columns that are not relevant to the study.
- Then, check for missing values and duplicates to ensure data quality.
- Next, convert the gender variable to a factor in R, as this will allow R to treat it as a categorical variable.
- Finally, add a new column that indicates whether both the depression and suicidal_thoughts columns are marked as 'Yes'. Because students who report both depression and suicidal thoughts are at higher risk of self-harm or suicide. This represents a critical mental health warning sign that requires immediate attention.

To explore the code used in this analysis, refer to the "case-study-analyzing-depression-survey-data.ipynb" file.

## Results

The resulting visualizations can be found in the "Results.md" file.


