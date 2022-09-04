# Student-record-management-project-SQL-query-
Short version: This is a SQL project to show case the ability to design relational database based on real-world scenario and SQL query skills. 
Disclaimer: The data has been anonymized in respond to subjects' privacy rights using mockaroo random data generator ("https://www.mockaroo.com/"). 

Summary: <br />
My current full-time job handles a database of incoming international students who take a language placement test and are placed into different levels of writing classes based on their language proficiency. There is over 10,000 entries in this database and it's growing. The original data management method was to create an excel sheet every time there would be a placement test (several times a year) and import information from the registrar (e.g. student ID, email, students' academic groups, education history,  ), from the placement exam (different components of test scores, students' self-placement survey, scorers' individual scores), and from students' exam registration information (years of high school in the U.S.). There were some challenges to the traditional method of data managing, to name a few:<br />
(1) Error-prone: merging tables from different sources using copy-pasting or v-lookup function is prone to errors and . would be difficult to keep track who has taken the exam or not, and what level <br />
(2) Difficult to query data: keeping data entries on excel sheets based on the time students took the placement exams have led to management issues, e.g. duplicate records of students taking exams at different times (how to say this better?), quiry students' placement level across different excel sheets. <br />
(3) Data update issue: new international students enrolled throughout the summer with weekly updates in the database. <br />
To ease the level of effort of compiling the results of multiple exams throughout the years and keep integrity of maintaining student placement and course registration information, and accurately track students’ registration status in relation to their placement results, and help the coordinators predict the number of students, there is need for the program to build a database to house the student information. <br />

Business rules:<br />
(1) All international students (visa status) whose language status is "English is not a dominant language" is on the tracking list for the placement exam. Coordinators receive an international matriculation list weekly from other administrative bodies in the university. <br />
(2) Students register for the placement exam through Qualtrics. Coordinators will send out either reminder emails or instructions based on the students registered or not before the registration deadline for the exam.<br />
(3) 
