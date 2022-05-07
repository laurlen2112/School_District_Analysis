# Module 4: PyCitySchool Analysis

# *Overview*:
The initial purpose of this analysis was an evaluation of student test scores and funding data to assist the school and district in strategic decision making.  Upon completion of that analysis, it was requested that I remove the 9th grade math and reading scores for Thomas High School (THS) and re-run the  analysis based on this new data.

# *Results*: 
## [Impact to District Summary](https://github.com/laurlen2112/School_District_Analysis/blob/main/resources/district_summary_comparison.png): 
*	461 students from THS were removed from the analysis, reducing the total student count to 38,709
*	No change to the total budget
*	Comparison of the [unformatted District Summary](https://github.com/laurlen2112/School_District_Analysis/blob/main/resources/district_summary_comparison_unformatted.png)  shows a small drop in average grades and percent of passing students:
    *	estimated 0.05 drop in average math scores
    *	estimated 0.22% drop in students passing math
    *	estimated 0.02 drop in average reading scores
    *	estimated 0.14% drop in students passing reading
*	Drop in the overall passing percentage is estimated at 0.32%

## Impact to School Summary:
* Replacing the 9th grade THS students [math](https://github.com/laurlen2112/School_District_Analysis/blob/main/resources/math%20score%20comparison.png)  and [reading](https://github.com/laurlen2112/School_District_Analysis/blob/main/resources/reading%20score%20comparison.png) scores with NaN presents no impact to 9th grade scores in other schools because [average scores](https://github.com/laurlen2112/School_District_Analysis/blob/main/resources/math_reading_by%20grade_code.png) are calculated on a per school basis, per grade basis
* Replacing THS 9th grade student scores with NaN did cause a drop in [its metrics](https://github.com/laurlen2112/School_District_Analysis/blob/main/resources/Compare_THS_metrics.png); however, it did not effect THS in relation to other schools as it maintained its 2nd place status among the [top five schools](https://github.com/laurlen2112/School_District_Analysis/blob/main/resources/top_5_comparison.png)
* No changes to the [bottom five schools](https://github.com/laurlen2112/School_District_Analysis/blob/main/resources/bottom_5_comparison.png) are found

## Impact to Other Metrics:
* As illustrated by the images below, scores calculated by school spending, school size, and school type were unaffected by converting the THS 9th grade scores to NaN
   * [Scores by school spending](https://github.com/laurlen2112/School_District_Analysis/blob/main/resources/scores_by_spending.png) 
   * [Scores by school size](https://github.com/laurlen2112/School_District_Analysis/blob/main/resources/scores_by_size.png)
   * [ Scores by school type](https://github.com/laurlen2112/School_District_Analysis/blob/main/resources/scores_by%20_type.png)      
* This is likely due to the fact that those metrics were [calculated from the “per_school_summary_df” data frame](https://github.com/laurlen2112/School_District_Analysis/blob/main/resources/spending_size_type_code.png).  The percent passing reading, the percent passing math, and the overall passing percent were the [only metrics that were changed](https://github.com/laurlen2112/School_District_Analysis/blob/main/resources/THS%20_DF_COde.png).

# *Summary*
In summary, the district analysis changed by reducing the overall student count, reducing THS metrics regarding the average values of students passing math and/or reading, reducing the percentage of students passing math and/or reading, and reducing the overall percentage.  The  change to THS scores did not effect THS’ standing in the top 5 schools nor did it effect the other metrics captured in the original analysis.
