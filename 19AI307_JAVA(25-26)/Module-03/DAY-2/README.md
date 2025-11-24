# Ex.No:3(b) POLYMORPHISM

## QUESTION:
Write a Java program to:

Create a base class Shape with methods draw() and calculateArea().

Create two subclasses:

Circle: overrides draw() and calculateArea() to handle a circle.

Cylinder: overrides draw() and overrides calculateArea() to calculate the total surface area of the cylinder 

Take input from the user to choose between circle and cylinder, and input relevant dimensions.

## AIM:
To write a Java program to calculate the area of a Circle or the total surface area of a Cylinder using inheritance and method overriding.

## ALGORITHM :
1.	Start the program.
  
2.	Import the necessary package 'java.util'

3. Create a base class Shape with methods draw() and calculateArea().

4. Create a subclass Circle that extends Shape. It calculates area using the formula: 3.14 * radius * radius.

5. Create a subclass Cylinder that extends Shape. It calculates total surface area using the formula: 2 * 3.14 * radius * (radius + height).

6. The program asks the user to choose between "Circle" or "Cylinder".

7. If the user chooses "Circle", the program asks for the radius, creates a Circle object, and prints the area.

8. If the user chooses "Cylinder", the program asks for the radius and height, creates a Cylinder object, and prints the total surface area.

9. Close the scanner object and end the program.





## PROGRAM:
 ```
/*
Program to implement a Polymorphism using Java
Developed by: MEETHA PRABHU
RegisterNumber: 212222240065 
*/
```

## SOURCE CODE:
```
import java.util.Scanner;
import java.text.DecimalFormat;

abstract class Shape {
    public abstract void draw();
    public abstract double calculateArea();
}

class Circle extends Shape {
    double radius;

    public Circle(double radius) {
        this.radius = radius;
    }

    @Override
    public void draw() {
        System.out.println("Drawing a circle...");
    }

    @Override
    public double calculateArea() {
        return Math.PI * radius * radius;
    }
}

class Cylinder extends Shape {
    double radius;
    double height;

    public Cylinder(double radius, double height) {
        this.radius = radius;
        this.height = height;
    }

    @Override
    public void draw() {
        System.out.println("Drawing a cylinder...");
    }

    @Override
    public double calculateArea() {
        double baseArea = Math.PI * radius * radius;
        double lateralArea = 2 * Math.PI * radius * height;
        return (2 * baseArea) + lateralArea;
    }
}

public class ShapeDemo {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        DecimalFormat df = new DecimalFormat("0.00");
        Shape myShape;

        //System.out.print("Enter shape type (circle / cylinder): ");
        String shapeType = scanner.nextLine().trim();

        if (shapeType.equalsIgnoreCase("circle")) {
            //System.out.print("Enter the radius of the circle: ");
            double radius = scanner.nextDouble();
            myShape = new Circle(radius);

        } else if (shapeType.equalsIgnoreCase("cylinder")) {
            //System.out.print("Enter the radius of the cylinder: ");
            double radius = scanner.nextDouble();
            //System.out.print("Enter the height of the cylinder: ");
            double height = scanner.nextDouble();
            myShape = new Cylinder(radius, height);

        } else {
            System.out.println("Invalid shape type.");
            scanner.close();
            return;
        }

        myShape.draw();
        double area = myShape.calculateArea();
        System.out.println("Area: " + df.format(area));

        scanner.close();
    }
}

```
## OUTPUT:
<img width="632" height="332" alt="image" src="https://github.com/user-attachments/assets/58e01d38-545d-43bd-ab73-0c51e7ac3a73" />



## RESULT:
Thus, the program to calculate the area of a Circle and total surface area of a Cylinder using inheritance and method overriding was executed successfully.
