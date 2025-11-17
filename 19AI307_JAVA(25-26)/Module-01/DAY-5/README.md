# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to reverse a given string.

## AIM:
To develop a java program to reverse a string.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	





## PROGRAM:
 ```
/*
Program to implement a Strings and Math Function using Java
Developed by: MEETHA PRABHU
RegisterNumber: 212222240065
*/
```

## SOURCE CODE:
```
import java.util.*;
public class Main{
    public static void main(String[] args)
    {
        Scanner sc =new Scanner(System.in);
        String str = sc.nextLine();
        String res=" ";
        for(int i=str.length()-1;i>=0;i--)
        {
            char ch = str.charAt(i);
            res+=ch;
        }
        System.out.println("Reversed string:"+res);
    }
}
```
## OUTPUT:
<img width="867" height="342" alt="image" src="https://github.com/user-attachments/assets/7af907c1-9c2f-4444-af5e-997e8208784a" />


## RESULT:
Thus, the java program to reverse a string is implemented using String operation sucessfully.
