# python-calculator
Open Source python calculator

FULL CODE: 

print("""
  ____    _    _      ____  _   _ _        _  _____ ___  ____  
 / ___|  / \  | |    / ___|| | | | |      / \|_   _/ _ \|  _ \ 
| |     / _ \ | |   | |    | | | | |     / _ \ | || | | | |_) |
| |___ / ___ \| |___| |___ | |_| | |___ / ___ \| || |_| |  _ < 
 \____/_/   \_\_____|\____| \___/|_____/_/   \_\_| \___/|_| \_\
""")

print("\n Welcome to the calculator.\n Designed and made by froger.\n GitHub Repository: https://github.com")

while True:
    print("\n Enter your function.")
    print(" 1. Addition")
    print(" 2. Subtraction")
    print(" 3. Multiplication")
    print(" 4. Division")
    print(" 5. Exit")
    function = input(" Enter Option: ").strip().lower()

    if function == "5" or function == "exit":
        print("Goodbye!")
        break

    if function == "1" or function == "addition":
        num1 = int(input("Enter the FIRST number you'd like to add: "))
        num2 = int(input("Enter the SECOND number you'd like to add: "))
        print("Result:", num1 + num2)

    elif function == "2" or function == "subtraction":
        num1 = int(input("Enter the FIRST number you'd like to subtract: "))
        num2 = int(input("Enter the SECOND number you'd like to subtract: "))
        print("Result:", num1 - num2)

    elif function == "3" or function == "multiplication":
        num1 = int(input("Enter the FIRST number you'd like to multiply: "))
        num2 = int(input("Enter the SECOND number you'd like to multiply: "))
        print("Result:", num1 * num2)

    elif function == "4" or function == "division":
        num1 = int(input("Enter the FIRST number you'd like to divide: "))
        num2 = int(input("Enter the SECOND number you'd like to divide: "))
        if num2 == 0:
            print("Error: Cannot divide by zero!")
        else:
            print("Result:", num1 / num2)
            
    else:
        print("Invalid option, try again.")

