# Python_individual_task1
## Medium level
    print('Hello user! Welcome to your deposit account!')
    balance = 0
    
    while True:
        deposit = input('Please enter the amount of money you want to deposit: ')
        try:
            deposit = int(deposit)
            balance += deposit
            print(f'Balance of your account is {balance}.')
        except ValueError:
            print("Invalid input.")
            continue
    
        exit = input('If you want to exit write STOP, or press Enter ')
        if exit == 'STOP':
            break
    
    print(f'Total balance of your account is {balance}. Have a nice day!')
