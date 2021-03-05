## 1
a) rejects if score is less than 90<br/>
b) rejects if not eligible

<br/><br/><br/>

## 2
a) will never get a band 1, since it escapes before checking if score >=85, since score >= 70 was the first condition<br/>
b) is ineffecient, as there is no need to check more once score is >=85

<br/><br/><br/>

## 3
````Python
x = "abcde"
y = "vwxyz"
if x<y:
    print(x,y)
else:
    print(y,x)
````

<br/><br/><br/>

## 4
````Python
gi = int(input("Gross Income: "))
dep = int(input("Depenedents: "))
gi -= 10000
gi -= dep*2000
it = 0.2*gi
if it<0:
    print("Income Tax: $0")
else:
    print("Income Tax: $"+str(it))
````

<br/><br/><br/>

## 5
````Python
p1 = ord(str(input("Player 1: ").upper())[0:1])
p2 = ord(str(input("Player 2: ").upper())[0:1])

#basic validation
allowed = [80, 82, 83]
if p1 not in allowed or p2 not in allowed:
    print("Invalid input detected.")

#fun
p1win = [-1, -2, 3]
#p2win = [-3, 1, 2]
    
if p1 == p2:
    print("Tie, both players played:", chr(p1))
elif p1-p2 in p1win:
    print("Player 1 wins")
else:
    print("Player 2 wins")
````
