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
(3) Each student can only take one test and receive only one result, regardless of which placement exam they choose to take throughout the year. Students who try to retake the test are removed from the registration list and notifications will be sent to the students who attempted to retake. <br />
(4) A student is placed in one level based on their placement result and the level will decide which course they need at the following semester and any subsequent courses. <br />
(5) There are course prerequisites that place stop on students to register for levels above their placement level and triggers reports to the program coordinators with such attempts. <br />
(6) Each student should register for their next-level writing classes immediately after they finished the current level. Based on this information, the coordinator need to send out a reminder email to them.  <br />
(7) If a student failed their writing class, they cannot move on to the next course level. <br />
(8) The placement information is also used for the coordinators to make decisions on the course schedules for the upcoming year. <br />
(9) Other business rules will be defined in later iterations of the database. <br />

The following is the logical model design for the database: 

![image](https://user-images.githubusercontent.com/94016314/188331490-709a3b09-1bb4-4214-af2b-ad112fcd3bf8.png)

The project showcases the following sql coding: 
- Data definition (creating tables and constraints)
- Data manipulation (data-input, data-revision)
- EDA based on the data questions
