# collegeapllication



create table student(
student_id number(5) primary key,
sname varchar2(30) not null,
email varchar2(30) unique,
password varchar2(20) not null,
gender varchar2(10) not null,
dateOfBirth varchar2(20) not null,
branch varchar2(20) not null,
dateOfJoin varchar2(20),
mobileno varchar2(20),
parentmobile_number varchar2(20) not null,
address varchar2(50) not null
);


CREATE SEQUENCE sequence_1
start with 1
increment by 1
minvalue 1
NOCYCLE;


CREATE SEQUENCE sequence_faculty
start with 1
increment by 1
minvalue 1
NOCYCLE;

CREATE SEQUENCE sequence_event
start with 1
increment by 1
minvalue 1
NOCYCLE;


CREATE SEQUENCE sequence_staffmeeting
start with 1
increment by 1
minvalue 1
NOCYCLE;


CREATE SEQUENCE sequence_alumni
start with 1
increment by 1
minvalue 1
NOCYCLE;

insert into student values(1,'cs','cs@mail.com','12345','male','01-01-1995','csc','05-jun-2016','1234567789','9876541975','bezavada');


create table faculty(
fid  number(20),
fname varchar2(20),
email varchar2(20) primary key,
password varchar2(20),
gender varchar(20),
dateofbirth varchar2(20),
mobilenumber number(20),
Address varchar2(20),
deptname varchar2(20),
doj varchar2(20)
);


create table admin(
admin_id varchar2(20) primary key,
password varchar2(20)
);

create table applicant(
appli_name varchar2(20),
email_id varchar2(20) primary key,
gender varchar2(10),
branch varchar2(20),
phone_num varchar2(15),
status varchar2(10),
percentage number(10));

create table events(
eid number(9),
e_name varchar2(50),
e_date varchar2(20),
e_venue varchar2(20)
);

create table staffmeeting(
id number(9),
meeting_name varchar2(40),
meeting_date varchar2(20),
meeting_time varchar2(20),
meeting_venue varchar2(20)
);



Create table ex_schedule(exam1 varchar2(20), e_date date , exam2 varchar2(20),
e_date3 date , exam4  varchar2(20), e_date4 date );

create table placement_cal(sno number(20),company_name varchar(20),
exam_date date,package number(20),type varchar(20));

create table alumni(alumni_id varchar2(20) primary key,password varchar2(20));

create table alumni_details(alumni_id varchar2(20), alumni_name varchar2(20),
branch varchar2(20),phone_num number(15));
