THE GRADEBOOK MANAGEMENT SYSTEM ASSIGNMENT

The Gradebook Management System is a python-based program that helps manage student grades efficiently using organized Python structures like lists, tuples and dictionaries. It allows users to add, update, view, and delete student information.

SETUP INSTRUCTIONS

- Ensure that python 3 is installed on the device.
- Open the .py file in a python environment.
- Run the python script.
- Follow the prompts displayed in the terminal.
  
#SECTION A - Basic Student Management

Features

• Prompts the user to enter their number of students
• ⁠ Prompts the user to enter student names
• ⁠ Prompts the user to enter student grades
• ⁠ Calculates the grades total
• ⁠ Calculates the average
• ⁠ Displays the grades total
• ⁠ Displays the average
• ⁠ Performs grade validation to ensure that grades entered are between 0 and 100

Example  Input/Output  
Assumptions  and  Limitations  

- Grades entered should be 0 zero and 100
- Grades can be whole numbers or numbers with decimal points
- Each student should have one grade

Known  Issues  

When prompted for the number of students and a user enters 0, the program encounters at division by zero error meaning does not handle a student count of 0 when the average is calculated. 
![Zero Division Error](0division.png)
