Employee Management Systems Insert statements

1	Employees:
   
	CREATE TABLE Employees (
		employee_id INT PRIMARY KEY,
		employee_name VARCHAR(100),
		department_id INT,
		salary DECIMAL(12, 2),
	FOREIGN KEY (department_id) REFERENCES Departments(department_id) ON DELETE SET NULL );

2	Departments:
   
	CREATE TABLE Departments (
		department_id INT PRIMARY KEY,
		department_name VARCHAR(100),
		manager_id INT,
		location VARCHAR(100),
	FOREIGN KEY (manager_id) REFERENCES Employees(employee_id) ON DELETE SET NULL);

3	JobRoles:

	CREATE TABLE JobRoles (
		role_id INT PRIMARY KEY,
		role_title VARCHAR(100),
		responsibilities TEXT,
		salary_grade INT
	);

4	EmployeeContacts:

	CREATE TABLE EmployeeContacts (
		contact_id INT PRIMARY KEY,
		employee_id INT,
		 phone_number VARCHAR(20),
		email VARCHAR(100),
	FOREIGN KEY (employee_id) REFERENCES Employees(employee_id) ON DELETE CASCADE);
