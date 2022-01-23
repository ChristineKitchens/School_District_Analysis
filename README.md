# School District Analysis

## Overview of School District Analysis
The State Board of Education requests that the city school district prepare all stardardized test data for analysis. Data will be analyzed to provide insight about performance trends and patterns to inform decisions at the school and district level. Results will assist school board and superintendants in decisions regarding school budgets and priorities.

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


Additionally, the school board observed evidence in student score data that indicates scores for 9th graders at Thomas High School (THS) have been altered. As such, math and reading scores for THS 9th graders are replaced with NaNs for the analysis. Descriptions of how the replacement impacted metrics is included in the report. Code script from which results were derived can be found in the [jupyter notebook for the project](PyCitySchools_Challenge.ipynb).

## School District Analysis Results

### District Summary
- After replacing Thomas High School 9th grade scores with NaNs, four changes were observed in the district summary:
  - The average math score decreased by 0.1 (79.0 to 78.9)
  - The percent of students with passing math scores decreased by 0.2% (75.0% to 74.8%)
  - The percent of students with passing reading scores decreased by 0.3% (86.0% to 85.7%)
  - The overall percent of students with passing scores for both reading and math decreased by 0.1% (65.0% to 64.9%)

<Tablecaption><i>Table 1. District Summary</i></Tablecaption>

