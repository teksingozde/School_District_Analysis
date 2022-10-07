
Project Overview
The PyCity School District requested the students' math and reading scores, along with the school information they attended, and the school types and school budget information. By using Python programming language and pandas library, the process of cleaning and examining the data in Jupyter Notebook was carried out.
Resources
•	Data Source: new_full_student_data.csv
•	Software: Python 3.9.12
Jupyter Notebook 6.4.8
Pandas 1.4.2
Results
In the Results section, you will see the tables of the examinations made and the examinations of the tables.
Table 1. Students Information
 
In the table above, the first five students are listed in line with the information obtained from the new_full student.csv file. 
According to the information obtained from this table, it is seen that the student named Travis Martin is a 9th grade student, a Sullivan High school student, and the reading score is 59.0, the math score is 88.2, the school type is public, and the school budget is $961.125.
Table 2.  Remove Null Rows 
 
According to the table above, it is seen that the lines belonging to the values that are NaN or missing are completely removed.
Table 3. Columns Data Types 
 
The data types of the columns are shown in the table above. 



Table 4. Grade Column Information
 
In Table 4, attention is drawn to the information about the grade column. Looking at the information of the Grade column, it is observed that the total length, that is, the data size, is 14831 rows, and the data type is object.
Table 5. Change Grade Column Data Type
 
Normally, according to the analyzes made in Table 3 and Table 4, it is known that the data type of the grade column is object. For Table 5, we are asked to change the data type of the grade column to integer.
Table 6. Summary Statistics
 
Table 6 shows the summary statistics values of the grade, reading_score, math_score and school_budget columns.
It is observed that all columns have 14831 values. This is because the lost data has been cleared.
According to the general student evaluation,
If the evaluation of the Grade column is made; Its mean is 10.35, its standard deviation is 1.09, its min value is 9 and its max value is 12.
If the reading_score column is evaluated; Its mean is 72.35, its standard deviation is 15.22, its min value is 10.5 and its max value is 100.
If the math_score column is evaluated; Its mean is 64.75, its standard deviation is 15.84, its min value is 3.7 and its max value is 100.
If the evaluation of the school_budget presentation is made; the average is $893742, the minimum value is $817615 and $991918.


Table 7. Display the Grade Column By Using loc
 
Table 7 shows the grade column using loc.
Table 8. Using iloc
 
In the above table, the values of the first three rows and school_name, reading_score and math_score columns are examined using iloc. According to the table, Sullivan High School students ranked first with a reading_score of 59 and a math_score of 88.2; Dixon High School students had a reading_score of 94.7 and a math_score of 73.5; Wagner High School students have a reading_score of 89.0 and a math_score of 70.4.



Table 9. Grade 9th Summary Statistics
 
In order to make general evaluations of 9th grade students, a summary statistics table was created using loc and describe. Starting from this table;
In total, there are 4132 9th grade students.
The standard deviation of 9th grade students' reading_score scores is 15.27 and the standard deviation of math_score scores is 16.66.
The 9th grade student with the minimum reading_score score is 17.90, while the student with the minimum math_score score is 5.30.
The student with the maximum reading_score score has a score of 99.90, and the student with the maximum math_score score has a score of 100.0.




Table 10. Row with Minimum Reading Score 
 
The student with the minimum reading_score;
 His order on the list is 3706, his first and last name is Matthew Thomas. The student's ID number is 81758630.
Matthew Thomas is a 10th grader and attends Dixon High School. Matthew has a minimum reading_score of 10.5 and a math_score of 58.4. Matthew's school type is Charter and his school budget is $870334.
Table 11. Dixon High School’s 10th Graders Reading Score
 
Reading_score scores of 10th grade students studying at Dixon High School are shown in the table above. To analyze this table, loc conditionals are used.
The first of the Dixon High School 10th graders is on line 45, and his score in this ranking is 71.1.
In this school, the second student among the 10th graders is on the 60th row. This student's reading_score is 59.5. However, when the table is examined carefully, it will be noticed that it does not have an order from smallest to largest or largest to smallest. Because the student on line 19368 has a reading_score score of 84.4.
Table 12. School Budgets for School Types 
 
As can be seen in Table 12, there are two types of schools. These; charter and public schools. The budget for the charter school type is $872625 on average, while the budget for the public school type is $911195 on average. In this case, it can easily be said that the public school type is more expensive than the charter school type.






Table 13. Student Count with School Names
 
In the table above, schools are listed from largest to smallest according to the number of students.
While the school with the most students would be Montgomery High School with 2038 students
The second school with 1961 students is Green High School. Dixon High School ranked third with 1583 students.
Looking at the last rows, it is seen that Campbell High School and Chang High School are in the last two rows. But the difference between them is huge. While Campbell High School has 407 students, Chang High School has 171 students.
Table 14. School Type with Grade and Math Scores
 
When the examination is made according to Table 14,
If a charter school type interpretation is made, the reading_score score of the 9th grade students is 70.07, the 10th grade students are 66.44, the 11th grade students are 68.02 and the 12th grade students are 60.21.
If a Public School type interpretation is made, the reading_score score of the 9th grade students is 63.77, the 10th grade students are 63.76, the 11th grade students are 59.31 and the 12th grade students are 63.56.
If a comparison is made between Charter and Public school types, it is quite open to interpretation that 9th, 10th and 11th grade students are more successful in Charter school type, excluding 12th grade students. According to the public school type reading_score score, it can be interpreted that only the 12th grades are successful.
Summary
For the School District Analysis study, first Jupyter Notebook was established. To comment on Jupyter Notebook, writing the codes is both more practical, more understandable and very supportive in terms of finding errors easily. In this module, the main focus was on importing the pandas library and then using it efficiently in the analysis. Pandas library, in general, is very involved in performing mathematical operations, cleaning data and manipulating data. For this study, first of all, how many rows of data are missing was determined and cleaning was done. Then, the grade column is converted from object data type to integer data type. In general, statistical summaries of the columns were made and necessary comments were made. Student numbers were determined on the basis of schools, and mathematics and reading scores were examined according to school types. The student with the minimum reading score has been identified. At the same time, their budgets according to school types were examined and the reading scores of each school type were analyzed on a per-class basis, and it is said that in general, in the reading score round, Charter school types are more successful despite being cheaper.
If we look at this general summary, data cleaning is very important, especially in large volumes of data, and it ensures that the analysis comes out with a high reliability rate.














