# Ex.No:3(D)    INTERFACE 

## QUESTION:
Two types of traffic controllers decide whether a vehicle can pass based on signal color. The decision logic varies by controller.
AggressiveController: Allows only if "GREEN".
DefensiveController: Allows for "GREEN" or "YELLOW".
AggressiveController: Allows only if "GREEN".
DefensiveController: Allows for "GREEN" or "YELLOW".

## AIM:
To write a Java program demonstrating interfaces by defining a TrafficController interface and implementing it in two different controller classes with different decision logic.

## ALGORITHM :
1. Start the program.
2. Import the java.util package.
3. Create an interface TrafficController with a method decide().
4. Implement the interface in AggressiveController:
       - Return "GO" only if color is "GREEN".
       - Otherwise return "STOP".
5. Implement the interface in DefensiveController:
       - Return "GO" if color is "GREEN" or "YELLOW".
       - Otherwise return "STOP".
6. In the main method, use Scanner to read the signal color and controller type.
7. If type is 1, create AggressiveController; otherwise create DefensiveController.
8. Call the decide() method and print the result.
9. End the program.

## PROGRAM:
 ```
/*
Program to implement a Interface using Java
Developed by: ABINAYA S
RegisterNumber:  212222230002
*/
```

## SOURCE CODE:
```
import java.util.*;

interface TrafficController {
    String decide(String color);
}

class AggressiveController implements TrafficController {
    public String decide(String color) {
        return color.equals("GREEN") ? "GO" : "STOP";
    }
}

class DefensiveController implements TrafficController {
    public String decide(String color) {
        return (color.equals("GREEN") || color.equals("YELLOW")) ? "GO" : "STOP";
    }
}

class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        String color = sc.next();
        int type = sc.nextInt();

        TrafficController controller;

        if (type == 1)
            controller = new AggressiveController();
        else
            controller = new DefensiveController();

        System.out.println(controller.decide(color));
    }
}
```






## OUTPUT:
   
<img width="726" height="279" alt="image" src="https://github.com/user-attachments/assets/382d71df-12d7-499a-8825-320ad965269f" />


## RESULT:
  Thus, the Java program was successfully written and executed to demonstrate interfaces with two different implementations of traffic control logic.
