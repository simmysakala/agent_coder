# Enhanced simple calculator with modulus and basic operation
 
print("Welcome to the Mulungushi University Simple python Calculator!")
print("operaters")
print("You can use +, -, *, /, %, **, //")

try:
    first = float(input("Enter the first number: "))
    op = input("Enter an operator (+, -, *, /, %): ")
    second = float(input("Enter the second number: "))

    if op == "+":
        print("Result =", first + second)
    elif op == "-":
        print("Result =", first - second)
    elif op == "*":
        print("Result =", first * second)
    elif op == "/":
        if second == 0:
            print("Error: Cannot perform modulus with zero (division by zero).")
        else:
            print("Result =", first / second)
    elif op == "**":
        print("result =", first ** second)
    #improve modulus zero check with an explanation.
    elif op == "%"
        if second == 0:
            print("Error: Cannot perform modulus with zero (modulus by zero).")
        else:
            print("Result =", first % second)
    else:
        print("Error: Unknown operator")
#improved error handling message for non_numeri input 
except ValueError:
    print("X Error: Please enter valid numerical values only!")
import math

num = float(input("Enter a number: "))
if num < 0:
    print("Error: Cannot calculate square root of negative number")
else:
    result = math.sqrt(num)
    print("Square root of", num, "is", result)
