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


# Question 3 of Assignment 3 BUSA 523 SPRING 2022 (Just because I liked that question )

def all_possible_outcomes(n):               # step 1: input size = n    
    answer = []                             # step 2: (1)      
    for i in range(1, 12):                  # step 3: (n )
        for j in range(i, 12):              # step 4: (n )
            if(n < i+j and i+j <= 21):      # step 5: (1)            
                answer.append([i,j])        # step 6: (1)               

    all_possible_outcomes(15)
