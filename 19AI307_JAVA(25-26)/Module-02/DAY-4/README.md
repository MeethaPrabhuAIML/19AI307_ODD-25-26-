# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write a class Rectangle using parameterized constructor and calculate area.

## AIM:
To create a class using parameterized constructor to calculate the area of a rectangle.

## ALGORITHM :
1.	Start the program.

2.	Import the necessary package 'java.util'

3. The program waits for the user to type the length and width values and stores them in variables.

4. The program creates a new Rectangle object called r by passing these length and width values to the constructor to initialize the object.

5. The program calculates the area using the area() method inside the object and prints the result "Area of the rectangle: " followed by the value.

6. Close the scanner object and end the program.	





## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: 
RegisterNumber:  
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class Rectangle {
double l;
double w;

Rectangle(double l, double w) {
    this.l = l;
    this.w = w;
}

double area() {
    return l * w;
}

public static void main(String[] args) {
    Scanner s = new Scanner(System.in);
    double l = s.nextDouble();
    double w = s.nextDouble();
    Rectangle r = new Rectangle(l, w);
    System.out.println("Area of the rectangle: " + r.area());
    s.close();
}


}
```





## OUTPUT:
<img width="741" height="410" alt="image" src="https://github.com/user-attachments/assets/54b6b4df-58a6-4e68-a36d-63693dd47f58" />



## RESULT:
Thus, the program to create a class with paramterized constructor is implemented successfully.
