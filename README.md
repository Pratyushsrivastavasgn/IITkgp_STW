USE Student_info;
CREATE TABLE Student(
Student_ID int,
Student_Name varchar(255),
Department varchar(255),
Hostel varchar(255)
);
//this is to create the table and use the database you can see the columns with its datatype(value/size)

<-------------------------------------------------------------------------->

INSERT INTO Student (Student_id,Student_Name,Department,Hostel)
values
(1,'Anwesh','CSE','Kaari'),
(2,'Pratyush','CSE','Oori'),
(3,'Vishal','ECE','Kaari'),
(4,'Vihan','CSE','Paari');
// this is to add the rows and data in the table mysql is a structured query lang. so we work upon the tables as they are structured.
here 

values
(entry1,entry2,...),
(entry1,entry2,...),
(entry1,entry2,...),
(entry1,entry2,...);

<-------------------------------------------------------------------------->

 -- SELECT * FROM Student;
-- SELECT Student_ID, Student_Name FROM Student;
-- SELECT distinct Department FROM Student;
SELECT Student_ID as ID, Student_Name as name FROM Student;

this is the cmd for displaying the table, where:-

* --> the complete table 
SELECT "Student_ID, Student_Name" FROM Student; --> is the colunm you need to display 

SELECT Student_ID as ID, Student_Name as name FROM Student;--> this changes the colunm names but thr original name is sustained its just for th dev purposes.
<-------------------------------------------------------------------------->


SELECT * FROM Student WHERE	hostel = 'Kaari'; 
this is WHERE keyword, by which we can search the entries.

<-------------------------------------------------------------------------->


UPDATE  Student 
SET percentage = 70 
where Student_Name = 'Vishal'

<-------------------------------------------------------------------------->

Sample Example Code



USE Student_info;
-- CREATE TABLE Student1(
-- Student_ID int,
-- Student_Name varchar(255),
-- Department varchar(255),
-- Hostel varchar(255),
-- Percentage int
-- );

-- INSERT INTO Student1 (Student_ID, Student_Name, Department, Hostel, Percentage) VALUES
-- (101, 'Aarav Mehta', 'Computer Science', 'H-Block', 89),
-- (102, 'Diya Sharma', 'Electronics', 'A-Block', 92),
-- (103, 'Kabir Rao', 'Mechanical', 'G-Block', 76),
-- (104, 'Sneha Patel', 'Civil', 'F-Block', 81),
-- (105, 'Aditya Verma', 'Electrical', 'E-Block', 85),
-- (106, 'Ishita Nair', 'Computer Science', 'H-Block', 94),
-- (107, 'Rohan Das', 'Information Tech', 'D-Block', 88),
-- (108, 'Ananya Gupta', 'Biotechnology', 'C-Block', 90),
-- (109, 'Kunal Roy', 'Mechanical', 'G-Block', 73),
-- (110, 'Pooja Iyer', 'Civil', 'F-Block', 80);
-- select * from Student1;
SELECT * FROM Student1 WHERE percentage BETWEEN 60 and 90 or Hostel = 'F-Block';
SELECT max(percentage) as max_percentage FROM Student1;
SELECT DISTINCT Hostel from Student1;









