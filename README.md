# eshikhon-assignments
here i will upload my assignments...

Students:
Id -> int 
Name -> String 
Address  -> String 
Create Table 
CREATE TABLE students ( id int, name varchar(200), address varchar(200) );

Insert Data into table 
INSERT INTO students(id, name, address) VALUES(1, "ABC", "Dhaka");

Drop Table
DROP TABLE students_v1;

Alter Table [Add]

ALTER TABLE students ADD mobile_number varchar(20);

Alter Table [ Modify Column Data type]

ALTER TABLE students MODIFY mobile_number int;

Alter Table [DROP Column]
ALTER TABLE students DROP COLUMN mobile_number;

Update 

UPDATE students SET name = "Hasan" where id = 1;

Delete 

DELETE FROM students WHERE id = 2;

SELECT * FROM `students` WHERE id = 1;

SELECT name FROM `students` WHERE id = 1;

SELECT name FROM `students`;

SELECT DISTINCT address FROM students;

SELECT * FROM students where address LIKE 'D%';


SELECT * FROM students ORDER by id DESC;


SELECT * FROM students ORDER by id ASC;

SELECT * FROM students ORDER by name;

SELECT MIN(id) FROM students;

SELECT MAX(id) FROM students;
SELECT AVG(id) FROM students;

SELECT COUNT(id) FROM students;

SELECT SUM(id) FROM students;

SELECT SUM(id) as totalSum FROM students;

SELECT * FROM `students` WHERE address in ("Noakhali", "Khulna")	

SELECT * FROM `students` WHERE id BETWEEN 4 and 6;



SELECT s.name as studentName, t.name as teacherName from students as s INNER join teacher_student as ts on ts.student_id = s.id INNER join teacher as t on t.id = ts.teacher_id;
