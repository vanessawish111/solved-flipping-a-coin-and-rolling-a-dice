Download Link: https://assignmentchef.com/product/solved-flipping-a-coin-and-rolling-a-dice
<br>
<p class="ui header product-top-header" title="Program that simulates flipping a coin and rolling a dice Solution">Write a program that simulates flipping a coin and rolling a dice.A user will input their choice of flipping a coin (C), rolling a dice (D), or exiting (E).If the user chooses a coin toss, the program will ask how many times the coin should be tossed, and then will simulate tossing the coin that many times and print the result to the user.

If the user chooses rolling a die, the program will ask how many sides the die has and how many times it should be rolled.  The program will then simulate rolling a die (with the number of sides specified) that many times.

The program will continue until the user presses E.This should be a lot of fun!

Here are some great things to think about as you begin your program!You will need two functions. A string flipCoin() and a int rollDice(int) function. These functions will generate a random number. For the coin flip, the random number should be in the range of 1 to 2. If the number is 1, the function should return heads. If the random number is 2, the function should return tails. For the roll dice function, the random number should be in the range of 1 to the number of sides. The function should return the result of the die roll.

Important notes: You will want to seed your random number generator. To do this at the beginning of your program #include &lt;ctime.

Use the following commands to seed the random number generator.

//Get the system time to use it to seed the random number generator

unsigned seed = time(0);

//seed the random number generator

srand(seed);

To get a random number between 1 and 2, use the following code: int toss = 1 + rand() % 2;.Sample Output from the ProgramWelcome to the random value generator!

Would you like to flip a coin (C), roll a die (D), or exit (E)? C

How many times do you want to flip the coin? 5

Flip 1 : tails

Flip 2 : heads

Flip 3 : heads

Flip 4 : heads

Flip 5 : tails

Would you like to flip a coin (C), roll a die (D), Exit (E)? D

How many sides does your die have? 6

How many times do you want to roll the die? 5

Roll 1 : 5

Roll 2 : 3

Roll 3 : 2

Roll 4 : 2

Roll 5 : 2

Would you like to flip a coin (C), roll a die (D), or exit (E)? D

How many sides does your die have? 20

How many times do you want to roll the die? 3

Roll 1 : 19

Roll 2 : 16

Roll 3 : 15

Would you like to flip a coin (C), roll a die (D), or exit (E)? E

Thanks for playing!

Press any key to continue

The psedocode:

Using the pseudocode below, write the code that will meet the requirements.

Main FunctionDeclare the number of tosses, number of sides, and user choice.

Seed the random number generator.

while user choice !=EAsk the user if they want to flip a coin, roll a die, or exit.

If the choice is C

Ask the user how many times to flip the coin.

For i=1 to number of flips Step 1

Call flipCoin()

Print result

If the choice is D

Ask the user how many sides the die has.

Ask the user how many times to roll the die.

For i=1 to number of rolls Step 1

Call rollDice()

Print resultElse

Display the closing message.

flipCoin Function

Generate an integer random number between 1 and 2.

If a 1 is generated return heads, else return tails.

rollDice Function

Generate a random number between 1 and the number of sides.

Return the result of the roll.