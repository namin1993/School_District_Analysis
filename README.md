# School Disctrict Analysis

## Overview
Overview of the school district analysis: Explain the purpose of this analysis.

The purpose of the school district analysis is to parse through the combined student and school data to determine which schools have:

- the highest overall performance in reading and math scores
- the relationship between the school's capita per student and their overall passing scores
- the relationship between school size and overall passing scores
- the relationship between school type and overall passing scores

We have to remove incorrect data from the 9th Grade Thomas High School class in order to recalculate all averages in test scores.

## Results
Results: Using bulleted lists and images of DataFrames as support, address the following questions.

- How is the district summary affected?
    The District summary after removing the 9th grade Thomas High School students overall math and reading scores from the data is not significantly impacted. The overall passing percentage in the district decreased by 0.1% after the removal.

- How is the school summary affected?
    The School Summary after the grading audit in the data set only affected the Thomas High School row where the percentage passing average in Math, Reading, and both subjects (Overall Passing %) greatly reduced from the 90s average to the mid-60s average.

- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
    
    After replacing all the 9th grade math and reading scores with NaN values and still keeping the total number of students, the passing percentages for Thomas High School reduced as follows:
        Passing Math % reduced from 93% to 66%
        Passing Reading % reduced from 97% to 69%
        Overall Passing % reduced from 90% to 65%

    If you recalculate the grade averages while removing the number of 9th graders attending Thomas High school, the passing percentages do not change. The actually boost their ranking from number 4 to number 2 as the highest perfomring school.

## PyCity Schools Top 5 - Original Rankings
    ![PyCity Schools Top 5 - Original Rankings](https://github.com/namin1993/School_District_Analysis/blob/e0db4e22172c5cd52f69bd725a723fa894e13c92/Resources/PyCity%20Schools%20Original%20-%20Ranking.png "PyCity Schools Top 5 - Original Rankings")

## PyCity Schools Top 5 - New Rankings
    ![PyCity Schools Top 5 - New Rankings](https://github.com/namin1993/School_District_Analysis/blob/3d99152e9d219ec4b64cb89707cd1600d1486bdb/Resources/PyCity%20Schools%20Challenge%20-%20Top%20Schools%20Ranking.png "PyCity Schools Top 5 - Challenge Rankings")

How does replacing the ninth-grade scores affect the following:
- Math and reading scores by grade
    Replacing the 9th grade scores and removing the number of 9th graders from the total student population in Thomas High School does not affect the 10th, 11th, and 12th grade math and reading scores for Thomas High School.

- Scores by school spending
    Replacing the 9th grade scores does not affect the scores by school spending since we did not recalculate the budget per student after removing the number of 9th graders within Thomas High School's student body. 

- Scores by school size
    Replacing the 9th grade scores does not affect the scores by school size since the number of 10th, 11th, and 12th graders in Thomas Hight school would still keep the total student population between 1,000 - 1,999 students.

- Scores by school type
    Replacing the 9th grade scores does not affect the scores by school type.

## Summary

After replacing the 9th grade scores as NaN values for Thomas High School, their school ranking increased by 2 places, but the overall school district analysis regarding scores based on school spending, school size, and school type remained the same since the number of 9th grade students in Thomas High School is negligible to the overall data set of all 15 different schools in the district.
