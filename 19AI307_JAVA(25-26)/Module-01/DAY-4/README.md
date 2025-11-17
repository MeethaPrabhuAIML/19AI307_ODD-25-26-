# Ex.No:1(D) ARRAYS

## QUESTION:
Write a Java program to count how many elements in an array are divisible by 3 or 5

## AIM:
To write a Java program to count how many elements in an array are divisible by 3 or 5.

## ALGORITHM :
1.	Start the program.

2.	Import the necessary package 'java.util'
   
3.	Get the Total Count The program asks the user for a number (to decide how many numbers to check) and stores it in the n variable.

4. Create an Empty List The program makes an array that is big enough to hold n numbers.

5. Fill the List (First Loop) The program starts a loop that repeats n times. Each time, it asks the user for a number and puts that number into the list.

6. Set Up a Counter The program creates a new variable called count and sets its value to 0. This will be used to count the numbers that match our rule.

7. Check the List (Second Loop) The program starts a second loop. This loop goes through every number in the list, one by one, from start to finish.

8. Check the Rule Inside this second loop, it looks at the current number and checks: Is this number divisible by 3? OR is this number divisible by 5?

9. Increase the Counter If the rule in Step 7 is true (the number is divisible by 3 or 5), the program adds 1 to the count variable.

10 Print the Result After the second loop has finished checking all the numbers in the list, the program prints the final total value of count.

11. Close the program and scanner object.

## PROGRAM:
 ```
/*
Program to implement a Array concept using Java
Developed by: 
RegisterNumber:  
*/
```

## SOURCE CODE:

```
import java.util.*;
public class Main{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int [] arr = new int[n];
        for(int i=0;i<n;i++)
        {
            arr[i] = sc.nextInt();
        }
        int count=0;
        for(int i=0;i<n;i++)
        {
            if(arr[i]%3==0 || arr[i]%5==0)
            {
                count++;
            }
        }
        System.out.println(count);
    }
}
```

## OUTPUT:
<img width="866" height="602" alt="image" src="https://github.com/user-attachments/assets/99c4e21f-e5c8-46a1-9542-ffc14308dc73" />



## RESULT:
Thus, the Java program to count how many elements in an array are divisible by 3 or 5 is implemented using Arrays successfully.

