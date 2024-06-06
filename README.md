# tsn
while True:
    print('Select an operation to perform: ')
    print('1. ADD')
    print('2. SUBTRACT')
    print('3. MULTIPLY')
    print('4. DIVIDE')
    print('5. EXIT')
    operation = input()
    #to break the loop
    if operation == '5':
        print("Exiting...")
        break
    #Enter 1, 2,  3, 4 to perform each operation as needed
    if operation in ['1', '2', '3', '4']:
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))
    #Addition
        if operation == '1':
            print("The sum is " + str(int(num1) + int(num2)))
    #Subtraction
        elif operation == '2':
            print("The difference is " + str(int(num1) - int(num2)))
    #Multiplication
        elif operation == '3':
            print("The product is " + str(int(num1) * int(num2)))
    # Division
        elif operation == '4':
            #Devide by 0
            if num2 == 0:
                print('Divide by 0 Error')
            else:
                print("The quotient is " + str(int(num1) / int(num2)))
    else:
        print("Invalid Entry ")

