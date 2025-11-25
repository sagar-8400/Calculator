# Simple Calculator Program (Student Level)

print("--- SIMPLE CALCULATOR ---")

# Taking input
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

print("\nChoose Operation:")
print("1. Addition (+)")
print("2. Subtraction (-)")
print("3. Multiplication (*)")
print("4. Division (/)")

choice = input("Enter your choice (1/2/3/4): ")

# Performing calculation
if choice == "1":
    result = num1 + num2
    print(f'Result: {num1} + {num2} = {result}')

elif choice == "2":
    result = num1 - num2
    print(f'Result: {num1} - {num2} = {result}')

elif choice == "3":
    result = num1 * num2
    print(f'Result: {num1} * {num2} = {result}')

elif choice == "4":
    if num2 != 0:
        result = num1 / num2
        print(f'Result: {num1} / {num2} = {result}')
    else:
        print("Error! Division by zero not allowed.")

else:
    print("Invalid choice! Please select 1, 2, 3, or 4.")
