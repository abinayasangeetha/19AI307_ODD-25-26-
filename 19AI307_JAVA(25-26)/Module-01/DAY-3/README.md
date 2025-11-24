# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:
Write a Java program to count the frequency of digits in a non-negative integer using loops and arrays.

## AIM:
To write a Java program that uses looping statements and an array to count how many times each digit (0 to 9) occurs in a given number.

## ALGORITHM :
1. Start the program.
2. Import the java.util package.
3. Read the input number from the user.
4. Create an array of size 10 to store digit frequencies.
5. If the number is zero, increment the count of digit 0.
6. Use a loop to extract each digit using % 10 and update its frequency.
7. Divide the number by 10 in each iteration until it becomes zero.
8. Loop through the frequency array and print digits that appear at least once.
9. End the program.




## PROGRAM:
 ```
/*
Program to implement a Looping Statement using Java
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
        int n = sc.nextInt();

        int[] freq = new int[10];

        if (n == 0) {
            freq[0] = 1;
        }

        while (n > 0) {
            int digit = n % 10;
            freq[digit]++;
            n /= 10;
        }

        for (int i = 0; i < 10; i++) {
            if (freq[i] > 0) {
                System.out.println("Digit " + i + ": " + freq[i] + " time(s)");
            }
        }
    }
}



```




## OUTPUT:

<img width="675" height="351" alt="image" src="https://github.com/user-attachments/assets/ddb12ff9-ae52-4b4f-9fc1-0231fb6d5893" />



## RESULT:
  Thus, the Java program was successfully written and executed to count the frequency of digits using looping statements.
