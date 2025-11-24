# Ex.No:3(A) INHERITANCE AND AGGREGATION

## QUESTION:
Design a system to manage student assignments using inheritance.
Super Class: Student
studentId
studentName
Sub Class: Assignment
assignmentId
title
submissionDate

grade (–1 means "Not graded")

The system should accept inputs for a student and their assignment, then display all details.
If grade = –1, print "Not graded"; otherwise print the grade.

## AIM:
To write a Java program that demonstrates inheritance by deriving an Assignment class from a Student class and displaying all assignment details including grade status.

## ALGORITHM :
1. Start the program.
2. Import the java.util package.
3. Create a superclass Student with attributes studentId and studentName.
4. Create a subclass Assignment extending Student with assignment details.
5. Add a display() method in Assignment to print all details.
6. In the main method, create a Scanner object to accept input values.
7. Read student and assignment details from the user.
8. Store these values in an Assignment object.
9. Call the display() method to print details.
10. End the program.

## PROGRAM:
 ```
/*
Program to implement a Inheritance and Aggregation using Java
Developed by: ABINAYA S
RegisterNumber: 212222230002
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Student {
    String studentId;
    String studentName;
}

class Assignment extends Student {
    String assignmentId;
    String title;
    String submissionDate;
    int grade; 

    public void display() {
        System.out.println("Student ID: " + studentId);
        System.out.println("Student Name: " + studentName);
        System.out.println("Assignment ID: " + assignmentId);
        System.out.println("Title: " + title);
        System.out.println("Submission Date: " + submissionDate);

        if (grade == -1)
            System.out.println("Grade: Not graded");
        else
            System.out.println("Grade: " + grade);
    }
}

class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Assignment a = new Assignment();

        a.studentId = sc.nextLine();
        a.studentName = sc.nextLine();
        a.assignmentId = sc.nextLine();
        a.title = sc.nextLine();
        a.submissionDate = sc.nextLine();
        a.grade = sc.nextInt();

        a.display();
    }
}

```
## OUTPUT:

<img width="910" height="689" alt="image" src="https://github.com/user-attachments/assets/99a3fe03-6d74-4177-8a86-fe86a6835d72" />


## RESULT:
   Thus, the Java program was successfully written and executed using inheritance to manage and display student assignment details.
