# BUSA523.Guy.Anin
Programming
# Creating function that will return sqaure of any input integer
n = int(input())
print(n**2)



# Creating Function for nth Fibonacci number

def Fibonacci(n):
    if n < 0:
        print("Incorrect input")
    elif n == 0:
        return 0
    elif n == 1 or n == 2:
        return 1
    else:
        return Fibonacci(n-1) + Fibonacci(n-2)
 
print(Fibonacci(8))


# Question 2 of Assignment 1 BUSA 523 SPRING 2022

import random

# Arbitrary choosing the  the upper bound of the limit
n = int(input('enter a number between 1 and: '))
number = random.randint(1,n)
guess = int(input('enter a number between 1 and {}: '.format(n)))
print("you will have 5 attempts to guess the number correctly to win")

while guess != number: # When your guess is different from the winning number, two cases occured
    if guess < number: # Guess is lower than winning number 
        print('Your guess is low. Please try again')
        guess = int(input('enter a number between 1 and {}: '.format(n)))



    if guess > number: # Guess is higher than winning number
        print('Your guess is high. Please try again')
        guess = int(input('enter a number between 1 and {}: '.format(n)))


while guess == number: # Correctly guessed the winning number 
    print('Bingo! You guessed it correctly')
    
