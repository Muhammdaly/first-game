print("Welcome to the Rock, Paper, Scissors game:")
rules = input("Press Enter to continue or type (Help) for the rules: ").lower()
if rules == "help":
  print("\n********** RULES **********\n")
  print("1) You choose and the computer chooses")
  print("2) Rock smashes Scissors -> Rock wins")
  print("3) Scissors cut paper -> Scissors wins")
  print("Paper covers Rock -> paper wins\n")
else:
 print("")
choice = input("Enter your choice (Rock, Paper, Scissors): ")
computer_list=["Rock","Paper","Scissors"]
import random
computer_choice = random.choice(computer_list)
rock =("""
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
""")
paper = ("""
     _______
---'    ____)____
           ______)
          _______)
         _______)
---.__________)
""")
scissors = ("""
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
""")
if choice=="rock" and computer_choice =="Paper":
  print("\nYou chose:\n")
  print(rock)
  print("\nComputer chose\n")
  print(paper,"\n")
  print("You lose Paper beats Rock")
elif choice == "rock" and computer_choice =="Scissors": 
  print("\nYou chose:\n")
  print(rock)
  print("\nComputer chose\n")
  print(scissors,"\n")
  print("You win Rock beats Scissors")
elif choice=="rock" and computer_choice == "Rock":
  print("\nYou chose:\n")
  print(rock)
  print("\nComputer chose\n")
  print(rock,"\n")
  print("Draw!")
elif choice=="paper" and computer_choice =="Rock":
  print("\nYou chose:\n")
  print(paper)
  print("\nComputer chose\n")
  print(rock,"\n")
  print("You win Paper beats Rock")
elif choice == "paper" and computer_choice == "Scissors":
  print("\nYou chose:\n")
  print(paper)
  print("\nComputer chose\n")
  print(scissors,"\n")
  print("You lose Scissors beats Paper")
elif choice == "paper" and computer_choice == "Paper":
  print("\nYou chose:\n")
  print(paper)
  print("\nComputer chose\n")
  print(paper,"\n")
  print("Draw!")
elif choice == "scissors" and computer_choice == "Rock":
  print("\nYou chose:\n")
  print(scissors)
  print("\nComputer chose\n")
  print(rock,"\n")
  print("You lose Rock beats Scissors")
elif choice=="scissors" and computer_choice=="Paper":
  print("\nYou chose:\n")
  print(scissors)
  print("\nComputer chose\n")
  print(paper,"\n")
  print("You win Scissors beats Paper ")
elif choice == "scissors" and computer_choice == "Scissors":
 print("\nYou chose:\n")
 print(scissors)
 print("\nComputer chose\n")
 print(scissors,"\n")
 print("Draw!")
else:
  print("invalid choice.")
