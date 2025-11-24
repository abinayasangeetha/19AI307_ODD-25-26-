# Ex.No:3(C) ABSTRACTION

## QUESTION:
Create an abstract class TaxPayer with method calculateTax(). Create subclasses SalariedPerson and BusinessPerson.

## AIM:
To implement abstraction in Java using an abstract class and its concrete subclasses that define their own tax calculation logic.

## ALGORITHM :
1. Start the program.
2. Import the java.util package.
3. Create an abstract class TaxPayer with an abstract method calculateTax().
4. Create a subclass SalariedPerson that implements calculateTax() to return income * 0.10.
5. Create another subclass BusinessPerson that implements calculateTax() to return income * 0.15.
6. In the main method, create a Scanner object to read input.
7. Read the taxpayer type (1 for salaried, others for business).
8. Read the income.
9. Based on the type, create the appropriate object (SalariedPerson or BusinessPerson).
10. Call calculateTax() on the object and print the result.
11. End the program.

## PROGRAM:
 ```
/*
Program to implement a Abstraction using Java
Developed by: ABINAYA S
RegisterNumber: 212222230002
*/
```

## SOURCE CODE:
```
import java.util.*;

abstract class TaxPayer {
    abstract double calculateTax();
}

class SalariedPerson extends TaxPayer {
    double income;

    SalariedPerson(double income) {
        this.income = income;
    }

    @Override
    double calculateTax() {
        return income * 0.10;   // 10% tax
    }
}

class BusinessPerson extends TaxPayer {
    double income;

    BusinessPerson(double income) {
        this.income = income;
    }

    @Override
    double calculateTax() {
        return income * 0.15;   // assumed 15% tax
    }
}

class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int type = sc.nextInt();
        double income = sc.nextDouble();

        TaxPayer t;

        if (type == 1) {
            t = new SalariedPerson(income);
        } else {
            t = new BusinessPerson(income);
        }

        System.out.printf("%.2f", t.calculateTax());
    }
}
```
## OUTPUT:

<img width="600" height="460" alt="image" src="https://github.com/user-attachments/assets/5bc8c514-be22-43d1-9f51-a9d6f075f38c" />


## RESULT:
  Thus, the Java program was successfully written and executed to demonstrate abstraction using an abstract class and subclass-specific implementations.
