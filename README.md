# Rock-Paper-and-Scissors
A basic game with symbolic representation of Rock, Paper and Scissor Hand

# *******************MINE*******************
rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''

paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''

scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''
import random
print("Welcome you're about to play the world famous\nGame.!")
print("\nRock Paper and Scissors")
player_input = input("\nrock paper scissors? \n")
player = player_input.lower()
if player == "rock" :
   print(rock)
elif player == "paper":
   print(paper)
elif player == "scissors":
   print(scissors)

comp = random.randint(0,2)
options = [rock, paper, scissors]
ai = options[comp]
print('\n', ai)

if player == "rock":
  if ai == rock:
    print("it is a draw")
  elif ai == paper:
    print("You lose")
  elif ai == scissors:
    print("You win")
elif player == "paper":
  if ai == rock:
    print("You win")
  elif ai == paper:
    print("it is a draw")
  elif ai == scissors:
    print("You lose")
elif player == "scissors":
  if ai == rock:
    print("You lose")
  elif ai == paper:
    print("You win")
  elif ai == scissors:
    print("is is a draw")

# *******************INSTRUCTOR***********************

import random

rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''

paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''

scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''
game_images = [rock, paper, scissors]

user_choice = int(input("What do you choose? Type 0 for Rock, 1 for Paper or 2 for Scissors.\n"))
print(game_images[user_choice])

computer_choice = random.randint(0, 2)
print("Computer chose:")
print(game_images[computer_choice])

if user_choice >= 3 or user_choice < 0:
  print("You typed an invalid number, you lose!")
elif user_choice == 0 and computer_choice == 2:
  print("You win!")
elif computer_choice == 0 and user_choice == 2:
  print("You lose")
elif computer_choice > user_choice:
  print("You lose")
elif user_choice > computer_choice:
  print("You win!")
elif computer_choice == user_choice:
  print("It's a draw")
