# Ex.No:3(F) WRAPPER CLASS

## QUESTION:
Find the largest digit in a number using wrapper class methods.

## AIM:
To write a Java program to find the largest digit in a given number using Wrapper class methods.

## ALGORITHM :
1.	Start the program.

2.	Import the necessary package 'java.util'

3.	The program waits for the user to input an integer number.

4. The program calls the findLargestDigit method to process the number.

5. Inside the method, convert the number to a string using the Integer.toString() method.

6. Iterate through each character of the string and convert it back to a numeric digit using Character.getNumericValue().

7. Compare the current digit with the maximum found so far using Integer.max().

8. The program prints the largest digit found.

9. Close the scanner object and end the program.





## PROGRAM:
 ```
/*
Program to implement a Wrapper Class using Java
Developed by: MEETHA PRABHU
RegisterNumber:  212222240065
*/
```

## SOURCE CODE:
```
import java.util.Scanner; 

public class LargestDigitWrapperInput {

    public static void main(String[] args) {
        
        
        Scanner scanner = new Scanner(System.in);

       
        int number = scanner.nextInt();

     
        int largest = findLargestDigit(number);

        
        System.out.println("The largest digit is: " + largest);
        
     
        scanner.close();
    }

    /**
     * Finds the largest digit in a number using wrapper class methods.
     * (This function is unchanged)
     */
    public static int findLargestDigit(int num) {
     
        String numString = Integer.toString(num);

        int maxDigit = 0; 

        
        for (char c : numString.toCharArray()) {
            
          
            int digit = Character.getNumericValue(c);

           
            maxDigit = Integer.max(maxDigit, digit);
        }

        return maxDigit;
    }
}
```






## OUTPUT:
<img width="652" height="302" alt="image" src="https://github.com/user-attachments/assets/5e338b35-0afe-48e3-ba49-412e87bfc33e" />



## RESULT:
Thus, the program to find the largest digit in a number using Wrapper class methods was executed successfully.
