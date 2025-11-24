# Ex.No:4(D) DESIGN PATTERN -- ABSTRACT FACTORY

## QUESTION:
You need to clone documents. Implement the Prototype Pattern to copy a Document object with a title and content. On user input, create a copy and print both the original and the clone.

## AIM:
To implement the Prototype Design Pattern in Java by creating a class that supports cloning and demonstrates object duplication.

## ALGORITHM :
1. Start the program.
2. Import the java.util package.
3. Create a Document class that implements Cloneable.
4. Add title and content as instance variables.
5. Implement the clone() method to return a shallow copy of the Document object.
6. Create a print() method to display document details.
7. In the main method, read title and content from the user.
8. Create the original Document object.
9. Clone the original document using the clone() method.
10. Print both the original and cloned documents.
11. End the program.

## PROGRAM:
 ```
/*
Program to implement a Abstract Factory Pattern using Java
Developed by: ABINAYA S
RegisterNumber: 212222230002
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Document implements Cloneable {
    private String title;
    private String content;

    public Document(String title, String content) {
        this.title = title;
        this.content = content;
    }

    public Document clone() {
        try {
            return (Document) super.clone();
        } catch (CloneNotSupportedException e) {
            return null;
        }
    }

    public void print() {
        System.out.println(title + " - " + content);
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String title = sc.nextLine();
        String content = sc.nextLine();
        
        Document original = new Document(title, content);
        Document cloned = original.clone();
        
        System.out.print("Original: ");
        original.print();
        System.out.print("Cloned: ");
        cloned.print();
        
        sc.close();
    }
}
```

## OUTPUT:

<img width="1244" height="350" alt="image" src="https://github.com/user-attachments/assets/390b834f-3587-4917-b420-76339b19003a" />

## RESULT:
  Thus, the Java program was successfully written and executed to demonstrate the Prototype Design Pattern by cloning a Document object and displaying both the original and cloned copies.
