# Ex.No:5(E) MULTITHREADING -SYNCHRONIZATION

## QUESTION:
Maintain two integer variables a and b, read their initial values from the user, then use a synchronized block to swap them and print the swapped values.

## AIM:
To write a Java program that demonstrates synchronization using a synchronized block to safely swap two variables.

## ALGORITHM :
1. Start the program.
2. Import the java.util package.
3. Read the integer values a and b from the user.
4. Create an object lock for synchronization.
5. Use a synchronized block on the lock object.
6. Inside the block, swap the values of a and b using a temporary variable.
7. After swapping, print the updated values of a and b.
8. End the program.

## PROGRAM:
 ```
/*
Program to implement a Synchronization concept using Java
Developed by: ABINAYA S
RegisterNumber:  212222230002
*/
```

## SOURCE CODE:
```
import java.util.*;

class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int b = sc.nextInt();

        Object lock = new Object();

        synchronized (lock) {
            int temp = a;
            a = b;
            b = temp;
        }

        System.out.println("a = " + a);
        System.out.println("b = " + b);
    }
}
```

## OUTPUT:

<img width="518" height="354" alt="image" src="https://github.com/user-attachments/assets/1580e62e-1efa-4e28-998b-87c9f37b8944" />


## RESULT:
  Thus, the Java program was successfully written and executed to demonstrate synchronization using a synchronized block to safely swap two variables.
