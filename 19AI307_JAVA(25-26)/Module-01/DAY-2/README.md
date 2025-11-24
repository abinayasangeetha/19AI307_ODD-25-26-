# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
Aliens scan DNA numbers using special rules:
If the DNA number is divisible by 2 and ends in 4, they accept it.
If the DNA number is divisible by 2 but ends in anything else, it is a suspect.
If the DNA number is odd, they reject it.
Write a Java program that reads a DNA number and prints one of the following:
Accepted
Suspect
Rejected

## AIM:
To write a Java program that implements conditional statements to check a DNA number and classify it as Accepted, Suspect, or Rejected based on given conditions.

## ALGORITHM :
1.Start the program.

2.Import the Scanner class from the java.util package.

3.Read the DNA number from the user.

4.Check whether the number is even or odd.

5.If the number is odd → print "Rejected".

6.If the number is even, check whether it ends with 4.

7.If it ends with 4 → print "Accepted".

8.Otherwise → print "Suspect".

9.End the program.



## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: ABINAYA S
RegisterNumber:  212222230002
*/
```

## SOURCE CODE:

```
import java.util.*;
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int dna = sc.nextInt();

        if (dna % 2 != 0) {
            System.out.println("Rejected");
        } else {
            if (dna % 10 == 4)
                System.out.println("Accepted");
            else
                System.out.println("Suspect");
        }
    }
}



```





## OUTPUT:

 <img width="571" height="332" alt="image" src="https://github.com/user-attachments/assets/657bfb88-5f42-4334-a08e-8667d391e91a" />



## RESULT:
   Thus, the Java program was successfully written and executed to classify the DNA number using conditional statements.


## RESULT:

