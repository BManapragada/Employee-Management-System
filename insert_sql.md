Insert Statements
1	Employees

    INSERT INTO Employees (employee_id, employee_name, department_id, salary) 
    VALUES
    (1, 'Bharath', 1, 60000.00),
    (2, 'Kumar', 2, 55000.00),
    (3, 'Prakash', 1, 62000.00),
    (4, 'Raju', 3, 58000.00),
    (5, 'Mani', 2, 59000.00)

2	Departments:

    INSERT INTO Departments (department_id, department_name, manager_id, location) 
    VALUES
    (1, 'HR', 3, 'New York'),
    (2, 'Finance', 2, 'Chicago'),
    (3, 'IT', 5, 'San Francisco'),
    (4, 'Operations', NULL, 'Los Angeles')

3	JobRoles:

    INSERT INTO JobRoles (role_id, role_title, responsibilities, salary_grade)
    VALUES
    (1, 'HR Manager', 'Manage HR department', 5),
    (2, 'Financial Analyst', 'Analyze financial data', 4),
    (3, 'Software Developer', 'Develop software solutions', 6),
    (4, 'Operations Manager', 'Manage operations', 5),
    (5, 'Intern', 'Assist in various tasks', 2)

4	EmployeeContacts:

    INSERT INTO EmployeeContacts (contact_id, employee_id, phone_number, email)
    VALUES
    (1, 1, '123-456-7890', 'bhar@example.com'),
    (2, 2, '987-654-3210', 'kr@example.com'),
    (3, 3, '111-222-3333', 'prak@example.com'),
    (4, 4, '444-555-6666', 'raju@example.com'),
    (5, 5, '777-888-9999', 'raju@example.com')
