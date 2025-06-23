# Read

CREATE TABLE uchitdb.student_details
(stud_id integer  primary key,
stud_name varchar(100),
stud_branch varchar(100)
);

CREATE TABLE student_branch_details 
( branch_id INTEGER PRIMARY KEY,
SUBJECT VARCHAR(100),
stud_id  int not null,
foreign key(stud_id) reference student_details(stud_id)
)
