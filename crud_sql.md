CRUD for Employee Management System

1	Table: Employees
•	Create: This query inserts a new employee into the Employees table with the specified values for employee_id, employee_name, department_id, and 	salary
	
 	INSERT INTO Employees (employee_id, employee_name, department_id, salary) VALUES (1, 'EMP1', 1, 50000.00)

•	Read: To retrieve all employee records from the Employees table

	SELECT * FROM Employees

•	Update: To update an employee's information in the Employees table

	UPDATE Employees SET salary = 55000.00 WHERE employee_id = 1

•	Delete: To delete an employee record from the Employees table

	DELETE FROM Employees WHERE employee_id = 1

2	Table: Departments
•	Create: This query inserts a new row into the Departments table with specified values for department_id, department_name, manager_id, and location.

	INSERT INTO Departments (department_id, department_name, manager_id, location)
	VALUES (1, ‘Sales’, 101, ‘New York’)

•	Read: To retrieve all department records from the Departments table

	SELECT * FROM Departments

•	Update: To update a department's information in the Departments table

	UPDATE Departments SET location = 'Los Angeles' WHERE department_id = 1

•	Delete: To delete a department record from the Departments table

	DELETE FROM Departments WHERE department_id = 1

3	Table: JobRoles
•	Create: This query inserts a new job role into the JobRoles table with the specified values for role_id, role_title, responsibilities, and salary_grade.
 
	INSERT INTO JobRoles (role_id, role_title, responsibilities, salary_grade) 
	VALUES (1, 'Software Engineer', 'Develop and maintain software applications', '5')

•	Read: To retrieve all job role records from the JobRoles table

	SELECT * FROM JobRoles

•	Update: To update a job role’s information in the JobRoles table
	UPDATE JobRoles SET salary_grade = 6 WHERE role_id = 1

•	Delete: To delete a job role record from the JobRoles table
	DELETE FROM JobRoles WHERE role_id = 1

4	Table: EmployeeContacts
•	Create: This query inserts a new contact into the EmployeeContacts table with the specified values for contact_id, employee_id, phone_number, and email.

	INSERT INTO EmployeeContacts (contact_id, employee_id, phone_number, email)
	VALUES (1, 101, ‘123-456-7890’, ‘example@example.com’)

•	Read: To retrieve all contacts from the EmployeeContacts table.

	SELECT * FROM EmployeeContacts

•	Update: To update a contact's information in the EmployeeContacts table.

	UPDATE EmployeeContacts SET phone_number = ‘987-654-3210’ WHERE contact_id = 1

•	Delete: To delete a contact record from the EmployeeContacts table

	DELETE FROM EmployeeContacts WHERE contact_id = 1;

