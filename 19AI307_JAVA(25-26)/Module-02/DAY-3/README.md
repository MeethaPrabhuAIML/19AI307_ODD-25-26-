# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:
Write a Java program to create a class called Rectangle with private instance variables length and width. Provide public getter and setter methods to access and modify these variables

## AIM:
To create a class with private instances variable along with getter and setter methods to access and modify the variables.

## ALGORITHM :
1.	Start the program.
   
2.	Import the necessary package 'java.util'

3. The program creates a new Rectangle object called rect. This is the "container" to hold the length and width details.

4. The program waits for the user to type the length value. It saves this detail into the rect object using the setLength method.

5. The program waits for the user to type the width value. It saves this detail into the rect object using the setWidth method.

6. The program retrieves the length information stored inside rect using the getter method and prints it.

7. The program retrieves the width information stored inside rect using the getter method and prints it.

8. Close the scanner object and end the program.





## PROGRAM:
 ```
/*
Program to implement a Access Specifiers using Java
Developed by: MEETHA PRABHU
RegisterNumber: 212222240065
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Rectangle {
    // Private instance variables
    private double length;
    private double width;

    // Getter and Setter for length
    public double getLength() {
        return length;
    }
    public void setLength(double length) {
        this.length = length;
    }

    // Getter and Setter for width
    public double getWidth() {
        return width;
    }
    public void setWidth(double width) {
        this.width = width;
    }

    // Method to calculate area
    public double calculateArea() {
        return length * width;
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Rectangle rect = new Rectangle();

        // Input length and width
        System.out.print("");
        rect.setLength(sc.nextDouble());

        System.out.print("");
        rect.setWidth(sc.nextDouble());

        // Print rectangle details and area
        System.out.println("Length: " + rect.getLength());
        System.out.println("Width: " + rect.getWidth());

        sc.close();
    }
}
```

## OUTPUT:
<img width="720" height="482" alt="image" src="https://github.com/user-attachments/assets/dab984c0-b364-4449-b57a-7123e30f73a6" />



## RESULT:
Thus, the program to create an object with private instance along with getter and setter method is implemented successfully.
