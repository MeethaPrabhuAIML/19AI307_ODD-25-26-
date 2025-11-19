# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:
Write a method that accepts a string and returns whether it contains only lowercase letters or not.

## AIM:
To write a method that checks if the word contains lowercase letters or not.


## ALGORITHM :
1.	Start the program.

2.	Import the necessary package 'java.util'

3. The program waits for the user to type a line of text and stores it in the input variable.

4. The program processes the text using a custom method. It checks every character one by one to see if it is a small letter (between 'a' and 'z').

5. If it finds a character that is not lowercase, the result is false. If all characters are lowercase, the result is true.

6. The program prints the final result (true or false) to the screen.

7. Close the scanner object and end the program.	





## PROGRAM:
 ```
/*
Program to implement a Access Modifiers using Java
Developed by: MEETHA PRABHU
RegisterNumber: 212222240065
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

public class Main {

    // Method to check if string contains only lowercase letters
    static boolean isLowercase(String str) {
        for (int i = 0; i < str.length(); i++) {
            char ch = str.charAt(i);
            if (ch < 'a' || ch > 'z') {
                return false;
            }
        }
        return true;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String input = sc.nextLine();

        boolean result = isLowercase(input);
        System.out.println(result);

        sc.close();
    }
}

```





## OUTPUT:
<img width="408" height="357" alt="image" src="https://github.com/user-attachments/assets/e11e7c76-9734-4d0b-b09f-237b04ba1aaa" />



## RESULT:
Thus, the program to create a method to check the presence of lowercase letters is implemented successfully.
