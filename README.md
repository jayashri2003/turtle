![image](https://github.com/jayashri2003/turtle/assets/152845576/3b6df750-f497-41eb-9eaf-368e3da14edf)# turtle
#The Python Turtle Race project

#Setting Up the Game Environment
>>> import turtle
>>> import random

#Setting Up the Turtles and Homes

>>> player_one = turtle.Turtle()
>>> player_one.color("green")
>>> player_one.shape("turtle")
>>> player_one.penup()
>>> player_one.goto(-200,100)
>>> player_two = player_one.clone()
>>> player_two.color("blue")
>>> player_two.penup()
>>> player_two.goto(-200,-100)

>>> player_one.goto(300,60)
>>> player_one.pendown()
>>> player_one.circle(40)
>>> player_one.penup()
>>> player_one.goto(-200,100)
>>> player_two.goto(300,-140)
>>> player_two.pendown()
>>> player_two.circle(40)
>>> player_two.penup()
>>> player_two.goto(-200,-100)

#Creating the Die
>>> die = [1,2,3,4,5,6]
>>> for i in range(20):
...     if player_one.pos() >= (300,100):
...             print("Player One Wins!")
...             break
...     elif player_two.pos() >= (300,-100):
...             print("Player Two Wins!")
...             break
...     else:
...             player_one_turn = input("Press 'Enter' to roll the die ")
...             die_outcome = random.choice(die)
...             print("The result of the die roll is: ")
...             print(die_outcome)
...             print("The number of steps will be: ")
...             print(20*die_outcome)
...             player_one.fd(20*die_outcome)
...             player_two_turn = input("Press 'Enter' to roll the die ")
...             die_outcome = random.choice(die)
...             print("The result of the die roll is: ")
...             print(die_outcome)
...             print("The number of steps will be: ")
...             print(20*die_outcome)
...             player_two.fd(20*die_outcome)
 

![image](https://github.com/jayashri2003/turtle/assets/152845576/82b9ca7e-a8ce-4d86-907f-8d9cd4966fc7)
![image](https://github.com/jayashri2003/turtle/assets/152845576/f4aa8e2a-1e2f-4d6b-8658-27fce830b911)




