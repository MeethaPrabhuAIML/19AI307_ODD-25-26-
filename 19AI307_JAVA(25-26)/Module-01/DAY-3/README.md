# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:
A left-aligned triangle pattern is a pattern of stars (*) where each row contains an increasing number of stars, aligned to the left side.

Write a Java program that:

Prompts the user to enter the number of rows for the triangle.

Uses nested loops to print the left-aligned triangle pattern.

Ensures that each row contains stars corresponding to its row number.


## AIM:
To print a left-aligned triangle pattern is a pattern of stars (*) where each row contains an increasing number of stars, aligned to the left side.

## ALGORITHM :
1.	Start the program.
   
2.	Import the necessary package 'java.util'
     
4.	Get the Number of Rows The program asks the user to type in a number and stores it in the rows variable. This number will be the total height of the triangle.

5. Start the Main Row Loop (Outer Loop) The program starts a loop that controls the rows (lines). It uses a counter i, which starts at 1 and will continue as long as i is less than or equal to the rows number.

6. Start the Printing Loop (Inner Loop) Inside the main loop, another loop begins. This one controls what is printed on the current line. It uses a counter j, which starts at 1 and continues as long as j is less than or equal to the current value of i.

7. Print an Asterisk Inside this inner loop, the program prints one asterisk and a space ("* "). This step will repeat i times (e.g., on row 3, it prints 3 asterisks).

8. Move to the Next Line When the inner loop (Step 4 and 5) is completely finished for that row, the program prints a newline. This moves the printing to the start of the next line.

9. Repeat for the Next Row The program goes back to Step 3 to start the next row (by increasing i by 1). This whole process repeats until i is greater than rows.



## PROGRAM:
 ```
/*
Program to implement a Looping Statement using Java
Developed by: MEETHA PRABHU
RegisterNumber: 212222240065
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class ReverseNumber {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int rows = sc.nextInt();

        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print("* ");
            }
            System.out.println();
        }

        sc.close();
    }
}
```

## OUTPUT:
<img width="892" height="553" alt="image" src="https://github.com/user-attachments/assets/4d79ed95-17c5-48b5-90ac-22cdaab30c1b" />



## RESULT:
Thus, the program to print a left-aligned triangle pattern of stars (*) using looping statement is implemented successfully.

