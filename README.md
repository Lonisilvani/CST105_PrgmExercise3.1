/*
 Loni Silvani
CST-105 
March 9th, 2018
Lisa Hebert
This program will run a guessing game. 
 */
package guessmynumber;
import java.util.Scanner;
/**
 *
 * @author lonis
 */
public class GuessMyNumber {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // Begin main method here
        Scanner input = new Scanner(System.in);
        //System.in= System input
        int a = 1 + (int) (Math.random() * 9999),
        guess, 
        count = 0;
        System.out.println("Guess an NUMBER between 1 and 10000"); 

        while((guess = input.nextInt()) != a){
            //loop is created as long as condition is true
        if (guess > a)
            //IF will test the results
     {  
       System.out.println("GO LOWER!");
     }
     else
            //carried out if not true.
     {
       System.out.println("GO HIGHER");
     }
     count++;
     //COUNT++ is an operator that will add one to the variable
   }

   System.out.println("YOU WIN!!!! "+ count +" tries!");
  }

}
