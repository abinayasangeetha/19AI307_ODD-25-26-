# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
Write a class Greeting with a method say_hello() which takes a name and returns “Hello <name>, welcome!”.

## AIM:
To write a Java program using classes and objects where a method inside a class returns a greeting message based on user input.

## ALGORITHM :
1. Start the program.
2. Import the java.util package.
3. Create a class with a method say_hello() that accepts a name and returns a greeting message.
4. In the main method, create a Scanner object to read input from the user.
5. Read the user's name as a string.
6. Create an object of the class.
7. Call the say_hello() method using the object and store the returned message.
8. Display the output message.
9. End the program.



## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by: ABINAYA S
RegisterNumber: 212222230002
*/
```

## SOURCE CODE:

```
import java.util.Scanner;

class prog {

    String say_hello(String name) {
        return "Hello " + name + ", welcome!";
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String name = scanner.nextLine();
        prog obj = new prog();
        System.out.println(obj.say_hello(name));
    }
}

```
## OUTPUT:

<img width="754" height="327" alt="image" src="https://github.com/user-attachments/assets/993f0979-8bc2-4e51-8e6a-dbf2a3b3ee1c" />


## RESULT:
    Thus, the Java program using classes and objects was successfully written and executed to display a greeting message.
