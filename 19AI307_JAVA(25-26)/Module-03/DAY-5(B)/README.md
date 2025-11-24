# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
Write a Java program to reverse a number using the Integer wrapper class and compare it with the original number to check whether it is a palindrome.
## AIM:
To write a Java program that uses the Integer wrapper class and String operations to reverse a number and determine if the number is a palindrome.

## ALGORITHM :
1. Start the program.
2. Import the java.util package.
3. Read an integer input from the user.
4. Convert the integer to a string using Integer.toString().
5. Reverse the string using StringBuilder.
6. Compare the original and reversed strings.
7. If both are equal, print that the number is a palindrome.
8. If not equal, print that it is not a palindrome and display the reversed number.
9. End the program.

## PROGRAM:
 ```
/*
Program to implement a Wrapper Class using Java
Developed by: ABINAYA S
RegisterNumber:  212222230002
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        String original = Integer.toString(num);
        String reversed = new StringBuilder(original).reverse().toString();

        if (original.equals(reversed)) {
            System.out.println(num + " is a palindrome number.");
        } else {
            System.out.println(num + " is not a palindrome number.");
            System.out.println("Reversed Number: " + reversed);
        }
    }
}
```

## OUTPUT:

<img width="942" height="347" alt="image" src="https://github.com/user-attachments/assets/61eaf674-2aa7-4c05-aaf7-7e79f8273e4c" />


## RESULT:
  Thus, the Java program was successfully written using the Wrapper Class to check whether a number is a palindrome by reversing it and comparing it with the original.
