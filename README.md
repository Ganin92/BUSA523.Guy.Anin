# BUSA523.Guy.Anin
Programming


# Creating function that will return square of any input integer
n = int(input())
print(n**2)



# Creating Function for nth Fibonacci number (a series of numbers in which each number is the sum of the two preceding numbers... exple The Rule is xn = xn−1 + xn−2)
# the 8th term is the 7th term + the 6th term (fbn(18) is 2584, check the website and learn something new today ) Understand this then may be "Bitcoin will hit $100k" lol
# math is fun so here is  the link where  I am learning about the fibonacci sequence... check it out and have fun https://www.mathsisfun.com/numbers/fibonacci-sequence.html 

def Fibonacci(n):
    if n < 0:
        print("Incorrect input")
    elif n == 0:
        return 0
    elif n == 1 or n == 2:
        return 1
    else:
        return Fibonacci(n-1) + Fibonacci(n-2)
 
print(Fibonacci(17))


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
    
