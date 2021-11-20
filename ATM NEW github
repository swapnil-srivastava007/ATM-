balance=10000
pin=0000

def balance_check():
  global balance
  print("Your A/C balance is ",balance)
def cash_withdraw(withdraw_amount):
  global balance
  print(withdraw_amount," Withdraw succesfully!")
  balance=balance-withdraw_amount
  print("Your updated balance is ",balance)
def cash_deposit(deposit_amount):
  global balance
  print("Deposited succesfully!")
  balance=balance+deposit_amount
  print("Your updated balance is ",balance)
def change_pin(old, new):
  global pin
  if not pin==old:
    print("Invalid old PIN, Please try again or visit the nearest branch")
  else:
    pin=new
    print("ATM Card PIN ending with xx23 is updated Successfully!")

print("""WELCOME TO XYZ BANK!
      Enter your card..""")
pws=int(input("Enter your pin: "))
if pin==pws:
  while True:
    print("""
-----------------------------------
   WELCOME TO XYZ BANK!
    1.Check Balance
    2.Cash Withdraw
    3.Cash Deposit
    4.Change PIN
    5.Exit""")
    choice=int(input("Enter your choice: "))
    if choice==1:
      balance_check()
    elif choice==2:
            amount=int(input("Enter your withdraw amount:"))
            cash_withdraw(amount)
    elif choice==3:
           amount=int(input("Enter your deposit amount:"))
           cash_deposit(amount)
    elif choice==4:
          old_pin=int(input("Enter your old pin:"))
          new_pin=int(input("Enter your new pin:"))
          change_pin(old_pin, new_pin)
    elif choice==5:
        print("Exit successfully")
        break
    else:
        print("INVALID CHOICE")
else:
  print("INVALID PIN")
