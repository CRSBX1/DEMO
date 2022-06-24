import math
cont = "yes"


while cont.lower() == "yes":
    print("-------calculator--------")
    print('''Please type in the math operation you would like to complete: + for addition, - for subtraction, * for multiplication, / for division, \/ for square root, ** for power''')

    operation = input("enter math operation: ")

    number_1 = float(input('Please enter the first number: '))
    number_2 = float(input('Please enter the second number: '))

    if operation == '+':
     print('{} + {} = '.format(number_1, number_2))
     print(number_1 + number_2)

    elif operation == '-':
     print('{} - {} = '.format(number_1, number_2))
     print(number_1 - number_2)
 
    elif operation == '*':
     print('{} * {} = '.format(number_1, number_2))
     print(number_1 * number_2)

    elif operation == '/':
     print('{} / {} = '.format(number_1, number_2))
     print(number_1 / number_2)

    elif operation == '\/':
     print('\/{} \/ {} = '.format(number_1, number_2))
     print( (math.sqrt(number_1)) , (math.sqrt(number_2)) )

    elif operation == '**':
        print('{}^{} = '.format(number_1, number_2))
        print(number_1**number_2 )

    else:
     print('You have not typed a valid operator, please run the program again.')
    cont = input('Continue? yes/no: ')
    if cont == "no":
     print("Thank you for using calculator =)")
     break

#Made by Antoni Lawrence
