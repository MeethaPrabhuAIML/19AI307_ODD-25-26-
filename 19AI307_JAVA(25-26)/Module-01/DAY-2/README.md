# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:
Given a month number (1 to 12), print which quarter of the year it belongs to:

Months 1,2,3 → "First Quarter"

Months 4,5,6 → "Second Quarter"

Months 7,8,9 → "Third Quarter"

Months 10,11,12 → "Fourth Quarter"
If the number is not in 1-12, print "Invalid Month".

## AIM:
To develop a java program to get the month from user and and display appropriate output for the given input.

## ALGORITHM :
1. Start the program

2. Import necessary java modules java.util

3. Get the Month Number The program asks the user to type in a number and stores it in the variable v.

4. Check for First Quarter It checks if the number v is between 1 and 3. If it is, the program prints "First Quarter".

5. Check for Second Quarter If the first check failed, the program then checks if v is between 4 and 6. If it is, it prints "Second Quarter".

6. Check for Third Quarter If the previous checks failed, the program then checks if v is between 7 and 9. If it is, it prints "Third Quarter".

7. Check for Fourth Quarter If the previous checks failed, the program then checks if v is between 10 and 12. If it is, it prints "Fourth Quarter".

8. Handle Invalid Numbers If the number v was not between 1 and 12 (meaning all the checks above failed), the program prints "Invalid Month".
   
9. Close the program and scanner object. 



## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: MEETHA PRABHU
RegisterNumber: 212222240065
*/
```

## SOURCE CODE:
```
import java.util.*;
public class Main{
    public static void main(String[] args){
        int v = new Scanner(System.in).nextInt();
        
        if(v>=1 && v<=3){
            System.out.println("First Quarter");
        }
        else if(v>=4 && v<=6){
            System.out.println("Second Quarter");
        }
        else if(v>=7 && v<=9){
            System.out.println("Third Quarter");
        }
        else if(v>=10 && v<=12){
            System.out.println("Fourth Quarter");
        }
        else{
            System.out.println("Invalid Month");
        }
    }
}
```
## OUTPUT:
<img width="872" height="267" alt="image" src="https://github.com/user-attachments/assets/8bfa02a6-d5c7-4bcc-9920-c8b38b51e3a9" />

## RESULT:
Thus, the program to generate the name of the month using conditional statement is implemented successfully.


