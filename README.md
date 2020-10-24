# School-Analysis

## Overview of Project
The school board reached out to our analysis firm to review school district test scores by various dimensions, such as size of school, budget per student, and school type. In order to analyze this data, we are making use of Jupyter Notebooks and the Python package named Pandas.

After reviewing the district test scores for Maria and the school board, we discovered that the 9th grade math and reading test scores from Thomas High School appear to have been altered. As a result, we need to go back through the data and replace the Thomas High School ninth grade test scores with NaN values. After we remove those values, we need to redo our district analysis without the Thomas High School ninth grade scores. 

## Results
### How is the district summary affected?
The District Summary included the following fields (columns):*'Total Schools', 'Total Students', 'Total Budget', 'Average Math Score','Average Reading Score', '% Passing Math', '% Passing Reading','% Overall Passing'.* Of these fields, all of the values specific to student scores changed after we removed the ninth grade test scores from Thomas High School. Specifically, the values changed from these initial values to these modified values:
| Field Name | Initial Value  | Modified Value |
| --- | --- |--- |
|**Average Math Score** | 79% |78.9%|
|**Average Reading Score**| 81.9% | 81.9% |
|**% Passing Math**| 75% | 74.8% |
|**% Passing Reading**| 85.8% |85.7%|
|**% Overall Passing**| 65.2% |64.9%|

### How is the school summary affected?
After removing the Thomas High School ninth grade scores, the overall scores for Thomas High School decreased slightly across all fields from the Initial analysis to the Final analysis. During analysis, there was an interim School Summary table with significantly lower values. This was caused by erroneously dividing the variables *per_student_passing_math, per_student_passing_reading, and per_passing_math_reading* by a count of the entire student body of Thomas High School (1635) rather than a count of 10th-12th graders (1174).
| Field Name | Initial Value  | Interim Value | Final Value |
| --- | --- | --- | --- |
|**Average Math Score** | 83.42% | 83.35% |83.35%|
|**Average Reading Score**| 83.85% | 83.9% | 83.9% |
|**% Passing Math**| 93.27% | 66.91% |93.19% |
|**% Passing Reading**| 97.31% | 69.66% |97.02%|
|**% Overall Passing**| 90.95% | 65.08% |90.63%|

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
As the previous table showed, the overall passing percentage dropped from an initial value of 90.95% to a final value of 90.63%. This reduction of .32% did not change the overall rank of Thomas High School compared to the other High Schools in the district, remaining in second place.
| Top Five Schools | Initial Rank | Final Rank | % Overall Passing |
| --- | --- | --- | --- |
|**Cabrera High School** | 1 | 1 |91.33%|
|**Thomas High School**| 2 | 2 | 90.63% |
|**Griffin High School**| 3 | 3 |90.6% |
|**Wilson High School**| 4 | 4 |90.58%|
|**Pena High School**| 5 | 5 |90.54%|

### How does replacing the ninth-grade scores affect the following:
#### Math and reading scores by grade

#### Scores by school spending

#### Scores by school size

#### Scores by school type

## Summary


```py
    
```

