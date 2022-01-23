# School District Analysis

## Overview of School District Analysis
The State Board of Education requests that the city school district prepare all stardardized test data for analysis. Data will be analyzed to provide insight about performance trends and patterns to inform decisions at the school and district level. Results will assist school board and superintendants in decisions regarding school budgets and priorities. In particular, the board is interested in relationships between student funding and standardized test scores.

The following metrics were requested:

1. The district summary
2. The school summary
3. The top 5 performing schools, based on the overall passing rate
4. The bottom 5 performing schools, based on the overall passing rate
5. The average math score for each grade level from each school
6. The average reading score for each grade level from each school
7. The scores by school spending per student
8. The scores by school size
9. The scores by school type


Additionally, the school board noted evidence in student score spreadsheets indicate that grades for 9th graders at Thomas High School have been altered. As such, math and reading grades for Thomas High School 9th graders are replaced with NaNs for the analysis.

## School District Analysis Results
Using bulleted lists and images of DataFrames as support, address the following questions.

### District Summary
How is the district summary affected?
<figcaption><i>Fig 1. District Summary</i></figcaption>

![Fig 1. District Summary](https://github.com/InRegards2Pluto/School_District_Analysis/blob/21835b7fd2a862fd8e048fb23bb6b2e8c4464453/Resources/district_summary_df_initial.png)

<figcaption><i>Fig 2. District Summary (THS Replaced)</i></figcaption>

![Fig 2. District Summary (THS Replaced)](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/district_summary_df_fixed.png)

### School Summary
How is the school summary affected?
<figcaption><i>Fig 3. School Summary</i></figcaption>

![Fig 3. School Summary](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_summary_initial.png)

<figcaption><i>Fig 4. School Summary (THS Replaced)</i></figcaption>

![Fig 4. School Summary (THS Replaced)](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_spending_range_fixed.png)

How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

### Scores by Grade
How does replacing the ninth-grade scores affect the following:
Math and reading scores by grade
<figcaption><i>Fig 5. Math Scores by Grade</i></figcaption>

![Fig 5. Math Scores by Grade](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_per_grade_math_initial.png)

<figcaption><i>Fig 6. Math Scores by Grade (THS Replaced)</i></figcaption>

![Fig 6. Math Scores by Grade (THS Replaced)](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_per_grade_math_fixed.png)
Scores by school spending

<figcaption><i>Fig 7. Reading Scores by Grade</i></figcaption>

![Fig 7. Reading Scores by Grade](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_per_grade_reading_initial.png)

<figcaption><i>Fig 8. Reading Scores by Grade (THS Replaced)</i></figcaption>

![Fig 8. Reading Scores by Grade (THS Replaced)](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_per_grade_reading_fixed.png)

### Scores by School Spending
Scores by school spending
<figcaption><i>Fig 9. Scores by School Spending</i></figcaption>

![Fig 9. Scores by School Spending](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_spending_range_initial.png)

<figcaption><i>Fig 10. Scores by School Spending (THS Replaced)</i></figcaption>

![Fig 10. Scores by School Spending (THS Replaced)](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_spending_range_fixed.png)

### Scores by School Size
Scores by school size
<figcaption><i>Fig 11. Scores by School Size</i></figcaption>

![Fig 11.Scores by School Size](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_size_initial.png)

<figcaption><i>Fig 12. Scores by School Size (THS Replaced)</i></figcaption>

![Fig 12. Scores by School Size (THS Replaced)](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_size_fixed.png)

### Scores by School Type
Scores by school type
<figcaption><i>Fig 13. Scores by School Type</i></figcaption>

![Fig 13. Scores by School Type](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_type_initial.png)

<figcaption><i>Fig 14. Scores by School Type (THS Replaced)</i></figcaption>

![Fig 14. Scores by School Type (THS Replaced)](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_type_fixed.png)

## School District Analysis Summary
Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

## Resources
- Data Source: 
  - [schools_complete.csv](Resources\schools_complete.csv).
  - [students_complete.csv](Resources\students_complete.csv)
- Software: Jupyter Notebook