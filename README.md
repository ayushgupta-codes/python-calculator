# python-calculator
beginner-friendly calculator built using Python


# Python Calculator
# Created by Ayush Gupta

print("================================")
print("      AYUSH'S CALCULATOR )
print("================================")

print("1. Addition (+)")
print("2. Subtraction (-)")
print("3. Multiplication (*)")
print("4. Division (/)")

choice = input("Choose an operation (1-4): ")

try:
    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))

    if choice == "1":
        result = num1 + num2
        print("Result:", result)

    elif choice == "2":
        result = num1 - num2
        print("Result:", result)

    elif choice == "3":
        result = num1 * num2
        print("Result:", result)

    elif choice == "4":
        if num2 == 0:
            print("Error: Cannot divide by zero!")
        else:
            result = num1 / num2
            print("Result:", result)

    else:
        print("Invalid choice! Please choose 1-4.")

except ValueError:
    print("Error: Please enter valid numbers.")

print("Thank you for using the calculator!")
