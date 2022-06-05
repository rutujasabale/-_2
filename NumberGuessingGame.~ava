/** Number Guessing Game */
 
import java.util.*;
class NumberGuessingGame 
{
  public static void main(String args[])
  {
    Scanner scan = new Scanner(System.in);
    int random_num, guess, count=0, numberOfTries=1;
    
    System.out.println("*****************************");
    System.out.println("-- Guessing number Game --");
    System.out.println("*****************************");
    
    random_num = 100 - (int)(Math.random()*1);
    System.out.println("Pick a number :");
    
    boolean win = false;
    
    while(win == false){
      guess = scan.nextInt();
      if(numberOfTries < 5)
      {
        if(guess == random_num)
        {
          System.out.println();
          System.out.println("You guess it correctly "+random_num);
          System.out.println("It only took you " +numberOfTries+ " guesses to get it right");
          win = true;
        }
        else if(guess < random_num)
        {
          System.out.println();
          System.out.println("You are too low..!!");
          System.out.println();
          System.out.println("Guess again..");
        }
        else if(guess > random_num)
        {
          System.out.println();
          System.out.println("You are too high..!!");
          System.out.println();
          System.out.println("Guess again..");
        }
      }
      
      else if(numberOfTries == 5)
      {
        if(guess == random_num)
        {
          System.out.println();
          System.out.println("You guess it correctly.."+random_num);
          System.out.println("It only took you " +numberOfTries+ " guesses to get it right");
          win = true;    
        }  
        if(guess != random_num)
        {
          System.out.println();
          System.out.println("Sorry you are out of attempts..\nThe correct answer is "+random_num+ "\nBest luck for next time..!!");
          break;
        }
      }
      numberOfTries = numberOfTries + 1;
    }
  }
}