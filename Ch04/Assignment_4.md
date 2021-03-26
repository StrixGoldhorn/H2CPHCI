## 1
````Python
def multiply(x,y):
    s = 0
    for i in range(y):
        s += x
    return s
        
def main():
    x = int(input("x: "))
    y = int(input("y: "))
    if(x>y):
        x,y = y,x
    if(x<0 and y<0):
        x=abs(x)
        y=abs(y)
    print(f'\nAnswer: {multiply(x,y)}')
    
main()
````

<br/><br/><br/>

## 2
````Python
def recur(n):
    global cnt
    if cnt!=(n+1):
        print("*"*cnt)
        cnt+=1
        recur(n)
    else:
        return
        
def main():
    n = int(input("n: "))
    recur(n)

main()
````

<br/><br/><br/>

## 3
````Python
s = 0
cnt = 1
def recur(n):
    global s, cnt
    if cnt!=(n+1):
        s+=cnt
        cnt+=1
        recur(n)
    else:
        return
        
def main():
    global s
    n = int(input("n: "))
    recur(n)
    print(s)

main()
````

<br/><br/><br/>

## 4
````Python
balance = 1000

def deposit():
    global balance
    dep = int(input("\nHow much to deposit? $"))
    balance += dep
    print(f'Current balance: {balance}\n\n')
    return

def withdraw():
    global balance
    wdrw = -1
    while wdrw<0 or wdrw>balance:
        wdrw = int(input("\nHow much to withdraw? $"))
    balance -= wdrw
    print(f'Current balance: {balance}\n\n')
    return

def seebal():
    global balance
    print(f'\nCurrent balance: {balance}\n\n')
    return

def main():
    global balance
    menu = "1. Deposit\n2. Withdrawal\n3. See Balance\n4. Quit"
    print(menu)
    usr1 = int(input("Option: "))
    exitcondition = 4

    while usr1 != exitcondition:
        #psuedo-switchcase
        if usr1 == 1:
            deposit()

        elif usr1 == 2:
            withdraw()

        elif usr1 == 3:
            seebal()
            
        else:
            print("Not an option.\n\n\n")
        
        print(menu)
        usr1 = int(input("Option: "))
    print(f"Current balance is ${balance}. Have a nice day.")
    return

main()
````
