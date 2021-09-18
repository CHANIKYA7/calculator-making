# calculator-making
mini project using the if and elif  functions
result = 0
x = input("enter a number")
y = input("enter another number")
if '.' in x:
    x = float(x)
    print("x is float")
if '.' in y:
    y = float(y)
    print("y is float")
if '.' not in x:
    x = int(x)
    print("x is integer")
if '.' not in y:
    y = int(y)
    print("y is integer")

choice = input('''select operator:
               '+' for addition
               '-' for subtraction
               '*' for multiplication
               '/' for division
               '^' for square
               '%' for module ''')
if choice == '+':
    print("{} + {} = ".format(x,y))
    print(x + y)
elif choice == '-':
    print("{} - {} = ".format(x,y))
    print(x-y)
elif choice == '*':
    print("{} * {} = ".format(x,y))
    print(x*y)
elif choice == '/':
    print("{} / {} = ".format(x,y))
    print(x/y)
elif choice == '^':
        result = x**y
        print(result)
elif choice == '%':
    print("{} % {} = ".format(x,y))
    print(x%y)
else:
    print("enter a valid operator , run the program again")
