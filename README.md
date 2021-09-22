# Calculator-Making
## Using the if and elif  functions



### Intialy taking a variable (result) is equall to 0:
result = 0
###  x and y values  from the user:
x = input("enter a number")
y = input("enter another number")
### Using the if condition finding the x is integer or float:
### if x having . then it's float, printed x is float and otherwise it will go to the next line:
if '.' in x:
    x = float(x)
    print("x is float")
### if y having . then it's float,printed y is float and otherwise it will go to the next line:
if '.' in y:
    y = float(y)
    print("y is float")
### if x not  having . then it's integer,printed x is integer and otherwise it will go to the next line:
if '.' not in x:
    x = int(x)
    print("x is integer")
### if y not  having . then it's integer,printed y is integer:
if '.' not in y:
    y = int(y)
    print("y is integer")
### selecting the operator and which is store in the choice variable:
choice = input('''select operator:
               '+' for addition
               '-' for subtraction
               '*' for multiplication
               '/' for division
               '^' for square
               '%' for module ''')
## Using the if and elif  function
### if the choice is + it will perform addition between in x and y and printed x+y, otherwise move to elif condition:
if choice == '+':
    print("{} + {} = ".format(x,y))
    print(x + y)
### if the choice is - it will perform subtraction between in x and y and printed x-y, otherwise move to elif condition:
elif choice == '-':
    print("{} - {} = ".format(x,y))
    print(x-y)
### if the choice is * it will perform multiplication between in x and y and printed x*y, otherwise move to elif condition:
elif choice == '*':
    print("{} * {} = ".format(x,y))
    print(x*y)
### if the choice is / it will perform division between in x and y and printed x/y, otherwise move to elif condition:
elif choice == '/':
    print("{} / {} = ".format(x,y))
    print(x/y)
### if the choice is ^ it will perform power between in x and y and printed x^y, otherwise move to elif condition:
elif choice == '^':
        result = x**y
        print(result)
### if the choice is % it will perform modulus between in x and y and printed x%y, otherwise move to else condition:
elif choice == '%':
    print("{} % {} = ".format(x,y))
    print(x%y)
### if the user choosen different operator it will run again:
else:
    print("enter a valid operator , run the program again")
