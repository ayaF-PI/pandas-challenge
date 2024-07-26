
# Pandas Challenge 

## Overview
This project aims to analyze school and standardized test data using Pandas in Python. As the Chief Data Scientist for your city's school district, you will help the school board and mayor make strategic decisions regarding future school budgets and priorities by analyzing district-wide standardized test results. The task involves aggregating the data to showcase trends in school performance.

## Background
You have been tasked with analyzing the district-wide standardized test results to help the school board and mayor make strategic decisions regarding future school budgets and priorities. You'll be given access to every student's math and reading scores, as well as various information on the schools they attend. Your task is to aggregate the data to showcase obvious trends in school performance.

## Files
- `PyCitySchools.ipynb`: The Jupyter notebook containing the analysis code.
- `Resources/schools_complete.csv`: The dataset containing information about the schools.
- `Resources/students_complete.csv`: The dataset containing information about the students.

## Instructions

### District Summary
Perform the necessary calculations and create a high-level snapshot of the district's key metrics:
- Total number of unique schools
- Total students
- Total budget
- Average math score
- Average reading score
- % passing math (the percentage of students who passed math)
- % passing reading (the percentage of students who passed reading)
- % overall passing (the percentage of students who passed math AND reading)

### School Summary
Perform the necessary calculations and create a DataFrame that summarizes key metrics about each school:
- School name
- School type
- Total students
- Total school budget
- Per student budget
- Average math score
- Average reading score
- % passing math (the percentage of students who passed math)
- % passing reading (the percentage of students who passed reading)
- % overall passing (the percentage of students who passed math AND reading)

### Highest-Performing Schools by Percentage of Overall Passing
- Sort the schools by % Overall Passing in descending order
- Save the results to a DataFrame called `top_schools`
- Display the first 5 rows

### Lowest-Performing Schools by Percentage of Overall Passing
- Sort the schools by % Overall Passing in ascending order
- Save the results to a DataFrame called `bottom_schools`
- Display the first 5 rows

### Math Scores by Grade
- Use the code provided to separate the data by grade
- Group by `school_name` and take the mean of each
- Use the code to select only the `math_score`
- Combine each of the scores above into single DataFrame called `math_scores_by_grade`

### Reading Scores by Grade
- Use the code provided to separate the data by grade
- Group by `school_name` and take the mean of each
- Use the code to select only the `reading_score`
- Combine each of the scores above into single DataFrame called `reading_scores_by_grade`

### Scores by School Spending
- Use `pd.cut` with the provided code to bin the data by the spending ranges
- Use the code provided to calculate the averages
- Create the `spending_summary` DataFrame using the binned and averaged spending data

### Scores by School Size
- Use `pd.cut` with the provided code to bin the data by the school sizes
- Use the code provided to calculate the averages
- Create the `size_summary` DataFrame using the binned and averaged size data

### Scores by School Type
- Group the `per_school_summary` DataFrame by `School Type` and average the results
- Use the code provided to select the new column data
- Create a new DataFrame called `type_summary` that uses the new column data

## Analysis

### Observable Trends
1. **Trend 1: School Spending and Student Performance**
   - Schools with higher spending per student tend to have better overall performance in both math and reading. This suggests that increased funding may contribute positively to student achievement.

2. **Trend 2: School Size and Performance**
   - Smaller schools generally show higher passing percentages compared to larger schools. This might indicate that smaller student bodies allow for more personalized attention and better educational outcomes.

### Summary of Analysis
The analysis of the school district's data reveals significant trends in how various factors such as school size, type, and spending impact student performance. Schools with higher budgets per student and smaller student bodies tend to perform better. These insights can inform decisions on resource allocation and strategic initiatives to improve education quality.

