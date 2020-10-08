# School_District_Analysis
Anallyzing testing data across the district. Utilizing Jupyter Notebook, Python 3.7.6. 
## Analysis Overview ##
The chief aim of this project is the analyze the testing results for the given school district, for both district and charter schools. The key analyses were calculating the passing rates for the math and reading portions of the test, the averages for the math and reading scores, and an overalll passing rate determined by the number of students passing both math and reading. In addition to breaking down the results by school and by grade, the analysis took into consideration several factors for comparison, listed below. 
- School type: District vs. Charter
- School size: Small (<1000), Medium (1000-2000), and Large (2000-5000)
- School per Capita spending

The scope of this analysis to provide useful snapshots of data to both district leaders and specific school personnel. 
## Results ##
Initial results are displayed below. Due to a compromise of testing security, follow analyses were performed to adjust the original results. Initial analyses were adjusted by removing the 9th grade reading and math scores from Thomas High School (THS). The effects are specified below. 
- Initial District Summary: <br />
![](Resources/district_summary.png)
- Adjusted District Summary: <br />
![](Resources/adj_district_summary.png) <br />
On a district wide level (with 39170 students total), the effects of removing the 461 9th grade scores from THS are minimal. The greatest change being that the adjusted percent of students passing reading rose by .3%. With the exception of the average reading score which had no significant change, the other values showed an increase by about .1%.  
- Initial School Summary: <br />
![](Resources/school_summary.png)
- Adjusted School Summary: <br />
![](Resources/adj_school_summary.png) <br />
While average math score showed no significant change and average reading score even improved by 0.1%, removing the compromised scores dropped the % passing rates by tenths of percentage points in all 3 categories. 
- These drops hurt the school's overall standing relatively speaking, causing it to drop from the 2nd ranked school by % Overall Passing, to the 3rd ranked school behind Griffin. 
![](Resources/top_five.png) ![](Resources/adj_top_five.png)
- **Changes on Scores by Grade Level**: Given that each average for was calculated indpendently for each grade level, substituting *NaN* values for the 9th grades at THS has no impact on any of the scores, save for the dropping of an average for 9th graders. Displayed are the scores by grade levels, and the adjustment made for THS. 
<p float="middle">
  <img src="/Resources/math_by_grade.png" width="200" />
  <img src="/Resources/adj_math_by_grade.png" width="175" />
  <img src="/Resources/reading_by_grade.png" width="200" /> 
  <img src="/Resources/adj_reading_by_grade.png" width="175" />
</p> 

- **Changes on Scores by School Spending**: Given the scope of the district (which comprises 39170), removing the 461 9th graders from THS did not yield a statistically significant change to the tenths of a percentage point on district scores categorized by per capita spending. Adjusted results are listed first, original second. As can be seen, there was no detectable difference given our scope of precision. 
![](Resources/adj_spending_summary.png)
![](Resources/spending_summary.png) <br />
- **Changes on Scores by School Size**: Again, given the scope of the district (which comprises 39170), removing the 461 9th graders from THS did not yield a statistically significant change to the tenths of a percentage point on district scores categorized by school size. Adjusted results are listed first, original second. As can be seen, there was no detectable difference given our scope of precision. 
![](Resources/adj_size_summary.png) ![](Resources/size_summary.png) <br />

- **Changes on Scores by School Type**: Given the scope of the district (which comprises 39170), removing the 461 9th graders from THS did not yield a statistically significant change to the tenths of a percentage point on district scores categorized by school type. Adjusted results are listed first, original second. As can be seen, there was no detectable difference given our scope of precision. 
![](Resources/adj_type_summary.png) ![](Resources/type_summary.png) <br />

## Summary ##
It should be noted that I deliberately did not adjust the school size for THS for analyses that were analyzed at a district level such as the per capita, school size and school type results. Since any prep done by those schools would have been performed for the school at large not anticipating the removal of the 9th grade scores, I decided that it would not be accurate for the districts to see an adjusted analysis as it would be misleading and indicate greater resources were available per student than was the case. <br />
**Key Changes:**
1. At the district level, there were no changes on scores by per capita spending. 
2. At the district level, there were no changes on scores by school size. 
3. At the district level, there were no changes on scores by school type. 
- Thus, the analyses later conducted by the district leadership themselves, as well as any school-level analyses, will not have been compromised for any schools other than THS. 
4. The overall district summary resport showed changes given that it took into consideration 461 less than the original 39170 students. 
5. Thomas High School lost standing as the 2nd highest in Overall Passing rates. 
