## 1
1) `1 2 3 4 5 `
2) `1 2 3`
3) `1 3 5`
4) `6 5 4 3 2`

<br/><br/><br/>

## 2
````Python
name = "John Doe"
for i in range(50):
    print(name)
````

<br/><br/><br/>

## 3
````Python
for i in range(1,129):
    print(i, chr(i))
````

<br/><br/><br/>

## 4
````Python
testString = "Hello World"
testString = list(testString)
for i in testString:
    print(i, ord(i))
````

<br/><br/><br/>

## 5
````Python
testString = "Hello World"
testString.count(" ")
````

<br/><br/><br/>

## 6
````Python
usr = int(input("Number of iterations: "))
approx = 0
for i in range(1,usr+1):
    n = 2*i-1
    if i%2==1:
        approx += (1/n)
    else:
        approx -= (1/n)
print("π/4: ", approx)
print("π: ", approx*4)
````

<br/><br/><br/>

## 7
````Python
temp = input("Temperatures: ").split(", ")
total = 0
cnt = 0
for i in temp:
    if int(i)>0:
        total+=int(i)
        cnt+=1
if  total == 0:
    print("No days above freezing")
else:
    print(total/cnt)

# Sample input: 10, 20, 23, -2, -1000, -4, 0, 41
````

<br/><br/><br/>

## 8
````Python
fencelen = int(input("Fence length: "))
print("Length   Area\n")
maxa = -1

for i in range(1, round(fencelen/2)):
    area = round(i*((100-2*i)/2))
    space = 11 - len(str(i)) - len(str(area))
    print(i, " "*space, area)
    maxa = max(maxa, area)
print("\nMaximum area is: ", maxa)
````

<br/><br/><br/>

## 9
````Python
recur = int(input("Number of columns: "))
for i in range(1, recur+1):
    for j in range(1, i+1):
        print(i*j, end=" ")
    print("")
````

<br/><br/><br/>
