# Ex.No:5(D) THREAD PRIORITY

## QUESTION:
Write a Java program to set the priority and name of the current thread.
The thread name should be read from the user, and the priority should be set to 2.

## AIM:
To write a Java program that demonstrates how to modify the current thread’s name and priority using Thread class methods.

## ALGORITHM :
1. Start the program.
2. Import the java.util package.
3. Read the thread name from the user.
4. Get the reference to the current thread using Thread.currentThread().
5. Set the name of the thread using setName().
6. Set the priority of the thread using setPriority(2).
7. Print the thread’s priority.
8. Print the thread’s name.
9. Print the entire thread object to show its state.
10. End the program.

## PROGRAM:
 ```
/*
Program to implement a Thread Priority Concept using Java
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

        String name = sc.nextLine();      

        Thread t = Thread.currentThread();  
        t.setName(name);                    
        t.setPriority(2);                   

        System.out.println("Priority of Thread: " + t.getPriority());
        System.out.println("Name of Thread: " + t.getName());
        System.out.println(t);              
    }
}

```
## OUTPUT:

<img width="834" height="270" alt="image" src="https://github.com/user-attachments/assets/81bcfd3e-3b3a-4f1c-aa9e-febdcb4a76aa" />


## RESULT:
  Thus, the Java program was successfully written and executed to set and display the current thread's name and priority.
