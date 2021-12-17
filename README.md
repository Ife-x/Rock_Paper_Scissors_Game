# Rock_Paper_Scissors_Game

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


options = [rock, paper, scissors]
user_choice = int(input("what do you choose? Type 0 for rock, 1 for paper and 2 for scissors\n"))
if user_choice > 2:
  print("Your choice is out of range, you lose")
else:
  print(options[user_choice])
  computer_choice = random.randint(0,2)
  print("computer chose:")
  print(options[computer_choice])



  if user_choice == computer_choice:
    print("It's a tie.")
  elif user_choice > computer_choice:
    print("You win")
  elif user_choice < computer_choice:
    print("You lose")
  elif user_choice == 0 and computer_choice ==2:
    print("You win")
  elif user_choice == 2 and computer_choice == 0:
    print("You lose")
