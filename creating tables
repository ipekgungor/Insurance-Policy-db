1) Employee
create table Employee(
SSN number(11) primary key,
emp_id number(6),
emp_name varchar(25),
emp_surname varchar(30),
emp_address varchar(30),
emp_phone varchar(11),
unique(SSN, emp_id)
);

2) Customer 
create table Customer(
customer_id number(6) primary key,
customer_name varchar(25),
customer_surname varchar(30),
customer_address varchar(30),
customer_phone varchar(11),
up_to_date_health_information varchar(40),
employee_ssn number(11),
foreign key(employee_ssn) references employee(SSN)
);

3) InsurancePolicy
create table InsurancePolicy(
policy_id number(6) primary key,
policy_date date default sysdate,
customer_id number(6),
foreign key(customer_id) references Customer(customer_id)
);

4) Premium
create table Premium(
policy_id number(6) primary key,
unlimited_dental_treatment varchar(25),
unlimited_eye_treatment varchar(25),
foreign key(policy_id) references InsurancePolicy(policy_id)
);

5) Standard
create table Standard(
policy_id number(6) primary key,
one_time_eye_treatment varchar(25),
foreign key(policy_id) references InsurancePolicy(policy_id)
);

6) ContractedInstitution
create table ContractedInstitution(
institution_id number(4) primary key,
institution_name varchar(30),
institution_addres varchar(30),
institution_phone varchar(11),
treatment_method varchar(40)
);

7) Own
create table Own(
policy_id number(6),
institution_id number(4),
primary key(policy_id, institution_id),
foreign key(policy_id) references InsurancePolicy(policy_id),
foreign key(institution_id) references ContractedInstitution(institution_id)
);


