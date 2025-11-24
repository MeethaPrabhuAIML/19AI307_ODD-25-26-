# Ex.No:3(E) INNER CLASS

## QUESTION:
 Write a Java program where the inner class is declared private and accessed through a method in the outer class. 

## AIM:
To write a Java program to demonstrate the usage of a private inner class within an outer class to encapsulate data.

## ALGORITHM :
1.	Start the program.
   
2.	Import the necessary package 'java.util'
   
3. Create an Outer class containing a private Inner class.

4. The Inner class constructor initializes the data variable.

5. The Outer class has a method innercallingmethod to create an object of the Inner class and print the data.

6. The Main class reads an integer input from the user.

7. Create an object of the Outer class.

8. Call the innercallingmethod to pass the input data to the inner class and display it.

9. Close the scanner object and end the program.	





## PROGRAM:
 ```
/*
Program to implement a InnerClass using Java
Developed by: MEETHA PRABHU
RegisterNumber: 212222240065   
*/
```

## SOURCE CODE:
```
import java.util.*;
class Outer
{
    private class Inner
    {
        int data;
        Inner(int data)
        {
            this.data=data;
        }
    }
    void innercallingmethod(int data)
    {
        Inner in=new Inner(data);
        System.out.println("Data set inside private inner class: "+data);
    }
}
public class Main
{
    public static void main(String[] args)
    {
        Scanner in=new Scanner(System.in);
        int data=in.nextInt();
        Outer out=new Outer();
        out.innercallingmethod(data);
    }
}
```

## OUTPUT:
<img width="947" height="298" alt="image" src="https://github.com/user-attachments/assets/7be13238-4d81-4a21-a33d-541fccfc696e" />



## RESULT:
Thus, the program to demonstrate the usage of a private inner class within an outer class was executed successfully.
