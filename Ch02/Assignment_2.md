## 1
````Python
name = input("Name: ")
age = int(input("Age: "))
print("\nName:", name, "\nCurrent Age:", age, "\nAge in 10 years:", age+10)
````



## 2
````Python
import math
r = float(input("Radius: "))
print("\nDiameter:", 2*r, "\nCircumference:", math.pi*2*r, "\nVolume:", math.pi*4*r**2, "\nSphere:", (4/3)*math.pi*r**3)
````



## 3
````Python
wage = float(input("Hourly wage: $"))
reghr = float(input("Total regular hours: "))
othr = float(input("Total overtime hours: "))
print("Total weekly pay: $"+str(round(wage*reghr + othr*1.5*wage)))
````
