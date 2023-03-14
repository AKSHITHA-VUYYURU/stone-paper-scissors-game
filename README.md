# stone-paper-scissors-game
#building a game using python 
import random
user_input = input("Enter a choice (rock, paper, scissors): ")
possible_input = ["rock","paper","scissors"]
computer_input = random.choice(possible_input)
print(f"\nYou chose {user_input}, computer chose {computer_input}.\n")
if user_input == computer_input:
    print(f"Both players selected {user_input}. It's a tie!")
elif user_input == "rock":
    if computer_input == "scissors":
        print("Rock smashes scissors! You win!")
    else:
        print("Paper covers rock! You lose.")
elif user_input == "paper":
    if computer_input == "rock":
        print("Paper covers rock! You win!")
    else:
        print("Scissors cuts paper! You lose.")
elif user_input == "scissors":
    if computer_input == "paper":
        print("Scissors cuts paper! You win!")
    else:
        print("Rock smashes scissors! You lose.")
        
  output:1
 Enter a choice (rock, paper, scissors): rock

You chose rock, computer chose paper.

Paper covers rock! You lose.
output:2
Enter a choice (rock, paper, scissors): paper

You chose paper, computer chose paper.

Both players selected paper. It's a tie!
