## 1
````Python
item = input("Enter item name or xyz to stop: ")
price = "a"
qty = "a"
total = 0.0

while item != "xyz":
    while not price.replace('.','',1).isdigit():
        price = input("  Enter price per item: ")
    while not qty.isdigit():
        qty = input("  Enter quantity: ")
    cost = float(price)*int(qty)
    print(qty, item, "\t$"+str(cost), end="\n\n")
    total += float(price)*int(qty)
    price = "a"
    qty = "a"
    item = input("Enter item name or xyz to stop: ")
    
print(f"Total bill: ${total:.2f}")
````

<br/><br/><br/>

## 2a
````Python
n = 1
def GCD(x,y):
    global n
    if x==0 and y==0:
        print("\n\nUndefined")
        return
    elif y==0:
        print("\n\nGCD:", x)
        return
    elif x==0:
        print("\n\nGCD:", y)
        return
    if y>x:
        y,x = x,y
    new=x%y
    print("\n\nIteration: ", n, "\nNum 1: ", x, "\nNum 2: ", y, "\nRemainder: ", new)
    n+=1
    GCD(y,new)
    
n1 = int(input("Enter first number: "))
n2 = int(input("Enter second number: "))
GCD(n1, n2)
````
