Table 1: Employees (3NF)
- Fields:
  1. employee_id (Primary Key)
  2. employee_name
  3. department_id (Foreign Key referencing Departments table)
  4. salary
 - Functional Dependencies (FDs): employee_id → {employee_name, department_id, salary}
 - Foreign Key Policies: ON DELETE SET NULL (Set the department_id to NULL for related employees if a department is removed).
Sample data:

employee_id	employee_name	department_id	salary
1	John Doe	1	60001
2	BK	2	25000
3	Alex Johnson	1	62000
		




Table 2: Departments (3NF)
- Fields:
  1. department_id (Primary Key)
  2. department_name
  3. manager_id (Foreign Key referencing Employees table)
  4. location
- Functional Dependencies (FDs): department_id → {department_name, manager_id, location}
- Foreign Key Policies: ON DELETE SET NULL (Set the manager_id to NULL for related departments if a manager is eliminated).
Sample data:
department_id	department_name	manager_id	location
1	HR	3	New York
2	Finance	2	Chicago
3	IT	3	KS



Table 3: JobRoles (3NF)
- Fields:
  1. role_id (Primary Key)
  2. role_title
  3. responsibilities
  4. salary_grade
- Functional Dependencies (FDs): role_id → {role_title, responsibilities, salary_grade}
- Foreign Key Policies: No specific policies needed in this case.
Sample data:
role_id	role_title	responsibilities	salary_grade
1	HR Managed	Manage HR department	5
2	Financial Analyst	Analyse financial data	4
3	Software Developer	Develop software solutions	6



Table 4: EmployeeContacts (3NF)
- Fields:
  1. contact_id (Primary Key)
  2. employee_id (Foreign Key referencing Employees table)
  3. phone_number
  4. email
- Functional Dependencies (FDs): - contact_id → {employee_id, phone_number, email}
- Foreign Key Policies: ON DELETE CASCADE (If an employee is removed, remove the related contact details as well).
Sample data:
contact_id	employee_id	phone_number	email
1	1	123-456-7890	john@example.com
2	2	987-654-3210	jane@example.com
3	3	111-222-3333	alex@example.com

Note: All the tables are Third Normal Form (3NF) as they don’t have any transitive dependencies, and all columns seem to depend only on the primary key of each table.

