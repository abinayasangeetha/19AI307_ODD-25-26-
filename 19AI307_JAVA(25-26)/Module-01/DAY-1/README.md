# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:
Lovely wants to learn how Java print statements work.
Write a Java program that:

Takes her name, age, and favorite decimal number

Prints greeting using print()

Prints age using println()

Prints favorite number using printf() with 2 decimal places
## AIM:
To write a Java program that demonstrates the use of variables, data types, operators, and different print statements (print, println, and printf).

## ALGORITHM :
1.Start the program.
2.Create a Scanner object to read input.
3.Read the name (String), age (int), and favorite number (float).
4.Display greeting using System.out.print().
5.Display age using System.out.println().
6.Display favorite number using System.out.printf() formatted to two decimals.
7.End the program.



## PROGRAM:
 ```
/*
Program to implement variables and Operators using Java
Developed by: ABINAYA S
RegisterNumber:  212222230002
*/
```

## Sourcecode.java:
```
import java.util.Scanner;

public class PrintDemo {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String name = sc.nextLine();
        int age = sc.nextInt();
        float favNum = sc.nextFloat();

        System.out.print("Hello, " + name + "\n");
        System.out.println("You are " + age + " years old");
        System.out.printf("Your favorite number is %.2f", favNum);
    }
}
```






## OUTPUT:

<img width="872" height="457" alt="image" src="https://github.com/user-attachments/assets/aa1410fb-d8b6-4ef1-8824-67ce4d255fbe" />


## RESULT:
 Thus, the Java program was successfully written and executed to demonstrate the different printing methods in Java.
