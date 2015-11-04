# Introduction
This is an additional game that is based on simple math addition. It consists of four rounds. The user is asked to add two random numbers. Each correct answer is followed by 10 points and incorrect answer is followed by simpler question. At last, the final score is printed on the console screen.
## Code
```java
/**
 * 
 */

/**
 * @author Prasun Thapa
 *
 */import java.util.Scanner;
public class Addition_Game_HW6 {

	/**
	 * @param args
	 */
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		System.out.println("Hello Class");
		
		int score = 0;
		int hardnessOfQuestion = 10;
		
		// Round 1
		//	Generate 2 random numbers
		int number1 = (int)(Math.random() * hardnessOfQuestion);
		/* No longer needed debug statement
		 * System.out.println("Number1 is :" + number1 );
		 */
		
		int number2 = (int)(Math.random() * hardnessOfQuestion);
		/* No longer needed debug statement
		 * System.out.println("Number2 is :" + number2 );
		 */
		
		// to keep track of the correct answer.
		int correctAnswer = number1 + number2;
		
		//  Ask the user to add these two numbers together
		System.out.println
		("What integer is " + number1 + " + " + number2 + "?");
		System.out.println("Please answer in integers only.");
		
		//  Read in their response
		Scanner input = new Scanner(System.in);
		int studentAnswer = input.nextInt();
		//  Check if the answer was correct
		//		IF correct
		if (studentAnswer == correctAnswer){
			//			Tell them it was correct
			System.out.println("Answer was correct");
			//			Give them points
			score += hardnessOfQuestion;
			System.out.println("Score is: " + score);
			//			Make the next question harder
			hardnessOfQuestion *= 10;	
			System.out.println("hardness is: " + hardnessOfQuestion);
		}
		//		IF not correct
		else{
			//			Tell them it was wrong
			System.out.println("Answer was not correct");
			// 			Tell them the correct answer
			System.out.println("The correct answer was: " + correctAnswer);
			//			Do not give them points
			score += 0;
			//			Make the next question easier
			if(hardnessOfQuestion>10){
				hardnessOfQuestion /= 10;	
				/* This line of code would do the same thing
				 * as hardnessOfQuestion /= 10;.
				 * hardnessOfQuestion = hardnessOfQuestion / 10;
				 */
			}
		}
		System.out.println("End of round 1");
		// end of round 1
		
		// Round 2 (note: additional comments in round 1)
		//	Generate 2 random numbers
		number1 = (int)(Math.random() * hardnessOfQuestion);
		number2 = (int)(Math.random() * hardnessOfQuestion);

		
		// to keep track of the correct answer.
		correctAnswer = number1 + number2;
		
		//  Ask the user to add these two numbers together
		System.out.println
		("What integer is " + number1 + " + " + number2 + "?");
		System.out.println("Please answer in integers only.");
		
		//  Read in their response
		//Scanner input = new Scanner(System.in);
		studentAnswer = input.nextInt();
		//  Check if the answer was correct
		//		IF correct
		if (studentAnswer == correctAnswer){
			//			Tell them it was correct
			System.out.println("Answer was correct");
			//			Give them points
			score += hardnessOfQuestion;
			System.out.println("Score is: " + score);
			//			Make the next question harder
			hardnessOfQuestion *= 10;	
			System.out.println("hardness is: " + hardnessOfQuestion);
		}
		//		IF not correct
		else{
			//			Tell them it was wrong
			System.out.println("Answer was not correct");
			// 			Tell them the correct answer
			System.out.println("The correct answer was: " + correctAnswer);
			//			Do not give them points
			score += 0;
			//			Make the next question easier
			if(hardnessOfQuestion>10){
				hardnessOfQuestion /= 10;	
			}
		}
		// end of round 2
		System.out.println("End of round 2");
		// Round 3 (note: additional comments in round 1)
		//	Generate 2 random numbers
		number1 = (int)(Math.random() * hardnessOfQuestion);
		number2 = (int)(Math.random() * hardnessOfQuestion);

		
		// to keep track of the correct answer.
		correctAnswer = number1 + number2;
		
		//  Ask the user to add these two numbers together
		System.out.println
		("What integer is " + number1 + " + " + number2 + "?");
		System.out.println("Please answer in integers only.");
		
		//  Read in their response
		//Scanner input = new Scanner(System.in);
		studentAnswer = input.nextInt();
		//  Check if the answer was correct
		//		IF correct
		if (studentAnswer == correctAnswer){
			//			Tell them it was correct
			System.out.println("Answer was correct");
			//			Give them points
			score += hardnessOfQuestion;
			System.out.println("Score is: " + score);
			//			Make the next question harder
			hardnessOfQuestion *= 10;	
			System.out.println("hardness is: " + hardnessOfQuestion);
		}
		//		IF not correct
		else{
			//			Tell them it was wrong
			System.out.println("Answer was not correct");
			// 			Tell them the correct answer
			System.out.println("The correct answer was: " + correctAnswer);
			//			Do not give them points
			score += 0;
			//			Make the next question easier
			if(hardnessOfQuestion>10){
				hardnessOfQuestion /= 10;	
			}
		}
		// end of round 3
		System.out.println("End of round 3");
		// Round 4 (note: additional comments in round 1)
		//	Generate 2 random numbers
		number1 = (int)(Math.random() * hardnessOfQuestion);
		number2 = (int)(Math.random() * hardnessOfQuestion);

		
		// to keep track of the correct answer.
		correctAnswer = number1 + number2;
		
		//  Ask the user to add these two numbers together
		System.out.println
		("What integer is " + number1 + " + " + number2 + "?");
		System.out.println("Please answer in integers only.");
		
		//  Read in their response
		//Scanner input = new Scanner(System.in);
		studentAnswer = input.nextInt();
		//  Check if the answer was correct
		//		IF correct
		if (studentAnswer == correctAnswer){
			//			Tell them it was correct
			System.out.println("Answer was correct");
			//			Give them points
			score += hardnessOfQuestion;
			System.out.println("Score is: " + score);
			//			Make the next question harder
			hardnessOfQuestion *= 10;	
			System.out.println("hardness is: " + hardnessOfQuestion);
		}
		//		IF not correct
		else{
			//			Tell them it was wrong
			System.out.println("Answer was not correct");
			// 			Tell them the correct answer
			System.out.println("The correct answer was: " + correctAnswer);
			//			Do not give them points
			score += 0;
			//			Make the next question easier
			if(hardnessOfQuestion>10){
				hardnessOfQuestion /= 10;	
			}
		}
		// end of round 4
		System.out.println("End of round 4 and the end of the game");
		System.out.println("Final Score = " + score);
	}


	}
	```



