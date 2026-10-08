# THE GRADEBOOK MANAGEMENT SYSTEM ASSIGNMENT

The Gradebook Management System is a python-based program that helps manage student grades efficiently using organized Python structures like lists, tuples and dictionaries. It allows users to add, update, view, and delete student information.

## SETUP INSTRUCTIONS

- Ensure that python 3 is installed on the device.
- Open the .py file in a python environment.
- Run the python script.
- Follow the prompts displayed in the terminal.
  
## SECTION A - Basic Student Management

### Features
- Prompts the user to enter their number of students
- Prompts the user to enter student names
- Prompts the user to enter student grades
- Calculates the grades total
- Calculates the average
- Displays the total of the grades
- Displays the class average
- Performs grade validation to ensure that grades entered are between 0 and 100

###  Example  Input/Output  
This is a demonstration of how the program runs and the key features implemented.

![P1](sect_a1.png)
![P2](sect_a2.png)
![P3](sect_a3.png)

###  Assumptions  and  Limitations  

- Grades entered should be 0 zero and 100
- Grades can be whole numbers or numbers with decimal points
- Each student should have one grade

## Testing Summary
| Test | What was tested | Expected result | Actual result | Status |
|---|---|---|---|---|
| 1 | 3 students with valid grades were entered | The students should be accepted and stored | All 3 students were accepted and stored | Pass |
| 2 | Input a grade of 60 | The program should accept the grade | The program accepted the grade | Pass |
| 3 | Enter a grade of 109 | The program should reject the grade and ask for a valid one | The program rejected the grade and asked for for an input between 0 and 100 | Pass |
| 4 | Test grade of -18 | The program should reject the grade and ask for another one | The program rejected the grade and asked for another one | Pass |
| 5 | Enter different student names and grades | The total and average should be calculated | The total and average were calculated and displayed | Pass |
| 6 | Enter a student count of 0 | A zero division error | Terminal displayed a zero division error | Pass |
| 7 | Entering a grade of 0 | The program should accept the grade | Grade was accepted | Pass |
| 8 | Entering a grade of 100 | The program should accept the grade | Grade was accepted | Pass |

###  Known  Issues  

When prompted for the number of students and a user enters 0, the program encounters at division by zero error meaning does not handle a student count of 0 when the average is calculated. 

![Zero Division Error](0division.png)

### References
 
 W3Schools Python Tutorials. [W3Schools – Python Tutorial](https://www.w3schools.com/python/)

 ## SECTION B - Managing Student Grades with Lists and Tuples

 ### Features
- Prompt the user to answer the number of students
- Prompt the user to enter the student name
- Prompt the user to enter the math grade, the English grade, and the science grade
- Calculate and display each student’s  average grade
- Display the highest grade for each subject across the class
- Display the lowest grade for each subject across the
- Produce a summary table that show the students name ,the individual subject grade and average
- Validate the grade to ensure it is between 0 and 100

###  Example  Input/Output  
This is a demonstration of how the program runs and the key features implemented.

![P1](sect_b1.png)
![P2](sectb2.png)
![P3](sectb3.png)
![P4](sectb4.png)

###  Assumptions  and  Limitations  

- A student has exactly 3 grades, one for each subject
- Each student has a math grade, English grade, and a science grade.
- Grades are numbers between 0 and 100
- The program uses only the three subjects defined in the subjects list
- The average of each student is calculated using three subject gradeS


## Testing Summary
| Test | What was tested | Expected result | Actual result | Status |
|---|---|---|---|---|
| 1 | 3 students with valid grades were entered | The students should be accepted and stored | All 3 students were accepted and stored | Pass |
| 2 | Input a grade of 60 | The program should accept the grade | The program accepted the grade | Pass |
| 3 | Enter a grade of 109 | The program should reject the grade and ask for a valid one | The program rejected the grade and asked for for an input between 0 and 100 | Pass |
| 4 | Test grade of -18 | The program should reject the grade and ask for another one | The program rejected the grade and asked for another one | Pass |
| 5 | Enter different student names and grades | The total and average should be calculated | The total and average were calculated and displayed | Pass |
| 6 | Enter a student count of 0 | A zero division error | Terminal displayed a zero division error | Pass |
| 7 | Entering a grade of 0 | The program should accept the grade | Grade was accepted | Pass |
| 8 | Entering a grade of 100 | The program should accept the grade | Grade was accepted | Pass |

###  Known  Issues  

When prompted for the number of students and a user enters 0, the program encounters at division by zero error meaning does not handle a student count of 0 when the average is calculated. 

![Zero Division Error](0division.png)

### References
 
 W3Schools Python Tutorials. [W3Schools – Python Tutorial](https://www.w3schools.com/python/)

## SECTION C - Student Management Using Dictonaries

### Features

- Prompts the user to enter number of students
- Prompts the user to enter student names
- Prompts user to enter English, Math, and Science grades
- Prompts the user to enter the name of a new student
- Prompts the user to input the subject grades of a new student
- Allows users to view all the grades of a particular subject
- Allows users to update grades of existing student
- Uses a dictionary to map subject to grade
- Allows the removal of a student by their name
- Allow the user to search for a specific student and view their grade and average

###  Example  Input/Output  
This is a demonstration of how the program runs and the key features implemented.

![P1](sectc1.png)
![P2](sectc2.png)
![P3](sectc3.png)
![P1](sectc5.png)
![P2](sectc4.png)


###  Assumptions  and  Limitations  

- Grades entered should be 0 zero and 100
- Grades can be whole numbers or numbers with decimal points
- Each student should have one grade

## Testing Summary
| Test | What was tested | Expected result | Actual result | Status |
|---|---|---|---|---|
| 1 | 3 students with valid grades were entered | The students should be accepted and stored | All 3 students were accepted and stored | Pass |
| 2 | Input a grade of 60 | The program should accept the grade | The program accepted the grade | Pass |
| 3 | Enter a grade of 109 | The program should reject the grade and ask for a valid one | The program rejected the grade and asked for for an input between 0 and 100 | Pass |
| 4 | Test grade of -18 | The program should reject the grade and ask for another one | The program rejected the grade and asked for another one | Pass |
| 5 | Enter different student names and grades | The total and average should be calculated | The total and average were calculated and displayed | Pass |
| 6 | Enter a student count of 0 | A zero division error | Terminal displayed a zero division error | Pass |
| 7 | Entering a grade of 0 | The program should accept the grade | Grade was accepted | Pass |
| 8 | Entering a grade of 100 | The program should accept the grade | Grade was accepted | Pass |

###  Known  Issues  

When prompted for the number of students and a user enters 0, the program encounters at division by zero error meaning does not handle a student count of 0 when the average is calculated. 

![Zero Division Error](0division.png)

### References
 
 W3Schools Python Tutorials. [W3Schools – Python Tutorial](https://www.w3schools.com/python/)
