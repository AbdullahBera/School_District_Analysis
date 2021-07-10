# Overview of the School District Analysis

## Overview of Project

In this analysis, I supported Maria to analyze data from a variety of sources in a variety of formats of student scores from standardized tests in several schools. The data I analyzed is of 39,170 students from 15 schools where I used the Jupyter Notebook in Anaconda to run my code to analyze the data. The results of this analysis are intended to provide the School Board with insights regarding school performance, school budget, and school priorities. This analysis is done under the Family Educational Rights and Privacy Act (FERPA), respecting the privacy of the students in the data.  

### Objective 

I wanted to understand how changing the math and reading scores of students in Thomas High School, a charter school, will affect the district summary, the school summary, and Thomas High School's relative performance to the other schools. The total number of 9th graders in Thomas High School is 461. The objective of this analysis is to see if these 461 students have a significant impact in changing the outcomes of Thomas High School. Furthermore, I also delivered results regarding how the change in the scores affected math and reading scores by grade, school spending, school size, and school type. With these indicators, I concluded the implications of replacing math and reading scores of students in Thomas High School with NaN's.
## Results 

In this section, I comparatively analyze the results when 9th grader math and reading scores were present and when they were replaced with NaN's.

* **How is the district summary affected?** There is a relatively small difference in the results of the district summary. As can be inferred in table one compared to table two; excluding the math and reading scores of 9th graders from Thomas High School relatively decreases the results of the metrics. This implies that the scores of 9th graders from Thomas high school are high causing such a fall in the metrics, especially in math scores when they are excluded.
	![district_summary_withoutnan](Resources/district_summary_withoutnan.png)
	 ***Table 1: District Summary without NaN replacement***
 
	![district_summary_withnan](Resources/district_summary_withnan.png)	***Table 2: District Summary with NaN replacement***

* **How is the school summary affected?** In school summary, the only thing that is affected is the results for Thomas High School. At first, before removing 9th graders from the calculation the values for the % passing math, the % passing reading, and the % overall passing fall extremely low as can be seen in table 3 because the 461 students are included in the calculation.
	![ths_before_change](Resources/ths_before_change.png)	***Table 3: Thomas High School Before Number of Student Adjustment***

	However, I adjust the number of students in my calculation by excluding the 9th graders in Thomas High School. The results of the adjustment can be seen in table 4. 

	![ths_after_change](Resources/ths_after_change.png)	***Table 4: Thomas High School After Number of Student Adjustment***

	When comparing table 4 with the adjustment to the first case when I didn't change the math and reading scores of 9th graders from the analysis as in table 5, I find a relatively small drop in the results after the adjustments.

	![ths_before_excluding_9th](Resources/ths_before_excluding_9th.png)***Table 5: Thomas High School Before Excluding 9th Graders***

* **How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?** In terms of Thomas High School's performance compared to other schools, we don't see a change. Thomas High School is still ranked second according to the % overall passing values. Table 6 is before excluding 9th grader scores and table 7 is after excluding 9th grader scores. 

	![top_schools_before_excluding](Resources/top_schools_before_excluding.png)***Table 6: Top Five Schools Before Excluding 9th Graders in Thomas High School***

	![top_schools_after_excluding](Resources/top_schools_after_excluding.png)***Table 7: Top Five Schools After Excluding 9th Graders in Thomas High School***

* **How does replacing the ninth-grade scores affect the following:**
	- ***Math and Reading Scores by Grade:*** The only values that are affected by the change are the value for the math and reading scores of 9th graders in which the values become equivalent to NaN.
	

	![average_math_scores](Resources/average_math_scores.png)

	***Table 8: Average Math Scores by Grade***

	![average_reading_scores](Resources/average_reading_scores.png)

	***Table 9: Average Reading Scores by Grade***
	
	- ***Scores by School Spending:***  Before and after the change Thomas High School still falls in the range of $630 - 644, nothing changes the result in terms of categorizing district schools according to school spending.	
	![scores_by_school_spending](Resources/scores_by_school_spending.png)
	
	***Table 10: Scores by School Spending***
	
	- ***Scores by School Size:*** Before and after the change Thomas High School is categorized as a medium (1000-2000) school, likewise, when replacing the math and reading scores of 9th graders with NaN's nothing changes in the values categorized according to school size. 
	
	![scores_by_school_size](Resources/scores_by_school_size.png)
	
	***Table 11: Scores by School Size***

	- ***Scores by School Type:*** Lastly, the changes in 9th grader scores didn't affect the results of scores by school type.

	![scores_by_school_type](Resources/scores_by_school_type.png)
	
	***Table 12: Scores by School Type***


# Summary

## Conclusion 

This is a small study in understanding the performance of Thomas High School compared to the 14 schools in the study. In this analysis, I tried to see how manipulating the data by changing the math and reading scores of 9th graders from Thomas High School will affect the results of a couple of metrics. By doing this I wanted to see whether they have a significant impact on the total outcomes or not. However, the results don't pronounce a significant impact because the changes in the outcome are very small. We can say that 9th graders at Thomas High School are good performers in math because excluding them from the district analysis decreased the overall result of the % passing math. Secondly, I can say that when excluding 9th graders from the analysis, Thomas High School's performance didn't change compared to other schools, it still remained second according to % overall passing. When reading table 10 I can say that there is a negative correlation between the metrics and the amount of money spent on each student. This is a question that can be delved into further to understand the reason behind the negative correlation. Moreover, from table 11 we can conclude that medium-sized schools performed relatively better than small or large sized schools. Lastly, table 12 explicitly shows that charter schools are better performing schools compared to district schools.
## Challenges Encountered 
For most of writing this code, I had to go back and forth in the module and ask questions on Google to get the output I wanted. This was a sweet challenge because the more projects I get to complete the better I feel I become in searching for the right keywords. Compared to using Python in VS Code, I found it easier to use it in Jupyter Notebook.