## Console

Hello Class
What integer is 1 + 1?
Please answer in integers only.
2
Answer was correct
Score is: 10
hardness is: 100
End of round 1
What integer is 80 + 91?
Please answer in integers only.
7
Answer was not correct
The correct answer was: 171
End of round 2
What integer is 7 + 5?
Please answer in integers only.
12
Answer was correct
Score is: 20
hardness is: 100
End of round 3
What integer is 18 + 68?
Please answer in integers only.
86
Answer was correct
Score is: 120
hardness is: 1000
End of round 4 and the end of the game
Final Score = 120

## Summary

This program is a math addition project that asks the user to add two different numbers and displays the final score. The program looks complicated as it is too long. But, it is simple and easily assessable to user. I have used IF statement to verify the answer assigned by the user. IF statement is a conditional statement that runs on the basis of assigned limitations. The most unique thing that I have used in the program is the Math random syntax. By using this syntax, we can generate the random numbers in the console. The number varies if we run the program again and again, that makes the program unique every time. Beside these, I have used Scanner class for console input. I have used a lot of variables to store the values for calculations. IF statements and System.out statements are used time and again to check the answers prompt by the user and to print the statements according the matched conditions.

## Utilization of Git to Develop this Code

 I have effectively used the github and git commands to complete this program. Firstly, I made a repository in the github account. Then, I pushed my eclipse files to the repository created in the github. I was simultaneously working in the eclipse, command prompt and github account. The code written in the eclipse was pushed to github repository from time to time using the command prompt. I made the four branches, one branch for each round. I was pushing my files after finishing the code of each round. For this process, I used git add . to make some changes in the file. Subsequently, using the git commit, I assured the changes made in the file. And I used git push to send my file in the online repository. 
We use different branch to make a certain change in the file. It is because, if we make some error while making the change in a branch, we can easily extract the same data from the master branch and debug the error. Finally, we can use git merge to merge the contents of different branches. I did the same while coding this project.

## Executive Summary
In this homework set we learned the simultaneous use of eclipse and command prompt and github account. The online repository in the github account can also be consider as one of the secure way of storing data. We can figure out different other programs that are based on logical operations using the same concept. 
Git is really an interesting and useful topic. Thank you Dr. Evert for your entire effort.    

