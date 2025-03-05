# Employee Management System
## This project was developed in the first year of university under the supervision of Dr Mahmoud Mahdi.
## Overview
The Employee Management System is a C++ application designed to manage departments, staff, and projects within an organization. The system allows users to add, view, and manage departments, staff members, and projects, including budget management.

## Features
- **Department Management**: Add and view department details.
- **Staff Management**: Add, delete, and view staff members.
- **Project Management**: Add, view, and manage project budgets.

## Demo
![Employee Management System Demo](demo.gif)

## File Structure
- `Employee-Management-App.cpp`: Main application file containing the main menu and function calls.
- `Department.h` / `Department.cpp`: Contains the `Department` class for managing department details.
- `Staff.h` / `Staff.cpp`: Contains the `Staff` class for managing staff members.
- `StaffMember.h` / `StaffMember.cpp`: Contains the `StaffMember` class for individual staff member details.
- `Project.h` / `Project.cpp`: Contains the `Project` class for managing project details and budgets.
- `Budget.h` / `Budget.cpp`: Contains the `Budget` class for managing budget details.
- `SalariedEmployee.h` / `SalariedEmployee.cpp`: Contains the `SalariedEmployee` class for salaried employees.
- `CommissionEmployee.h` / `CommissionEmployee.cpp`: Contains the `CommissionEmployee` class for commission-based employees.
- `ExecutiveEmployee.h` / `ExecutiveEmployee.cpp`: Contains the `ExecutiveEmployee` class for executive employees.
- `HourlyEmployee.h` / `HourlyEmployee.cpp`: Contains the `HourlyEmployee` class for hourly employees.
- `Volunteer.h` / `Volunteer.cpp`: Contains the `Volunteer` class for volunteers.
- `Employee.h` / `Employee.cpp`: Contains the `Employee` base class for all employee types.

## Classes
### Department
- **Attributes**: `departID`, `departName`
- **Methods**: `departDetails()`, `printDepartDetails()`

### Staff
- **Attributes**: `staffList` (vector of `StaffMember` pointers)
- **Methods**: `addMember()`, `delMember()`, `showAll()`

### StaffMember
- **Attributes**: `employeeID`, `name`, `phone`, `email`
- **Methods**: `getData()`, `print()`, `getEmployeeId()`, `pay()`

### Project
- **Attributes**: `projectID`, `managerId`, `location`, `managerName`, `managerPhone`, `managerEmail`, `currentCost`, `budgetList` (vector of `Budget` pointers)
- **Methods**: `setManagerData()`, `inputData()`, `addBudget()`, `getTotalBudget()`, `print()`

### Budget
- **Attributes**: `Id`, `value`
- **Methods**: `increaseBudget()`, `set_id()`, `get_id()`, `set_value()`, `get_value()`, `input()`, `print()`

### SalariedEmployee
- **Attributes**: Inherits from `Employee`
- **Methods**: Specific methods for salaried employees

### CommissionEmployee
- **Attributes**: Inherits from `Employee`
- **Methods**: Specific methods for commission-based employees

### ExecutiveEmployee
- **Attributes**: Inherits from `Employee`
- **Methods**: Specific methods for executive employees

### HourlyEmployee
- **Attributes**: Inherits from `Employee`
- **Methods**: Specific methods for hourly employees

### Volunteer
- **Attributes**: Inherits from `Employee`
- **Methods**: Specific methods for volunteers

### Employee
- **Attributes**: Base class attributes
- **Methods**: Base class methods

## Installation
1. Clone the repository:
   git clone https://github.com/M7md-Galal/Employee-Management-System.git

2. Open the project in Visual Studio 2022.
3. Build the solution to compile the project.

## Usage
1. Run the application.
2. Use the main menu to navigate through the options:
   - `1. Department`: Manage departments.
   - `2. Staff`: Manage staff members.
   - `3. Project`: Manage projects and budgets.
3. Follow the prompts to add, view, or manage details.


   
