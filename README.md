# The-Banking-system-

This is human coded demo banking system and cannot be used as Real Life cash or money related service for Bankings payments.
<br>
THANK YOU
<br>
print( ' BANK of VIT Bhopal University ')
balance = 0
while True :
    print(" \n ----BanKing System Menu----")
    print(' 1>  Deposit')
    print(' 2>  Withdraw')
    print(' 3>  Check Balance')
    print(' 4>  Exit')
    choice= input (" Enter your Choice [1-4] \n ")
    if (choice == '1') :
        try:
            deposit_amount = float(input('Enter amount to Deposit ='))
            if deposit_amount > 0 :
                balance += deposit_amount # balance = balance + deposit_amount 
                print('Deposited Successfully!! ',' New Balance =', balance)
            else:
                print('Invalid Amount ; Money must be Positive ')
        except ValueError :
            print('Invalid input , PLEASE! Enter a number =')
    if choice =='2' :
        try:
            withdraw_amount = float (input('Enter amount to WITHDRAW = '))
            if withdraw_amount > 0:
                if balance>= withdraw_amount :
                    balance -= withdraw_amount # balance = balance - withdraw_amount
                    print('WIthdrew Successfullly!! \n', 'Current Balance= ',balance)
                else:
                    print('Insufficient Balance ')
            else:
                 print('Money cannot be NEGATIVE!!')
        except ValueError:
            print('Invalid input!  Please Enter a valid Input')
    elif choice =='3':
        print("Current Balance =", balance )
    elif choice =='4':
        print('Thank YOU!!')
        break
    else:
        print('Invalid choice')                
                    
