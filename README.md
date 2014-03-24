Rock-Paper-Scissor
==================
//  By  REINA OLARTE


import java.util.Scanner; // imports the Scanner class


public class RockPaperScissor
{
public static void main(String[]args)
{
//Create the Scanner input
Scanner input = new Scanner(System.in);

//Create the Random number

//Declaring the variables
//int UserNumber = 0;
int computerNumber;
String UserInput;
String ComputerDecision = "";

computerNumber = 1 + (int)(Math.random() * 3);

System.out.println("Welcome to the Rock, Paper, Scissor's game");
System.out.println("Please type Rock, Paper, or Scissor: ");
UserInput = input.nextLine();

/*if(UserInput.toUpperCase().equals("ROCK"))
{
UserNumber = 1;
}
else if(UserInput.toUpperCase().equals("PAPER"))
{
UserNumber = 2;
}
else if(UserInput.toUpperCase().equals("SCISSOR"))
{
UserNumber = 3;
}

*/
switch(computerNumber)
{
case 1:
ComputerDecision = "rock";
break;
case 2:
ComputerDecision = "paper";
break;
case 3:
ComputerDecision = "scissor";
break;
}

if ((UserInput.toUpperCase().equals("ROCK")) && (ComputerDecision.toUpperCase().equals("ROCK")))
{
System.out.println("Tied");
System.out.printf("You chose %s and computer chose %s", UserInput, ComputerDecision );
}
else if ((UserInput.toUpperCase().equals("ROCK")) && (ComputerDecision.toUpperCase().equals("PAPER")))
{
System.out.println("You Lost");
System.out.printf("You chose %s and computer chose %s", UserInput, ComputerDecision );
}
else if ((UserInput.toUpperCase().equals("ROCK")) && (ComputerDecision.toUpperCase().equals("SCISSOR")))
{
System.out.println("You Won");
System.out.printf("You chose %s and computer chose %s", UserInput, ComputerDecision );
}
else if ((UserInput.toUpperCase().equals("PAPER")) && (ComputerDecision.toUpperCase().equals("PAPER")))
{
System.out.println("Tied");
System.out.printf("You chose %s and computer chose %s", UserInput, ComputerDecision );
}
else if((UserInput.toUpperCase().equals("PAPER")) && (ComputerDecision.toUpperCase().equals("ROCK")))
{
System.out.println("You Won");
System.out.printf("You chose %s and computer chose %s", UserInput, ComputerDecision );
}
else if ((UserInput.toUpperCase().equals("PAPER")) && (ComputerDecision.toUpperCase().equals("SCISSOR")))
{
System.out.println("You Lost");
System.out.printf("You chose %s and computer chose %s", UserInput, ComputerDecision );
}

else if ((UserInput.toUpperCase().equals("SCISSOR")) && (ComputerDecision.toUpperCase().equals("ROCK")))
{
System.out.println("You Lost");
System.out.printf("You chose %s and computer chose %s", UserInput, ComputerDecision );
}

else if ((UserInput.toUpperCase().equals("SCISSOR")) && (ComputerDecision.toUpperCase().equals("PAPER")))
{
System.out.println("You Won");
System.out.printf("You chose %s and computer chose %s", UserInput, ComputerDecision );
}
else if ((UserInput.toUpperCase().equals("SCISSOR")) && (ComputerDecision.toUpperCase().equals("SCISSOR")))
{
System.out.println("Tied");
System.out.printf("You chose %s and computer chose %s", UserInput, ComputerDecision );
}
}   // End method main
}   // End class
