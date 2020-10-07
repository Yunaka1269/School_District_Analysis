# School_District_Analysis

##The school board has notified that reading and math grades for Thomas High School ninth graders had been altered. They asked to change those grades with "NaN"s and keep the rest of records. Run and repeat the analysis which was performed earlier after those scores being replaced. The school board and Maria would like to know how this change affects the overall analysis and followings are task and results:

***(Note: pictures show original analysis on the left and new analysis on right)***

1. How is the district summary affected?

   [District_Summary_Result](https://github.com/Yunaka1269/School_District_Analysis/blob/main/Pictures/District_Summary.PNG)
  
   -Decline shows in average math score by  -0.1, % passing math by -0.2%, % passing reading by -0.3%, and % overall passing by -0.1%  

2. How is the school summary affected?

   [School_Summary_Result](https://github.com/Yunaka1269/School_District_Analysis/blob/main/Pictures/School_Summary.PNG)
  
   -Increase in average reading score +.05

   -Decline in average math score -0.07, % passing math -0.09%, % passing reading -0.29%, % overall passing -0.32%

3. How does replacing the ninth grader's math and reading scores affect Thomas High School's performance relative to the other schools?

   [Top_Five_Schools_Result](https://github.com/Yunaka1269/School_District_Analysis/blob/main/Pictures/Top_Five.PNG) and [Bottom_Five_Schools_Result](https://github.com/Yunaka1269/School_District_Analysis/blob/main/Pictures/Bottom_Five.PNG)
  
   -Top five and bottom five schools are the same even after the change being made. The change didn't affect significantly enough to move the overall ranking.  

4. How does replacing the ninth-grade scores affect below

   A. [Math_By_Grade_Result](https://github.com/Yunaka1269/School_District_Analysis/blob/main/Pictures/Math_By_Grade.PNG) and [Reading_By_Grade_Result](https://github.com/Yunaka1269/School_District_Analysis/blob/main/Pictures/Reading_By_Grade.PNG)
	
    -The change doesn't impact on other school or other grades math and reading score at all. The only change is Thomas High ninth grade scores become "nan".
		
   B. [Scores by school spending_Result](https://github.com/Yunaka1269/School_District_Analysis/blob/main/Pictures/School_Spending.PNG) 
	
    -The impact on scores by school spending category "($630-644)" is very little to none. The values in dataframe are the same.
		
   C. [Scores by school size_Result](https://github.com/Yunaka1269/School_District_Analysis/blob/main/Pictures/School_Size.PNG)
	
    -The impact on scores by school size "Medium (1000-2000)" is very little to none. The values in dataframe are the same.
		
   D. [Scores by school type_Result](https://github.com/Yunaka1269/School_District_Analysis/blob/main/Pictures/School_Type.PNG)
	
    -The impact on scores by school type "Charter" is very little to none. The values in dataframe are the same.
    
###Resources
- Data Source: schools_complete.csv, students_complete.csv
- Software: Jupyter Notebook 6.1.4

- Code: import numpy as np
  	df.loc["",""] 
	df.isnull().sum()
	df.value_counts()
	df=pd.cut()

##Summary

Even though Thomas High School ninth grader's scores are replaced with "NaN", they are still included in total students yet the impacts are very minimal on benchmarks because the population of Thomas High School ninth grade is 461 students which is just 1.2% of total students in the whole district. Also, the student counts of ninth grade was only deducted from the number of student who took test in Thomas High School for average score and passing % calculation. Therefore, the change doesn't affect the performance of other schools. The major changes in the updated school analysis are the values within Thomas High School summary, especially in % passing reading. By looking at the result change, average math score -0.07, average reading score +.05, % passing math -0.09%, % passing reading -0.29%, % overall passing -0.32%, the large number of Thomas High School ninth grader's reading score was near the average of 83 points. 
