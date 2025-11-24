# Ex.No:3(C) ABSTRACTION

## QUESTION:
Create abstract class GameScore with method finalScore().
Subclasses:

ArcadeGame: score = baseScore + (level × 100)

PuzzleGame: score = (attempts ≤ 3) ? 1000 - (attempts × 100) : 500

## AIM:
To write a Java program to calculate the final score for an Arcade Game or a Puzzle Game using abstract classes and polymorphism.

## ALGORITHM :
1.	Start the program.
   
2.	Import the necessary package 'java.util'

3. Create an abstract class GameScore with an abstract method finalScore().

4. Create a subclass ArcadeGame that extends GameScore and calculates the score using the formula: $base + (level \times 100)$.

5. Create a subclass PuzzleGame that extends GameScore and calculates the score based on attempts (higher score for fewer attempts).

6. The program waits for the user to input the game type (1 for Arcade, others for Puzzle).If the type is 1, the program reads the base score and level, then creates an ArcadeGame object.

7. Otherwise, the program reads the number of attempts and creates a PuzzleGame object.

8. The program calls the finalScore() method of the created object and prints the result.

9. Close the scanner object and end the program.






## PROGRAM:
 ```
/*
Program to implement a Abstraction using Java
Developed by: MEETHA PRABHU
RegisterNumber:  212222240065
*/
```

## SOURCE CODE:
```
import java.util.*;
abstract class GameScore
{
    abstract int finalScore();
}
class ArcadeGame extends GameScore
{
    int base,level;
    ArcadeGame(int base,int level)
    {
        this.base=base;
        this.level=level;
    }
    int finalScore()
    {
        return base+(level*100);
    }
    
}
class PuzzleGame extends GameScore
{
    int attempts;
    PuzzleGame(int attempts)
    {
        this.attempts=attempts;
    }
    int finalScore()
    {
        return (attempts<=3) ? 1000-(attempts*100):500;
    }
}
public class Main
{
    public static void main(String[] args)
    {
        Scanner sc=new Scanner(System.in);
        int type=sc.nextInt();
        GameScore game;
        if(type==1)
        {
            int base=sc.nextInt();
            int level=sc.nextInt();
            game=new ArcadeGame(base,level);
        }
        else
        {
            int attempts=sc.nextInt();
            game=new PuzzleGame(attempts);
        }
        System.out.println(game.finalScore());
    }
}
```






## OUTPUT:
<img width="398" height="261" alt="image" src="https://github.com/user-attachments/assets/eee73ac2-700b-4bac-bcd7-b15c58520051" />


## RESULT:
Thus, the program to calculate the final score for an Arcade Game or a Puzzle Game using abstract classes and polymorphism was executed successfully.


