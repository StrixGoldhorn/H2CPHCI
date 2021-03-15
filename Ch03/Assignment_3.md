## 1
````Python
targ = int(input("Enter an integer: "))
total = 1
for i in range(1,targ+1):
    total = total*i
print(total)
````

<br/><br/><br/>

## 2
````Python
x,y,z = int(input("Enter side 1: ")), int(input("Enter side 2: ")), int(input("Enter side 3: "))
if x==y==z:
    print("Equilateral triangle")
else:
    print("Not equilateral")
````

<br/><br/><br/>

## 3
````Python
def main():
    cin = list(input("Enter a word: "))
    vowels = ['a','e','i','o','u']
    vc = 0
    lc = 0
    for i in cin:
        if i == " ":
            print("Not a word")
            return
        lc+=1
        if i in vowels:
            vc+=1
    print(f"Letters: {lc}\nVowels: {vc}\nPercentage of vowels: {(vc/lc)*100:.2f}")
main()
````

<br/><br/><br/>

## 4
````Python
def main():
    n = int(input("Enter an integer: "))
    print("*"*(2*n))
    for i in range(0,n-2):
        print("*", " "*(2*n-4),"*") 
    print("*"*(2*n))
main()
````

<br/><br/><br/>

## 5
````Python
import math
def main():
    maxd = -1
    maxi = -1
    for i in range(25,50):
        factors = []
        for j in range(1, round(math.sqrt(i))+1):
            if(i%j==0):
                factors.append(int(j))
                factors.append(int(i/j))
        factors = sorted(set(factors)) #typecast to set first, so can remove duplicates in sq numbers
        print(f"{i}: ", " ".join(str(i) for i in factors))
        t = sum(factors)
        if t>maxd:
            maxd = t
            maxi = i
        print(f"Sum of divisors: {t}\n")
    print(f"{maxi} has maximum sum of divisors")
            
main()
````

<br/><br/><br/>

## 6
````Python
import random
import sys

def roll():
    seed = random.randrange(sys.maxsize)
    rng = random.Random(seed)
    res = []
    res.append(random.randint(1,6))
    res.append(random.randint(1,6))
    res.append(seed)
    return res

def main():
    cnt = 0
    pot = int(input("Amount of money in pot: "))
    maxp = pot
    while pot!=0:
        res = roll()
        print(f"Dice rolled {res[0]} and {res[1]}. Seed used: {res[2]}")
        total = res[0]+res[1]
        if total == 7:
            pot+=4
            if maxp<pot:
                maxp=pot
        else:
            pot-=1
        cnt+=1
    print(f"\n\nNumber of rolls to break: {cnt}\nMax money in pot: ${maxp}")

main()    
````

<br/><br/><br/>

## 7
````Python
import random
import sys

def rng():
    res = []
    seed = random.randrange(sys.maxsize)
    random.seed(seed)
    num = random.randint(1,100)
    res.append(num)
    res.append(seed)
    return res

def n00b_binarysearch(cnt, l, r, ans):
    mid = l+ (r-l) // 2
    print(f"Try #{cnt+1}: {mid}")
    
    if mid == ans:
        print(f"Computer took {cnt+1} tries")
        return
    
    elif mid<ans:
        n00b_binarysearch(cnt+1, mid, r, ans)
    
    else:
        n00b_binarysearch(cnt+1, l, mid, ans)

def verA():
    cmpnum = rng()
    cnt = 1
    guess = int(input("Enter your guess: "))
    while guess!=cmpnum[0]:
        if guess<cmpnum[0]:
            print("Too small")
        else:
            print("Too large")
        cnt+=1
        guess = int(input("Enter your guess: "))
    print(f"You've got it in {cnt} tries!\nSeed used was {cmpnum[1]}")
    
def verB():
    usrnum = int(input("Enter a number: "))
    if usrnum>100 or usrnum<0:
        return print("Out of range")
    n00b_binarysearch(0, 1, 100, usrnum)
    
def main():
    play = input('"A" for Version A, or "B" for Version B: ').upper()
    if play == "A":
        verA()
    elif play == "B":
        verB()
    else:
        print("Invalid")

main()
````

<br/><br/><br/>

## Extra tools
````Python
#Test seeds
import random
x = 9164351046940259820 #seed goes here
random.seed(x)
print("Dice game: ", random.randint(1,6))
random.seed(x)
print("RNG Guessing game: ", random.randint(1,100))
````
