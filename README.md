# PyCitySchools with Pandas

## Overview of the school district analysis

The purpose of this analysis is to help Maria, a data scientist for a city school district, to analyze student standardized test score trends using various summary views and data cuts. These trends provide insights to the board, which dictates strategy and funding decisions. After completing an initial review of the data, concerns were raised about possible academic dishonesty within the Thomas High School (THS) 9th grade standardized test scores. The extent of the issue was not known. Because of the importance of this data and the decisions that these analyses guide, it was important to complete another pass at the summaries to exclude THS 9th grade scores. This allowed us to provide a before-and-after view, and to determine the extent of the impact of these scores on our reviews.

## Results

- How is the district summary affected?  
The impact to the district summary was minimal. Average math scores decreased 0.1 points, and average reading scores stayed the same. Passing math % decreased 0.2 percentage points (ppts), passing reading % decreased 0.1 ppts, and overall passing % decreased 0.3 ppts.  

![District Summary](/Resources/Before-After_Comparison1.PNG)

- How is the school summary affected?  
By removing all 9th grade scores and student counts, THS average math scores remained about the same and average reading scores increased by 0.1 points. Passing math % decreased by 0.1 ppts, passing reading % decreased by 0.3 ppts, and overall passing % decreased 0.3 ppts.  

![School Summary](/Resources/Before-After_Comparison2.PNG)

- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?  
THS still remains the #2 of 15 in terms of overall passing %. There are no shifts in these rankings after removing THS 9th grade scores.  

- How does replacing the ninth-grade scores affect the following:  
  - Math and reading scores by grade  
  Other than THS 9th grade scores becoming NaN, there are no changes to this view.  

![By Grade Summary](/Resources/Before-After_Comparison3.PNG)

  - Scores by school spending  
  THS has a budget of $638 per student, so it falls in the $630-$644 bucket. There are no changes to this bucket in this view.

  - Scores by school size  
  THS has 1,635 students so they fall in the Medium bucket. There are no changes to this bucket in this view.

  - Scores by school type  
  THS is a Charter school. There are no changes to this bucket in this view.

## Summary

Below are a few key takeaways that we found after replacing THS 9th grade scores with NaN’s, and conducting a before-and-after comparison.  

1. Although the concerns were well-founded given the importance of this process, our review concluded that academic misconduct was not widespread in these scores. There were some changes to the overall average passing scores and passing percentages, but none were statistically significant.
2. Thomas High School’s ranking in the top 5 schools, based on overall passing % didn’t change based on our review. It doesn’t appear that academic misconduct played a role in their ranking.
3. Overall district performance slipped slightly based on this review. % passing math, % passing reading, and % overall passing all saw a few tenths of a percentage point decline after making this change.
4. Similar declines were seen within the Thomas High School totals. % passing reading slipped more than % passing math, and % overall passing decreased 0.3 ppts due to this change.
