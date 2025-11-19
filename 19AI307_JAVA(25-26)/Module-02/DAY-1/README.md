# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
Create a class Vehicle with attributes as number, type and owner.

## AIM:
To create a class Vehicle with attributes as number, type and owner.

## ALGORITHM :
1.	Start the program.
   
2.	Import the necessary package 'java.util'
   
3. Create the First Vehicle Object The program creates a new vehicle object called v1. This is the first "container" to hold vehicle details.

4. Get Input for First Vehicle The program waits for the user to type three things: the vehicle number, the vehicle type, and the owner's name. It saves these details into the v1 object.

5. Create the Second Vehicle Object The program creates another new vehicle object called v2. This is the second "container" to hold different details.

6. Get Input for Second Vehicle The program waits for the user to type three more things: a new vehicle number, type, and owner. It saves these details into the v2 object.

7. Print First Vehicle Details The program takes the information stored inside v1 and prints it out in a specific format (Number | Type | Owner).

8. Print Second Vehicle Details The program takes the information stored inside v2 and prints it out in the same format.

9. Close the scanner object and end the program.





## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by: MEETHA PRABHU
RegisterNumber: 212222240065
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Vehicle {
    String number;
    String type;
    String owner;

    void printVehicle() {
        System.out.println(number + " | " + type + " | " + owner);
    }
}

class prog {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        Vehicle v1 = new Vehicle();
        v1.number = scanner.next();
        v1.type = scanner.next();
        v1.owner = scanner.next();

        Vehicle v2 = new Vehicle();
        v2.number = scanner.next();
        v2.type = scanner.next();
        v2.owner = scanner.next();

        v1.printVehicle();
        v2.printVehicle();
        scanner.close();
    }
}
```






## OUTPUT:
<img width="1237" height="351" alt="image" src="https://github.com/user-attachments/assets/643fed08-f5be-4f03-a77c-c212572277dd" />



## RESULT:
Thus, the program to create an object is implemented successfully.
