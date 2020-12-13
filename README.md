# School District Analysis

## Overview of the School District Analysis
Our client, the chief data scientist for a city school district, was tasked with preparing standardized test data for analysis, reporting, and presentation to provide insights about student performance trends and patterns. These insights would be used to inform discussions and strategic planning at the school and district level.

At the outset we explored and cleaned the student data, then moved on to generating school and district summaries. We then identified high and low performing schools, and broke out average math and reading scores by grade. We also grouped scores by school type (charter vs district), school size, and school spending per student.

After creating these reports, some evidence emerged that the ninth-grade scores for one of the high schools may have been altered. In this final step we removed the suspicious test scores and generated the district and shool summaries again.

After adjusting our data to exclude the ninth-grade scores at Thomas High School, we wanted to answer the following questions:

* How is the district summary affected?

* How is the school summary affected?

* How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
  
* How does replacing the ninth-grade scores affect the following:
  * Math and reading scores by grade  
  * Scores by school spending
  * Scores by school size
  * Scores by school type

## Resources
* Data Sources:  
    schools_complete.csv  
    students_complete.csv  
    
* Software: 
    Python 3.7.6  
    Pandas library  
    Anaconda Jupyter notebook (server version 6.0.3)   

## Results
### How is the district summary affected?

The district summary shows that average math scores, as well as all passing rates decreased, if not dramatically, after excluding the Thomas High School (THS) ninth-grade scores. Average reading scores actually slightly improved after excluding the ninth graders, although it's not apparent in comparison below (at one decimal place):


*Original District Summary*  
![Original District Summary](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Original%20District%20Summary.png)



*Updated District Summary*  
![Updated District Summary](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Updated%20District%20Summary.png)



Average Math Score: down 0.1  
Average Reading Score: unchanged (up slightly not not visible here) 
% Passing Math: down 0.2  
% Passing Reading: down 0.1  
% Overall Reading: down 0.3  


### How is the school summary affected?

Only Thomas High School scores were impacted by the updated data. See the comparison between the original and updated THS scores and passing percentages below:


*Original School Summary*  
![Original School Summary](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Original%20School%20Summary.png)



*Updated School Summary*  
![Updated School Summary](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Updated%20School%20Summary2.png)




### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

After replacing the ninth graders' scores, Thomas High School's Overall Passing rate did decrease, but their ranking did not. THS still ranks second in the district in terms of Overall Passing rate. Notably, their ranking in terms of % Passing Reading did change, as they fell behind Griffin High School in the updated rankings.


*Original Top 5 Schools (Overall Passing Rate)*  
![Original Top 5](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Original%20Top%205%20Schools.png)



*Updated Top 5 Schools (Overall Passing Rate)*  
![Updated Top 5](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Updated%20Top%205%20Schools.png)




### How does replacing the ninth-grade scores affect the following:


#### Math and reading scores by grade  
    
Only the ninth-grade results for Thomas High School were impacted. None of the other schools were impacted, and no scores for 10th, 11th, and 12th graders in any school including THS were affected.
 
 
*Original Math Scores by Grade*  
![Original Math Scores by Grade](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Original%20Math%20Scores%20by%20Grade.png)


*Updated Math Scores by Grade*  
![Updated Math Scores by Grade](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Updated%20Math%20Scores%20by%20Grade.png)



*Original Reading Scores by Grade*  
![Original Reading Scores by Grade](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Original%20Reading%20Scores%20by%20Grade.png)


*Updated Reading Scores by Grade*  
![Updated Reading Scores by Grade](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Updated%20Reading%20Scores%20by%20Grade.png)
    
  
  
  
#### Scores by school spending

Thomas High School spends $638 per student, landing THS in the $630-644 bin. In the original analysis, this grouping spent the second most and had the third best ranking out of the four groupings. While the update slightly impacted the Overall Passing Rate for the THS bin, it did not impact the rankings in terms of Overall Passing Rate.


*Original Spending Bin Analysis*  
![Original Spending Bin Analysis](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Original%20Spending%20Bin%20Rankings.png)

*Updated Spending Bin Analysis*  
![Updated Spending Bin Analysis](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Updated%20Spending%20Bin%20Rankings.png)
    
    
    
  
#### Scores by school size  
    
Thomas High School has 1635 students, and is categorized as a medium-sized school. The changes to THS ninth-grade student scores slightly affected the Medium       (1000-2000 students) bin passing percentages, but did not impact the shool size grouping rankings.



*Original School Size Analysis*  
![Original School Size Analysis](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Original%20School%20Size%20Analysis.png)


*Updated School Size Analysis*  
![Updated Spending Bin Analysis](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Updated%20School%20Size%20Analysis.png)
    

#### Scores by school type  

Thomas High School is a Charter school. In the original analysis, Charter schools outperformed district schools across all score and % passing categories. The Charter school performance changed slightly after the update. The Average Math Score dropped slightly at two decimal places, while the Average Reading Score improved slightly. The % Passing rates for Charter schools all decreased slightly in the updated analysis, but Charter schools continued to outperform relative to district schools across categories.


*Original School Type Analysis*  
![Original School Type Analysis](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Original%20School%20Type%20Analysis.png)


*Updated School Type Analysis*  
![Updated School Type Analysis](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Updated%20School%20Type%20Analysis.png)

## Summary

There were numerous changes to our analysis after excluding the Thomas High School ninth-grade standardized test math and reading scores. Here are four noteworthy adjustments:

1. The most glaring difference is that we no have no test data for Thomas High School night graders. This makes it very difficult to evaluate that group of students and address their needs accordingly. Some consideration should be given to having the students take the test again, or finding some solution to this problem.

2. After excluding the THS ninth graders, the THS overall math scores decreased, as well as the % Passing Math, % Passing Reading, and % Overall Passing.
The THS overall average reading scores actually increased slightly after the update.

3. In the original analysis, Thomas High School was a top perfomer, with the second-best Overall Passing rate. That ranking did not change with the updated analysis. The Overall Passing % gap between the top performer, Cabrera High School, and THS did widen, however, afte the update. Conversely, the gap between Thomas High School and the others rounding out the top 5 tightened considerably.

4. In the updated rankings, Thomas High School's ranking in terms of % Passing Reading did change, as they fell behind Griffin High School.



