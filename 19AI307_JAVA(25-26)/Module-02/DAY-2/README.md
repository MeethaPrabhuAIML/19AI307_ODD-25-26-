# Ex.No:2(B) METHODS

## QUESTION:
Create two methods:
Get the input for radius from the user.
double getArea(double r) → calculate the area and return the area(Don't print anything in this method).
void printArea(double area) → pass the calculated area to this method and print the area of a circle.

## AIM:
To create methods to calculate the area of the circle.

## ALGORITHM :
1.	Start the program.

2. Import the necessary package 'java.util'

3. The program asks the user to enter a number (decimal or integer) for the radius and stores it in the radius variable.
   
4. The program calls a function named getArea. It sends the radius to this function, which calculates the area using the formula ($3.14 \times radius \times radius$) and returns the result.

5. The program calls another function named printArea. It sends the calculated area to this function, which prints the value formatted to exactly 2 decimal places.

6. Close the scanner object and end the program.



## PROGRAM:
 ```
/*
Program to implement a Methods using Java
Developed by: MEETHA PRABHU
RegisterNumber: 212222240065
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class Main {

    static double getArea(double r) {
        return 3.14 * r * r; 
    }

    
    static void printArea(double area) {
        System.out.printf("%.2f%n", area); 
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double radius = sc.nextDouble(); 
        double area = getArea(radius);  
        printArea(area);                
        sc.close();
    }
}

```


## OUTPUT:
<img width="515" height="272" alt="image" src="https://github.com/user-attachments/assets/a38700d8-5f3b-40df-b484-8f5e6fbba2ad" />



## RESULT:
Thus, the program to create methods to calculate the area of circle is implemented successfully.
