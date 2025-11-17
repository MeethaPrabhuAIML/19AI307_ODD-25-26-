# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:
Lovely wants to enter a secure tech conference. The security system checks certain conditions to grant access. These conditions are:

She must be registered (true/false).

She must have a valid ID (true/false).

She must NOT be blacklisted (true/false).

The system uses logical operators to evaluate her access eligibility:

If she is registered AND has a valid ID, and NOT blacklisted, she is granted access.

Otherwise, access is denied.

Your task is to evaluate these conditions using logical operators and print whether access is granted or denied.

Input Format:
Three boolean values entered by the user (true or false):

<isRegistered>
<hasValidID>
<isBlacklisted>
Output Format:
Access Granted: true/false


## AIM:
To evaluate these conditions using logical operators and print whether access is granted or denied.


## ALGORITHM :
1.Initialize Input System Prepare the program to receive input from the user (this is what Scanner sc = new Scanner(System.in); does).

2.Get Registration Status Read the first boolean (true/false) value from the user and store it in the reg variable. This value represents whether the user is registered.

3.Get ID Status Read the second boolean value from the user and store it in the id variable. This represents whether the user has a valid ID.

4.Get Blacklist Status Read the third boolean value from the user and store it in the blacklisted variable. This represents whether the user is on the blacklist.

5.Evaluate Access Conditions Perform a logical check using all three variables. The program checks if reg is true, AND id is true, AND blacklisted is false.

6.Grant Access If the combined condition in Step 6 is met (all three parts are true), the program will print the message: "Access Granted: true".

7.Deny Access If the combined condition in Step 6 fails (meaning at least one part is not as required), the program will execute the "else" block and print the message: "Access Granted: false".



## PROGRAM:
 ```
/*
Program to implement variables and Operators using Java
Developed by: MEETHA PRABHU
RegisterNumber: 212222240065
*/
```

## Sourcecode.java:
```
import java.util.*;
public class Main{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        boolean reg = sc.nextBoolean();
        boolean id = sc.nextBoolean();
        boolean blacklisted = sc.nextBoolean();
        if(reg==true && id==true && blacklisted==false)
        {
            System.out.println("Access Granted: true");
        }
        else
        {
            System.out.println("Access Granted: false");
        }
    }
}
```

## OUTPUT:
<img width="868" height="392" alt="image" src="https://github.com/user-attachments/assets/783d0957-3e0d-402c-a5b5-23cf65b7173f" />

## RESULT:
Thus, the program to evaluate these conditions using logical operators is implemented successfully.

