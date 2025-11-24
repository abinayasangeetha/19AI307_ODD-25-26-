# Ex.No:5(C)  FILE HANDLING USING JAVA
## QUESTION:
Write a program to write multiple lines to a file using FileWriter.The input continues until the user types "exit".After writing, print:File written successfully to multilines.txt

## AIM:
To write a Java program that demonstrates file handling by writing multiple lines of text to a file using the FileWriter class.

## ALGORITHM :
1. Start the program.
2. Import java.io and java.util packages.
3. Create a Scanner object to read user input.
4. Create a FileWriter object to write into "multilines.txt".
5. Start a loop to read lines from the user.
6. If the user types "exit", break the loop.
7. Otherwise, write the line to the file followed by a newline character.
8. Close the FileWriter after writing all lines.
9. Display a success message.
10. Handle exceptions using try–catch.
11. End the program.

## PROGRAM:
 ```
/*
Program to implement a File Handling using Java
Developed by: ABINAYA S
RegisterNumber:  212222230002
*/
```

## SOURCE CODE:
```
import java.io.*;
import java.util.*;

public class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        try {
            FileWriter fw = new FileWriter("multilines.txt");
            while (true) {
                String line = sc.nextLine();
                if (line.equals("exit"))
                    break;
                fw.write(line + "\n");
            }
            fw.close();
            System.out.println("File written successfully to multilines.txt");
        } catch (Exception e) {
            System.out.println(e);
        }
    }
}
```
## OUTPUT:
<img width="1069" height="261" alt="image" src="https://github.com/user-attachments/assets/bd3312f5-e7db-46ff-bedb-799cdae2b4a7" />



## RESULT:
  Thus, the Java program was successfully written and executed to demonstrate file handling by writing multiple lines to a file using FileWriter.
