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
| 1 | Entering grade 0 | The students should be accepted and stored | All 3 students were accepted and stored | Pass |
| 2 | Entering grade 100 | The program should accept the grade | The program accepted the grade | Pass |
| 3 | Entering grade 108 | The program should reject the grade and ask for a valid one | The program rejected the grade and asked for for an input between 0 and 100 | Pass |
| 4 | Test grade of -2 | The program should reject the grade and ask for another one | The program rejected the grade and asked for another one | Pass |
| 5 | Inputting multiple students | The program should accept all the students and store them| All students are stored | Pass |
| 6 | Calculating average | The student's average should be calculated and displayed | The correct average is shown | Pass |
| 7 |Finding the highest grade| The program should display the highest grade for each subject | The  max() fuction displays the highest subject grades | Pass |
| 8 | Finding the lowest grade | The program should display the lowest grade for each subject | The  min() fuction displays the lowest subject grades | Pass |
| 9 | Display summary table | The summary table should clearly show each student's name, individual subject grades, and their average | The summary table displayed the students name, math, English, and science, math, and the average | Pass |

###  Known  Issues  

- If 0 students are entered, then the program has no grades to add to the subject list, so the max and min functions can’t work with the empty list.

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

- Each student has one grade for each subject.
- The user is expected to enter an existing students name when they are viewing grades or searching for a student.
- The user inputs a valid subject when updating or viewing grades.
- Grades are xpected to be values between 0 and 100.
- Names with special characters should be allowed.
- The program uses the students name to identify and access as their grades.

## Testing Summary
| Test | What was tested | Expected result | Actual result | Status |
|---|---|---|---|---|
| 1 | Entering a name that contains special characters | If the name is entered as text, the program should accept it | The program accepted the name with a special character | Pass |
| 2 | Searching for a nonexistent student | The program should display student not found |The program displayed student not found | Pass |
| 3 | Adding new student | New student should be added without problems | The new student is added to the students dictionary | Pass |
| 4 | Entering a grade above 100 or below 0 | The program must prompt the user to enter a valid grade | The program asks the user to input in a grade between 0 and 100 | Pass |
| 5 | Updating an existing students grade | The specified subject grade should be replaced | TThe selected subject grade is replaced with the new grade | Pass |
| 6 | Searching for nonexistent subject | Program should output a message asking the user to enter a valid subject | Program prompted the user to enter a valid subject | Pass |

###  Known  Issues  

- At the start, grades above 100 and below 0  were accepted and this was fixed by adding a loop to validate the grades.
- Originally, the student biology wishes not in the list was accepted, adding a loop ensures only Math, English, or Science were entered
- Entering a name, but accidentally leaving a trailing space caused the student to be stored under a different dictionary, this resulted in “student not found” later when trying to remove names or search. strip() was added to areas where users were prompted to enter names to prevent this

### References
 
 W3Schools Python Tutorials. [W3Schools – Python Tutorial](https://www.w3schools.com/python/)
