# Ex. No: 5 Creating Triggers using PL/SQL

### AIM: To create a Trigger using PL/SQL.

### Steps:
1. Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(10),salary NUMBER);
2. Create salary_log table with following attributes (log_id NUMBER GENERATED ALWAYS AS IDENTITY, empid NUMBER,empname VARCHAR(10),old_salary NUMBER,new_salary NUMBER,update_date DATE);
3. Create a trigger named as log_salary-update.
4. Inside the trigger block, Insert the values into the salary_log table whenever the salary is updated.
5. End the trigger.
6. Update the salary of an employee in employee table.
7. Whenever a salary is updated for the employee it must be logged into the salary_log table with old salary and new salary.
8. Display the employee table, salary_log table.

### Program:
```
CREATE TABLE employee2( empid NUMBER,empname VARCHAR2(10),dept VARCHAR2(10),salary NUMBER);

CREATE TABLE sal_log (log_id NUMBER GENERATED ALWAYS AS IDENTITY, empid NUMBER, empname VARCHAR2(10), old_salary NUMBER, new_salary NUMBER,update_date DATE);

insert into employee2 values(1,'John','HR',50000);
insert into employee2 values(2,'Joe','IT',60000);
insert into employee2 values(3,'Bob','Finance',55000);
```
### Create employee table
```
CREATE TABLE employee(empid NUMBER, empname VARCHAR2(10), dept VARCHAR2(10), salary NUMBER);
```
### Create salary_log table
```
CREATE TABLE salary_log (log_id NUMBER,empid NUMBER,empname VARCHAR2(10),old_salary NUMBER,new_salary NUMBER,update_date DATE);
```
### PLSQL Trigger code
![5i](https://github.com/varshxnx/Ex-No-5-Creating-Triggers-using-PL-SQL/assets/122253525/34ac784f-e1d7-49d8-baf6-274c3b3ecfe6)

### Output
![5o](https://github.com/varshxnx/Ex-No-5-Creating-Triggers-using-PL-SQL/assets/122253525/f23ecdd1-7d41-42c6-bbeb-07590c7ec242)

### Result:
Therefore the output has been successfully verified.
