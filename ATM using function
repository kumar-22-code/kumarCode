def readPin():
    file = open("pin.txt",'r')
    a = int(file.read())
    file.close()
    return a

def readBal():
    file = open("balance.txt",'r')
    a = int(file.read())
    file.close()
    return a

def writePin(a):
    file = open("pin.txt",'w')
    file.write(str(a))
    file.close()

def writeBal(a):
    file = open("balance.txt",'w')
    file.write(str(a))
    file.close()

print("Press 1 : withdraw")
print("Press 2 : Check balance")
print("Press 3 : change pin")
print("Press 4 : Deposite")
choice = int(input("enter your choice = "))

if(choice==1):
    upin = int(input("enter a pin = "))
    pin = readPin()
    if(upin==pin):
        amount = int(input("enter a amount = "))
        bal = readBal()
        if(bal>=amount):
            bal = bal - amount
            print("Transaction successful")
            print(f"Current balance = {bal}")
            writeBal(bal)
        else:
            print("low balance")
    else:
        print("wrong pin")

if(choice==2):
    upin = int(input("enter a pin = "))
    pin = readPin()
    if(upin==pin):
        bal = readBal()
        print(bal)
    else:
        print("Wrong pin")
if(choice==3):
    upin = int(input("enter a pin = "))
    pin = readPin()
    if(upin==pin):
        npin=input("Enter a new pin : ")
        writePin(npin)
        print(f"Now your new pin is : {npin}")
    else:
        print("Wrong pin")
if(choice==4):
    upin = int(input("enter a pin = "))
    pin = readPin()
    if(upin==pin):
        amt = int(input("Enter an amount to deposit"))
        bal = readBal()
        bal += amt
        print(f"Deposited successfully! Current Balance = {bal}")
        writeBal(bal)
