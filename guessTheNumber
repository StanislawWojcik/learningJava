import java.util.Scanner;

public class NumberGame {

	private static int lowerRange = 0;
	private static int upperRange = 100;
	private static int counter = 1;
	private static int userChoice;
	
	// gets number from user
	public static int getNumber() {
		Scanner userNumber = new Scanner(System.in);
		System.out.println("Enter your number: ");
		int userChoice = userNumber.nextInt();
		return userChoice;
	}
	
	// gets random number from range 1-100
	public static int getRandomNumber() {
		int number = 1 + (int)(100 * Math.random());
	    return number;
	}
	
	// game loop
	public static void gameLoop() {
		int randomNumber = getRandomNumber();

		while (randomNumber!=userChoice) {
			userChoice=getNumber();
			if (userChoice > randomNumber) {
				upperRange = userChoice -1;
				System.out.println("Too high!");
				System.out.println("Guess the number in range from "+lowerRange+" to "+upperRange);
				counter++;
			} else if (userChoice < randomNumber) {
				lowerRange = userChoice +1;
				System.out.println("Too low!");
				System.out.println("Guess the number in range from "+lowerRange+" to "+upperRange);
				counter++;
			} else if (userChoice == randomNumber) {
				System.out.println("Congratulations! You win!");
				System.out.println("You needed " + counter + " rounds");

			}
		}
	}
	
	public static void main(String[] args) {
		gameLoop();

	}

}
