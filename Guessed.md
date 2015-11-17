import java.util.*;// imports all java utilities

public class GuessingGame {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

Scanner scan = new Scanner(System.in);
Random r = new Random();
int  num;
String a;
int answer, companswer;
answer = (int) Math.floor(Math.random()*30+1);//sets the int to a random number from 1-30
companswer = (int) Math.floor(Math.random()*30+1);//sets the int to a random number from 1-30


System.out.println("Do you wish to play single player or against an AI?(Solo? or Against?)");
a = scan.nextLine();//asks if the user wants to play against or solo


System.out.println("Please enter a number 1-30, to play this game(You only get one try)");
int guess = scan.nextInt();//asks the user for a number to be guessed
System.out.println("==ARCADE TOKEN USED==");




while(guess < 1 || guess > 30){
	
System.out.println("Choice not in range, try again.");
break;
}//tells the user if it is in range or not



while(guess!=answer){
	
System.out.println("INCORRECT! The answer was " + answer);
break;
}//tells the user if their guess was incorrect



while(guess == answer){
	
System.out.println("Congratulations! You guessed correctly! You have gained 100 tickets, which are redeemable for a prize at the Ticket Palace ");
break;
}//tells the user if their guess was correct



if(a == "Against"){
	
System.out.println("Computer guessed the number: " + companswer);


			while (companswer == answer){
				System.out.println("The computer was correct");
			}// Broken for now....
			
			} 

		
		
		
	}

}
