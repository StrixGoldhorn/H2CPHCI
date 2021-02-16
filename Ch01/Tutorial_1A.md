## Q1
````
BEGIN

		READ Mark
 
		CASE Mark
			Mark>69
				PRINT "A"
				BREAK
      
			Mark>59
				PRINT "B"
				BREAK
      
			Mark>54
      	PRINT "C"
				BREAK

			Mark>49
				PRINT "D"
				BREAK
    
			Mark>44
				PRINT "E"
				BREAK
     
			Mark>39
				PRINT "S"
				BREAK

			OTHERWISE
				PRINT "U"
				BREAK
		END-CASE
 
END
````

<br/><br/><br/>

## Q2

````
BEGIN

READ GrossIncome, Dependents
GrossIncome -= 10000
GrossIncome -= Dependents*2000
IncomeTax = 0.2*GrossIncome
PRINT IncomeTax

END
````
