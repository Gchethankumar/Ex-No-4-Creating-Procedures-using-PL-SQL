# Ex-No-4-Creating Procedures using PL/SQL

## AIM: 
To create a procedure using PL/SQL.

### Steps:
1. Create EMPLOYEE table with following attributes (empid number, empname varchar(10), dept varchar(10),salary number);
2. Create a procedure named as insert_EMPLOYEE data.
3. Inside the procdure block, write the query for inserting the values into the EMPLOYEE table.
4. End the procedure.
5. Call the insert_EMPLOYEE data procedure to insert the values into the EMPLOYEE table.
6. Display the EMPLOYEE table

## Program:
#### 1.Create a Table:
```sql
create table EMPLOYEE(empid number, empname varchar(10), dept varchar(10), salary number);
```
#### 2.Create Procedure:
```sql
create or replace procedure insert_EMPLOYEE_data as
2  begin
3  insert into EMPLOYEE(empid,empname,dept,salary) values(1,'Chandru','HR',70000);
4  insert into EMPLOYEE(empid,empname,dept,salary) values(2,'Chethan','MD',95000);
5  insert into EMPLOYEE(empid,empname,dept,salary) values(3,'Dileep','HR',80000);
6  commit;
7  end;
8  /
```
#### 3.Call the procedure:
```sql
 BEGIN
  2  insert_EMPLOYEE_data;
  3  END;
  4  /
```
#### 4.Display the Table:
```sql
select * from EMPLOYEE;
```
## Output:
![Screenshot 2023-10-16 170251](https://github.com/Gchethankumar/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/118348224/e092f50e-42dd-4f5f-ad34-d3edf3ca3491)


## Result:
Hence the procedure using pl/sql is created successfully.
