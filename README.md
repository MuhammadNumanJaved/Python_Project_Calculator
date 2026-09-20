# Python_Project_Calculator
Calcultor make easy
# Hello my name is Muhammad Numan Javed.
# Umt student python learner
# To make calculator by using functions
# we use math library for math

import math
def add(num1, num2):
    return num1 + num2

def subtract(num1, num2):
    return num1 - num2

def multiply(num1, num2):
    return num1 * num2

def divide(num1, num2):
    if num2 == 0:
        return "Error! number cannot be divided by zero!"
    else:
        return num1 / num2

def square_root(number):
    if number < 0:
        return "Error! you entered negative number!"
    else:
        return math.sqrt(number)

def power(base, exponent):
    return base ** exponent

# we will make choice options to make selection

print("*" * 40)
print("Welcome to the Calculator!")
print("1. Addition")
print("2. Subtraction")
print("3. Multiplication")
print("4. Division")
print("5. Square_Root")
print("6. Power")
print("*" * 40)

# we make choice for select upper choices

choice = input("Enter your choice: ")
if choice in ('1', '2', '3', '4'):
    num1 = float(input("Enter a first number: "))
    num2 = float(input("Enter a second number: "))
    if choice == '1':
        print(add(num1, num2))

    elif choice == '2':
        print(subtract(num1, num2))

    elif choice == '3':
        print(multiply(num1, num2))

    elif choice == '4':
        print(round(divide(num1, num2), 2))

elif choice == '5':
    number = float(input("Enter a number for square_root: "))
    print(round(square_root(number), 2))

elif choice == '6':
    base = int(input("Enter a base: "))
    exponent = int(input("Enter a exponent: "))
    print(power(base, exponent))

# if user will not select choices in given description then this statement will executed.

else:
    print("Invalid choice! Try again!")

# Thanks for visitng on our calculator program
