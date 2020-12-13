# School District Analysis

## Overview of the School District Analysis
Our client, the chief data scientist for a city school district, was tasked with preparing standardized test data for analysis, reporting, and presentation to provide insights about student performance trends and patterns. These insights would be used to inform discussions and strategic planning at the school and district level.

At the outset we explored and cleaned the student data, then moved on to generate school and district summaries. We then identified high and low performing schools, and broke out average math and reading scores by grade. We also grouped scores by school type (charter vs district), school size, and school spending per student.

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
* How is the district summary affected?

The district summary shows that scores and % passing rates decreased, if not dramatically, after excluding the Thomas High School (THS) ninth-grade scores. See the comparison below (at one decimal place):

*Original District Summary*
![Original District Summary](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Original%20District%20Summary.png)

*Updated District Summary*
![Updated District Summary](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Updated%20District%20Summary.png)

Average Math Score: down 0.1  
Average Reading Score: unchanged  
% Passing Math: down 0.2  
% Passing Reading: down 0.1  
% Overall Reading: down 0.3  


* How is the school summary affected?

Only Thomas High School scores were impacted by the updated data. See the comparison between the original and updated THS scores and passing percentages below:

*Original Thomas High School Summary*
![Original THS Summary](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Original%20THS%20Summary.png)

*Updated Thomas High School Summary*
![Updated THS Summary](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Updated%20THS%20Summary.png)


* How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

After replacing the ninth graders' scores, Thomas High School's Overall Passing rate did change, but their ranking did not. THS still ranks second in the district in terms of Overall Passing rate.

*Original Top 5 Schools (Overall Passing Rate)*
![Original Top 5](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Original%20Top%205%20Schools.png)


*Updated Top 5 Schools (Overall Passing Rate)*
![Updated Top 5](https://github.com/flowersmichael/School_District_Analysis/blob/main/Resources/Updated%20Top%205%20Schools.png)


* How does replacing the ninth-grade scores affect the following:
  
  * Math and reading scores by grade  
    
    Only the ninth-grade results for Thomas High School were impacted. None of the other schools were impacted, and no scores for 10th, 11th, and 12th grade scores     in all schools were not affected.
    
    
  
  * Scores by school spending
  
    
  
  * Scores by school size
  
  * Scores by school type

