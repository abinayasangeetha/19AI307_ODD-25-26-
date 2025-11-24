# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:
Create a class Utility with a static method square(int num) that returns the square of a number. Call the method without creating an object. 

## AIM:
To write a Java program demonstrating access modifiers and static methods by creating a method that can be called without creating an object.

## ALGORITHM :
1. Start the program.
2. Import the java.util package.
3. Create a class Utility with a static method square() that returns num * num.
4. In the main method, create a Scanner object to read an integer.
5. Check if input is an integer; if yes, read the number.
6. Call the static method square() using the class name Utility.
7. Store and display the returned value.
8. Close the Scanner.
9. End the program.

## PROGRAM:
 ```
/*
Program to implement a Access Modifiers using Java
Developed by: ABINAYA S
RegisterNumber: 212222230002
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Utility {
    static int square(int num) {
        return num * num;
    }
}

public class prog {
    public static void main(String[] args) {
       Scanner scanner = new Scanner(System.in);
       if (scanner.hasNextInt()) {
           int inputNumber = scanner.nextInt();
           int result = Utility.square(inputNumber);
           System.out.println(result);
       }
       
       scanner.close();
    }
}
```
## OUTPUT:

<img width="564" height="322" alt="image" src="https://github.com/user-attachments/assets/4c32e1a7-a4d8-4cdb-9293-8d8c7f05caa2" />


## RESULT:
  Thus, the Java program was successfully written and executed to demonstrate access modifiers using a static method that is called without creating an object.
