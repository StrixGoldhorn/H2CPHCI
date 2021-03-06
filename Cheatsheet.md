## Strix's Python Cheatsheet

### Menu UI
````Python
usr1 = input("blah blah blah")
exitcondition = "rawr"

while usr1 != exitcondition:
    somestatements = 1
    
    #psuedo-switchcase
    if usr1 == "alpha":
        dothis
    
    elif usr1 == "bravo":
        dothis
    
    elif usr1 == "charlie":
        dothat
    else:
        defaultstatment
    
    usr1 = input("check if usr wants to exit")
````

### RNGesus
````Python
import random
import sys

seed = random.randrange(sys.maxsize)
rng = random.Random(seed)
# run statements with random.blahblahblah
# seed is, well, the variable named seed
````
