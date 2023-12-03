CRUD for Employee Management System

1.	Table: Employees
•	Create: This query inserts a new employee into the Employees table with the specified values for employee_id, employee_name, department_id, and salary.
	
 	INSERT INTO Employees (employee_id, employee_name, department_id, salary)
	VALUES (1, 'EMP1', 1, 50000.00)

•	Read: To retrieve all employee records from the Employees table.
	SELECT * FROM Employees

•	Update: To update an employee's information in the Employees table
	UPDATE Employees SET salary = 55000.00 WHERE employee_id = 1

•	Delete: To delete an employee record from the Employees table
	DELETE FROM Employees WHERE employee_id = 1

2.	Table: Departments
•	Create: This query inserts a new row into the Departments table with specified values for department_id, department_name, manager_id, and location. 
	INSERT INTO Departments (department_id, department_name, manager_id, location)
	VALUES (1, ‘Sales’, 101, ‘New York’)

•	Read: To retrieve all department records from the Departments table
	SELECT * FROM Departments

•	Update: To update a department's information in the Departments table
	UPDATE Departments SET location = 'Los Angeles' WHERE department_id = 1

•	Delete: To delete a department record from the Departments table
	DELETE FROM Departments WHERE department_id = 1

