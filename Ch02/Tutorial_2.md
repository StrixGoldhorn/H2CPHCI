## 1
| Operations                                       | Values Returned                |
|--------------------------------------------------|--------------------------------|
| x + y                                            | 'dogcat'                       |
| "the" + x + "chase the" + y                      | 'thedogchase thecat'           |
| x*4                                              | 'dogdogdogdog'                 |
| print(x + y)                                     | dogcat                         |
| print(x,y)                                       | dog cat                        |

<br/><br/><br/>

## 2
| Code            | Output |
|-----------------|--------|
| round(10.6)     | 11     |
| int(10.6)       | 10     |
| round(10.666,2) | 10.67  |

<br/><br/><br/>

## 3
amount = 24.325
- a) `print("Your salary is $%0.2f" % amount)` Your salary is $24.32
- b) `print("The area is %0.1f" % amount)` The area is 24.3
- c) `print("%7f" % amount)` 24.325000
- d) `print("BMI btw {:f} and {:2.3f} is ideal".format(18.5,amount))` BMI btw 18.500000 and 24.325 is ideal
- e) `print("Overweight ={:>7.2f} – {:.2f}".format(amount, 29.9))` Overweight =  24.32 – 29.90

<br/><br/><br/>

## 4
````Python
print("%6s%6s%6s"%(x,y,z))
````

<br/><br/><br/>

## 5
````Python
import math
print(math.pow(8,2))
````
