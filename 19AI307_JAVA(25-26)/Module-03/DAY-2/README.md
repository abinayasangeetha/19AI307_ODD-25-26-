# Ex.No:3(b) POLYMORPHISM

## QUESTION:
Write a Java program to create a class MaxFinder with three overloaded max() methods:
max(int a, int b) – returns the maximum of two integers.
max(double a, double b) – returns the maximum of two double values.
max(int a, int b, int c) – returns the maximum of three integers.
In the main() method, demonstrate the use of each overloaded method with various inputs.

## AIM:
To implement compile-time polymorphism (method overloading) in Java by defining multiple max() methods with different parameter lists.

## ALGORITHM :
1. Start the program.
2. Import the java.util package.
3. Create a class MaxFinder with three overloaded max() methods:
      - max(int, int)
      - max(double, double)
      - max(int, int, int)
4. In each method, determine and return the maximum value.
5. In the main method, create a Scanner to read various inputs.
6. Read two integers, two doubles, and three integers from the user.
7. Create an object of MaxFinder.
8. Call each overloaded method using the input values.
9. Print the returned maximum values.
10. End the program.

## PROGRAM:
 ```
/*
Program to implement a Polymorphism using Java
Developed by: ABINAYA S
RegisterNumber:  212222230002
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class MaxFinder {

    public int max(int a, int b) {
        return (a > b) ? a : b;
    }

    public double max(double a, double b) {
        return (a > b) ? a : b;
    }

    public int max(int a, int b, int c) {
        return Math.max(a, Math.max(b, c));
    }
}

class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        MaxFinder mf = new MaxFinder();

        int a1 = sc.nextInt();
        int b1 = sc.nextInt();

        double d1 = sc.nextDouble();
        double d2 = sc.nextDouble();

        int x = sc.nextInt();
        int y = sc.nextInt();
        int z = sc.nextInt();

        System.out.println("Max(" + a1 + ", " + b1 + "): " + mf.max(a1, b1));
        System.out.println("Max(" + d1 + ", " + d2 + "): " + mf.max(d1, d2));
        System.out.println("Max(" + x + ", " + y + ", " + z + "): " + mf.max(x, y, z));
    }
}

```
## OUTPUT:

<img width="978" height="464" alt="image" src="https://github.com/user-attachments/assets/59dc6823-5976-46af-b77d-1b019a404754" />


## RESULT:
   Thus, the Java program was successfully written and executed to demonstrate polymorphism using method overloading.
