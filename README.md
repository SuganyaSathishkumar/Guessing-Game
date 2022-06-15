# Guessing-Game

## About the Game

         **Firstly,When we run the game ,the computer generates a random number.
         **So when the user plays the game,he has to guess the random number.
         ** So how could the user guess the random number and play the game.
         ** Let us assume that the computer generated random number is 25.
         ** If the user type a number 99,a message ""Too High!Try Again"" will be displayed.
         ** Else If the user type a number 14,a message "Too Low!Try Again"" will be displayed.
         ** It means that the number lies either between 14 and 99.
         **Then like this we come together anc finally guess the random number and a message "Congratulations!You got it right" will br displayed.
         
## Steps involved in creating the game

         (i) Generating Random Number
         (ii) Access the User entered value
         (iii)Compare with Random number and display the result.
         (iv) Handle Invalid User Input.
         
     
### Generating Random Number:

 ##JS Code to create a Random Number:
 ##### let randomNumber = Math.ceil(Math.random()*100);
  
   *** In order to generate a Random Number in Javascript , I use Math.random() Function.
   #### Math.random():
         
         It returns a random number (float value) in range 0 to less than 1.
         
  For example: 
     
  JS Code:   Console.log(Math.random());
  Output :   0.5708919280652551
  
  *** In order to generate a Random number from 1 to 100,I use Math.random()*100.
  
  For example:
  
  JS Code: Console.log(Math.random()*100);
  Output:  95.906698007537561
  
  *** Since I get the random number in flot value and I need an integer value as an input, I use Math.ceil() Function.
  #### Math.ceil():
  
        This function always rounds a number up to the next largest integer.
        
 For example:
 
 JS Code: Console.log(Math.ceil(95.906698007537561));
 Output :  96
 
 ### Accessing the User Entered value:
 
 #### JS Code to access the User entered value:
 let gameResult = document.getElementById("gameResult");
 let userInput = document.getElementbyId("UserInput");
 let randomNumber = Math.ceil(Math.random()*100);
 function CheckGuess(){
  let guessedNumber = parseInt(userInput.value);
 }
 ** The value that the user has given should be an integer, so we have converted the user Input value to ParseInt and stored it in guessedNumber variable.
 ** Here to get user Input we use HTML Input Element.
 ##### HTML Input Element: 
      Creates interactive controls in order to accept the data from the user.
##### Value Property:
       Use value property to get the value of the HTML Input Element.
   JS Code: document.getElementById("inputElement").value;
   
### Compare with Random Number and display the result:
##### If User Guess > Random Number:
*** If the Guessed Number is greater than the random number a message "Too High! Try Again" is displayed as  follows:
![image](https://user-images.githubusercontent.com/100849428/173826375-0d2c277f-2cf8-4e21-9d50-a5524b93f1ca.png)
#### If User Guess < Random Number:
*** If the Guessed Number is less than the random number a message "Too Low! Try Again" is displayed as  follows:
![image](https://user-images.githubusercontent.com/100849428/173826602-be8fae8a-5257-45b7-ba52-2e75c8c14e4c.png)
#### If User Guess === Random Number:
*** If the Guessed Number is equal to the random number a message "Congratulations!You got it right" is displayed as  follows:
![image](https://user-images.githubusercontent.com/100849428/173826967-2b2695b5-ccc5-42f1-83bb-f34aac857cfa.png)

## Handle Invalid User Input:

*** If there is any invalid input, a message "Provide a valid user input" will be displayed as follows:
![image](https://user-images.githubusercontent.com/100849428/173827745-98b18e3a-5079-41c5-95b6-3146b996f31a.png)


 
     