![Table 1. District Summary](https://github.com/InRegards2Pluto/School_District_Analysis/blob/21835b7fd2a862fd8e048fb23bb6b2e8c4464453/Resources/district_summary_df_initial.png)

<Tablecaption><i>Table 2. District Summary (THS Replaced)</i></Tablecaption>

![Table 2. District Summary (THS Replaced)](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/district_summary_df_fixed.png)

### School Summary
- Given that the only changes in the data occurred for Thomas High School, changes to data in the school summary table only occurred in the record associated with that school.
- Metrics such as "Total Students" and "Per Student Budget" remain unchanged. Even though scores for 9th graders were replaced with NaNs, the student records still remained, so any metric based on total student body would remain unchanged (unless related to test scores).
- For metrics related to math and reading scores, the following changes occurred after the replacement:
  - The average math score decreased by 0.07 (83.42 to 83.35)
  - The average reading score decreased by 0.05 (83.85 to 83.90)
  - The percent of students with passing math scores decreased by 0.08% (93.27% to 93.19%)
  - The percent of students with passing reading scores decreased by 0.29% (97.31% to 97.02%)
  - The overall percent of students with passing scores for both reading and math decreased by 0.32% (90.95% to 90.63%)

<Tablecaption><i>Table 3. School Summary</i></Tablecaption>

![Table 3. School Summary](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_summary_initial.png)

<Tablecaption><i>Table 4. School Summary (THS Replaced)</i></Tablecaption>

![Table 4. School Summary (THS Replaced)](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_summary_fixed.png)

### Relative Performance Across Schools
- In terms of how the replacement of the THS 9th grade scores impacted their performance relative to other schools, no observable changes were seen in ranking. Even after replacing the data and changes in THS score metrics, both the top 5 and bottom 5 performing schools (Table 4 and Table 5, respectively) remained the same. 
- Both with and without the 9th grade scores, THS ranked as the #2 performing school in the district.
  - However, it's worth noting that, across the 15 schools, the margin between rankings is slim for upper rankings. For example, when looking at the % overall passing metric, the difference between the #1 performing school (Cabrera High School) and the #5 performing school (Pena High School) was only ~0.79%. Score data for THS 9th graders prior to replacement did not deviate far from scores for grades 10-12 (see Tables 7-10). Therefore, it's not surprising that their relative ranking didn't change. However, if the original data (i.e. the data before the alleged tampering) deviated further from the other grades at THS, it's possible that those scores were low enough to pull the school out of the top 5 performing schools, even if it was only 1-2 percent lower. This may have been the driving force behind the academic dishonesty. Unfortunately, until the original, unaltered data can be located, one can only speculate.

<Tablecaption><i>Table 5. Top 5 Performing Schools Based on % Overall Passing</i></Tablecaption>

![Table 5. Top 5 Performing Schools Based on % Overall Passing (THS Replaced)](https://github.com/InRegards2Pluto/School_District_Analysis/blob/0b9c1118d85d58e0392d56149f50344f6e485de3/Resources/top_5_fixed.png)

<Tablecaption><i>Table 6. Bottom 5 Performing Schools Based on % Overall Passing (THS Replaced)</i></Tablecaption>

![Table 6. Bottom 5 Performing Schools Based on % Overall Passing (THS Replaced)](https://github.com/InRegards2Pluto/School_District_Analysis/blob/0b9c1118d85d58e0392d56149f50344f6e485de3/Resources/bottom_5_fixed.png)

### Scores by Grade
- Replacing 9th grade scores impacted scores by grade predictably. After the scores were replaced with NaNs, the 9th grade score for THS went from 83.6 for math and 83.7 for reading to have no record for either.
  
<Tablecaption><i>Table 7. Math Scores by Grade</i></Tablecaption>

![Table 7. Math Scores by Grade](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_per_grade_math_initial.png)

<Tablecaption><i>Table 8. Math Scores by Grade (THS Replaced)</i></Tablecaption>

![Table 8. Math Scores by Grade (THS Replaced)](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_per_grade_math_fixed.png)

<Tablecaption><i>Table 9. Reading Scores by Grade</i></Tablecaption>

![Table 9. Reading Scores by Grade](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_per_grade_reading_initial.png)

<Tablecaption><i>Table 10. Reading Scores by Grade (THS Replaced)</i></Tablecaption>

![Table 10. Reading Scores by Grade (THS Replaced)](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_per_grade_reading_fixed.png)

### Scores by School Spending
- Scores by school spending remained unchanged after the replacement.
- Surprisingly, data indicated that schools that spent less on students actually yielded higher scores across the board.

<Tablecaption><i>Table 11. Scores by School Spending</i></Tablecaption>

![Table 11. Scores by School Spending](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_spending_range_initial.png)

<Tablecaption><i>Table 12. Scores by School Spending (THS Replaced)</i></Tablecaption>

![Table 12. Scores by School Spending (THS Replaced)](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_spending_range_fixed.png)

### Scores by School Size
- Scores by school size remained unchanged after the replacement.
- Data indicates that smaller schools outperformed larger schools. Assuming that smaller schools also have smaller class sizes, this results lends to the notion that smaller classes are more conducive to learning than large classes. Further data is needed.

<Tablecaption><i>Table 13. Scores by School Size</i></Tablecaption>

![Table 13.Scores by School Size](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_size_initial.png)

<Tablecaption><i>Table 14. Scores by School Size (THS Replaced)</i></Tablecaption>

![Table 14. Scores by School Size (THS Replaced)](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_size_fixed.png)

### Scores by School Type
- Scores by school type remained unchanged after the replacement.
- Data overwhelmingly suggest that charter schools tend to outperform district schools. As seen in earlier sections, all top 5 performing schools are charter schools. Given that the charter schools also tended to have smaller school sizes compared to the district schools, this result is in alignment with discussions outlined in the previous section.

<Tablecaption><i>Table 15. Scores by School Type</i></Tablecaption>

![Table 15. Scores by School Type](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_type_initial.png)

<Tablecaption><i>Table 16. Scores by School Type (THS Replaced)</i></Tablecaption>

![Table 16. Scores by School Type (THS Replaced)](https://github.com/InRegards2Pluto/School_District_Analysis/blob/01632983c491c1dcbeb546bf9777767be9b3a7cf/Resources/school_type_fixed.png)

## School District Analysis Summary
- Overall, data indicates three conclusions:
  -  Charter schools outperform district schools
  -  Smaller schools outperform larger schools
  -  Schools with lower spending per student outperform schools with higher spending per student.
-  Further analysis should be conducted to understand how the metrics of school type, size, and spending interrelate with one another. For example, do charter schools perform better because they are smaller? Does the smaller school size also correlate to smaller average class size? Additional data should be requested from schools.
- Across all the requested metrics, replacing the Thomas High School 9th grade scores with NaNs impacted the following:
  - District Summary Data
    - The average math score decreased by 0.1 (79.0 to 78.9)
    - The percent of students with passing math scores decreased by 0.2% (75.0% to 74.8%)
    - The percent of students with passing reading scores decreased by 0.3% (86.0% to 85.7%)
    - The overall percent of students with passing scores for both reading and math decreased by 0.1% (65.0% to 64.9%)
  - Thomas High School Data
    - The average math score decreased by 0.07 (83.42 to 83.35)
    - The average reading score decreased by 0.05 (83.85 to 83.90)
    - The percent of students with passing math scores decreased by 0.08% (93.27% to 93.19%)
    - The percent of students with passing reading scores decreased by 0.29% (97.31% to 97.02%)
    - The overall percent of students with passing scores for both reading and math decreased by 0.32% (90.95% to 90.63%)
- Despite these various changes at both district and individual school level, more metrics remained unchanged than changed. The lack of change may have to do with the number of significant digits that various metrics were reported at, but changes would still be minimal even then.
- However, as discussed when reviewing the relative performance and ranking of the schools, the tampered data for the 9th graders did not deviate greatly from the untampered data for the 10th-12th graders. Therefore, even when replacing 9th grade data with NaNs, because 9th graders were still included in the total student count, any derivative metrics that didn't relate directly to scores were unchanged (e.g. spending per student and school size). Even metrics that did change did so minimally since the removed values were already similar to the remaining values, so mean values would not have changed greatly. It would ultimately be more informative to locate the untampered data for the THS 9th graders and then repeat the analysis.

## Resources
- Data Source: 
  - [schools_complete.csv](https://github.com/InRegards2Pluto/School_District_Analysis/blob/f7e7f9cbd7c7a0a260407ab7c05c14d766b39f29/Resources/schools_complete.csv).
  - [students_complete.csv](https://github.com/InRegards2Pluto/School_District_Analysis/blob/f7e7f9cbd7c7a0a260407ab7c05c14d766b39f29/Resources/students_complete.csv)
  - [PyCitySchools_Challenge.ipynb](PyCitySchools_Challenge.ipynb)
- Software: Jupyter Notebook
