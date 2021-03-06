# School_District_Analysis

## Overview
This analysis shows trends in school performance by looking at funding and standardized test scores. It will be used by the school board and superintendant to make decisions regarding budgets and priorities.

*** There is evidence of academic dishonesty from Thomas High School. 9th grade test scores have been removed from this analysis and excluded in calculating averages to uphold state testing standards. ***

This analysis analysis includes: 

- A high-level snapshot of the district's key metrics, presented in a table format
- An overview of the key metrics for each school, presented in a table format
- Tables presenting each of the following metrics:
  - Top 5 and bottom 5 performing schools, based on the overall passing rate
  - The average math score received by students in each grade level at each school
  - The average reading score received by students in each grade level at each school
  - School performance based on the budget per student
  - School performance based on the school size 
  - School performance based on the type of school

## Results
Below is how excluding the 9th grade data from Thomas High School effects the results for the entire district. Only test scores were excluded. No changes would be made to the total students or budget. 


### District Summary

![District_Summary.png](https://github.com/Brandonkish1/School_District_Analysis/blob/main/Resources/District_Summary.png)

- Changes to Data:
  - Average Math Score: Decrease of 0.1%
  - Average Reading Score: No Change
  - % Passing Math: Decrease of 0.2%
  - % Passing Reading: Decrease of 0.1%
  - % Overall Passing: Decrease of 0.3%

### School Summary

![School_Summary.png](https://github.com/Brandonkish1/School_District_Analysis/blob/main/Resources/School_Summary.png)

- Thomas High School's overall passing ranking didn't change. It still has the second highest % of Overall Passing students

### Effect of Thomas High School Performance Relative to Other Schools

![Top5_Schools.png](https://github.com/Brandonkish1/School_District_Analysis/blob/main/Resources/Top5_Schools.png)

- Only the test score data for Thomas High School will change. All other data will stay the same.


### Math and Reading Scores by Grade

#### Math

![Math_by_Grade.png](https://github.com/Brandonkish1/School_District_Analysis/blob/main/Resources/Math_by_Grade.png)

- Changes to Data:
  - 9th Grade: Data removed so data frame shows nan
  - 10th Grade: No changes to data. Only 9th grade test scores were removed
  - 11th Grade: No changes to data. Only 9th grade test scores were removed
  - 12th Grade: No changes to data. Only 9th grade test scores were removed

#### Reading

![Reading_By_Grade.png](https://github.com/Brandonkish1/School_District_Analysis/blob/main/Resources/Reading_By_Grade.png)

- Changes to Data:
  - 9th Grade: Data removed so data frame shows nan
  - 10th Grade: No changes to data. Only 9th grade test scores were removed
  - 11th Grade: No changes to data. Only 9th grade test scores were removed
  - 12th Grade: No changes to data. Only 9th grade test scores were removed


### Scores by School Spending

![Scores_by_Spending.png](https://github.com/Brandonkish1/School_District_Analysis/blob/main/Resources/Scores_by_Spending.png)

- Changes to Data: The image before and after look the same. The only number that might have changed was the row for <$584/student, because Thomas High School spent $630/student. No change is shown because there was only a small change in the test scores for Thomas High School and they are not reflected when rounding.


### Scores by School Size

![Scores_by_Size.png](https://github.com/Brandonkish1/School_District_Analysis/blob/main/Resources/Scores_by_Size.png)

- Changes to Data: Thomas High School is a Medium School. The only place for potential changes will be in the medium school row. No change is shown because there was only a small change in the test scores for Thomas High School and they are not reflected when rounding.

### Scores by School Type

![Scores_by_Type.png](https://github.com/Brandonkish1/School_District_Analysis/blob/main/Resources/Scores_by_Type.png)

- Changes to Data: Thomas High School is a Charter School. The only place for potential changes will be in the charter school row. No change is shown because there was only a small change in the test scores for Thomas High School and they are not reflected when rounding.

## Summary

Some of the changes to the code to exclude Thomas High School 9th grade test scores are below.

- Thomas High School 9th grade test scores were replaced with Null values
- When summarizing test scores for the whole district a new student total that excluded the Thomas High School 9th graders had to be used.
- Using the original total would have driven all of the percentages down.
- New test score info had to be calculated for Thomas High School and added to the per_school_summary_df
