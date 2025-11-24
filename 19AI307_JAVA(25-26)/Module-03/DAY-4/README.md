# Ex.No:3(D)    INTERFACE 

## QUESTION:
Schools use different grading schemes. You need to build a system to plug different strategies.

SimpleGrader: A: 90+, B: 75–89, C: 60–74, F: below 60

StrictGrader: A: 95+, B: 85–94, C: 70–84, F: below 70

Input Format:
marks
graderType
marks: Integer (0–100)

graderType: 1 for SimpleGrader, 2 for StrictGrader

## AIM:
To write a Java program to calculate the student's grade using different grading strategies (Simple and Strict) based on the marks obtained.

## ALGORITHM :
1.	Start the program.
   
2.	Import the necessary package 'java.util'

3. Create a base class Grader with an abstract method getGrade().

4. Create a subclass SimpleGrader that assigns grades based on standard ranges (A: 90+, B: 75+, C: 60+, F: <60).

5. Create a subclass StrictGrader that assigns grades based on stricter ranges (A: 95+, B: 85+, C: 70+, F: <70).

6. The program waits for the user to input the marks and the grader type (1 for Simple, 2 for Strict).

7. If the type is 1, create a SimpleGrader object.

8. If the type is 2, create a StrictGrader object.

9. The program calls the getGrade() method and prints the resulting grade.

10. Close the scanner object and end the program.





## PROGRAM:
 ```
/*
Program to implement a Interface using Java
Developed by: MEETHA PRABHU
RegisterNumber: 212222240065
*/
```

## SOURCE CODE:
```

import java.util.Scanner;

interface Grader {
    char getGrade(int marks);
}

class SimpleGrader implements Grader {
    public char getGrade(int marks) {
        if (marks >= 90) return 'A';
        else if (marks >= 75) return 'B';
        else if (marks >= 60) return 'C';
        else return 'F';
    }
}

class StrictGrader implements Grader {
    public char getGrade(int marks) {
        if (marks >= 95) return 'A';
        else if (marks >= 85) return 'B';
        else if (marks >= 70) return 'C';
        else return 'F';
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int marks = sc.nextInt();
        int graderType = sc.nextInt();

        Grader grader;

        if (graderType == 1)
            grader = new SimpleGrader();
        else
            grader = new StrictGrader();

        System.out.println(grader.getGrade(marks));
    }
}

```







## OUTPUT:
<img width="388" height="215" alt="image" src="https://github.com/user-attachments/assets/411636fd-356d-47d7-971c-badb790ceeaf" />



## RESULT:
Thus, the program to calculate the student's grade using different grading strategies was executed successfully.
