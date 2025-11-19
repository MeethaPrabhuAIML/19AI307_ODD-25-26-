# Ex.No:1(E) STRINGS AND MATH FUNCTION

## QUESTION:
Write a Java program to reverse a given string.

## AIM:
To develop a java program to reverse a string.

## ALGORITHM :
1. Start the program.
    
2. Import the necessary package 'java.util'
   
3. The program asks the user to type in a line of text (a string) and stores it in the str variable.

4. The program creates a new string variable called res and sets its initial value to a single space (" "). This string will hold the reversed text.

5. The program starts a loop. The loop's counter (i) is set to the last position (index) of the input text (str.length() - 1). The loop will continue as long as i is 0 or greater, moving backward one position at a time.

6. Inside the loop, the program gets the single character from the original text (str) at the current position i.

7. The program adds (appends) this single character to the end of the res string.

8. Repeat the Loop The program goes back to Step 4, decreases i by 1 (moves to the previous character), and repeats Steps 5 and 6. This continues until it has added all characters from the original text, from last to first.

9. After the loop is finished, the program prints the text "Reversed string:" followed by the new res string.

10. Close the scanner object and end the program.




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



