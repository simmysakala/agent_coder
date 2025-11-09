
git# Simple Calculator with Modulus made by a python

print("Welcome to the Calculator!")
print("You can use +, -, *, /, %")

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
            print("Error: Cannot divide by zero")
        else:
            print("Result =", first / second)
    elif op == "%":
        if second == 0:
            print("Error: Cannot divide by zero (modulus)")
        else:
            print("Result =", first % second)
    else:
        print("Error: Unknown operator")

except ValueError:
    print("Error: Please enter valid numbers")