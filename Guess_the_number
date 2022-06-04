//Guess th number using random function//
package com.company;
import java.util.Random;
import java.util.Scanner;
class Game1 {
    public int number;
    public int inputno;
    public int noOfGuess=0;
    Game1() //Number take from Computer//
    {
        Random rand=new Random();
        number=rand.nextInt(100);
    }
    void takeUserInput() //Number take from User//
    {
        System.out.printf("Guess the Number : ");
        Scanner sc=new Scanner(System.in);
        inputno=sc.nextInt();
    }
    boolean isCorrectNumber()
    {
        noOfGuess++;
        if(inputno==number)
        {
            System.out.format("Yes you Guess is right , it was %d \nYou guess it is %d attempt",number,noOfGuess);
            return true;
        }
        else if(inputno<number)
        {
            System.out.println("To Low");
        }
        else if (inputno>number)
        {
            System.out.println("To High");
        }
        return false;
    }
}
public class Game {
    public static void main(String[] arg)
    {
        Game1 g=new Game1();
        boolean b=false; //Initial value is given as False //
        while (!b)
        {
            g.takeUserInput();
            b=g.isCorrectNumber();
        }
        System.out.println(b);
    }
}
