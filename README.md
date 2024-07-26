# Pandas Challenge

## Overview
This project aims to analyze school and standardized test data using Pandas in Python. As the Chief Data Scientist for your city's school district, you will help the school board and mayor make strategic decisions regarding future school budgets and priorities by analyzing district-wide standardized test results. The task involves aggregating the data to showcase trends in school performance.

## Background
You are tasked with analyzing district-wide standardized test results to help the school board and mayor make strategic decisions regarding future school budgets and priorities. You will be given access to every student's math and reading scores, as well as various information on the schools they attend. Your goal is to aggregate the data to highlight trends in school performance.

## Files
- `PyCitySchools.ipynb`: The Jupyter notebook containing the analysis code.
- `Resources/schools_complete.csv`: Dataset containing information about the schools.
- `Resources/students_complete.csv`: Dataset containing information about the students.

## Instructions

### District Summary
Perform the necessary calculations to create a high-level snapshot of the district's key metrics:
- Total number of unique schools
- Total students
- Total budget
- Average math score
- Average reading score
- % passing math (the percentage of students who passed math)
- % passing reading (the percentage of students who passed reading)
- % overall passing (the percentage of students who passed both math and reading)

### School Summary
Create a DataFrame that summarizes key metrics about each school:
- School name
- School type
- Total students
- Total school budget
- Per student budget
- Average math score
- Average reading score
- % passing math
- % passing reading
- % overall passing

### Highest-Performing Schools
- Sort the schools by % Overall Passing in descending order
- Save the results to a DataFrame called `top_schools`
- Display the top 5 rows

### Lowest-Performing Schools
- Sort the schools by % Overall Passing in ascending order
- Save the results to a DataFrame called `bottom_schools`
- Display the bottom 5 rows

### Math Scores by Grade
- Separate the data by grade
- Group by `school_name` and calculate the mean of each `math_score`
- Combine the scores into a single DataFrame called `math_scores_by_grade`

### Reading Scores by Grade
- Separate the data by grade
- Group by `school_name` and calculate the mean of each `reading_score`
- Combine the scores into a single DataFrame called `reading_scores_by_grade`

### Scores by School Spending
- Bin the data by spending ranges using `pd.cut`
- Calculate the averages
- Create the `spending_summary` DataFrame using the binned and averaged spending data

### Scores by School Size
- Bin the data by school sizes using `pd.cut`
- Calculate the averages
- Create the `size_summary` DataFrame using the binned and averaged size data

### Scores by School Type
- Group the `per_school_summary` DataFrame by `School Type` and calculate the averages
- Create a DataFrame called `type_summary` using the new column data

## Analysis

### Observable Trends
1. **Impact of Spending**: Schools with higher spending per student tend to have better overall performance in both math and reading. This suggests that increased funding may positively contribute to student achievement.

2. **School Size**: Smaller schools generally show higher passing percentages compared to larger schools. This indicates that smaller student bodies may allow for more personalized attention and better educational outcomes.

### Written Report
#### Summary of Analysis
The analysis conducted on the school district's data has revealed critical insights into how different factors affect student performance. By examining metrics such as average scores, passing percentages, and budget allocations, we can better understand the trends and disparities across various schools.

#### Conclusions and Comparisons
1. **Impact of Spending**: Schools with higher spending per student show significantly better performance in both math and reading scores. This indicates that increased investment in school resources, teacher salaries, and student facilities can lead to improved academic outcomes.

2. **School Size**: Smaller schools generally have higher passing rates compared to larger schools. This trend suggests that smaller class sizes and a more close-knit school community may contribute to better academic support and student engagement, leading to higher success rates.

These findings provide a foundation for strategic planning and decision-making aimed at enhancing the quality of education within the district. By focusing on resource allocation and optimizing school sizes, the district can work towards ensuring equitable and high-quality education for all students.

