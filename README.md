# Rock-Paper-and-Scissors
A basic game with symbolic representation of Rock, Paper and Scissor Hand

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
