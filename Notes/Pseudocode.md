# A Dummies Guide to Pseudocode

<br/><br/><br/>

## Formatting
- `KEYWORDS` are in uppercase
- `VariablesLikeThis` are in camelCase
- `//Comments` are preceded by 2 forward slashes

<br/><br/><br/>

## Variables, Constants, Data Types

### Data Types
| Keywords   | Data Types             | Examples                                                     |
| ---------- |------------------------|--------------------------------------------------------------|
| `INTEGER`  | Whole numbers          | 1, 20, 300                                                   |
| `REAL`     | Real numbers           | 1/2, 2/3, 3/4                                                |
| `CHAR`     | One character          | "a", "A", "1"                                                |
| `STRING`   | Sequence of characters | "QWERTY", "Hello World", "123"                               |
| `BOOLEAN`  | True or False          | True, False                                                  |
| `DATE`     | Calendar date          | 11/09/2001, 11/11/2011                                       |

### Syntax
- Variable Declaration: `DECLARE <VarName> : <DataType>`
- Constants: `CONSTANT <VarName> : <Value>`
- Assignment: `<VarName> ← <Value>`

<br/><br/><br/>

## Arrays
### Delcaring Arrays
1D `DECLARE <VarName> : ARRAY[<LowerBound>:<UpperBound>] OF <DataType>`
2D `DECLARE <VarName> : ARRAY[<L1>:<U1>, <L2>:<U2>] OF <DataType>`


### Using Arrays
Changing/Assigning values:
1D `<VarName>[<Index>] ← <Value>`
2D `<VarName>[<Index1>, <Index2>] ← <Value>`
<br/>
Assigning an array
`<VarName1> ← <VarName2>`

<br/><br/><br/>

## Common Operations
### I/O
Input: `INPUT <VarName>`
Output: `OUTPUT <VarName or String>`
Output multiple: `OUTPUT <VarName or String>, <VarName or String>`


### Arithmetic Operations

| Operation      |  Operator |
|----------------|:---------:|
| Addition       |  +        |
| Subtration     |  -        |
| Multiplication |  *        |
| Division       |  /        |
| Modulo         |  MOD      |

- Resulting value is REAL
- Input can be REAL or INTEGER
- Augmented assignment (ie n += 3) NOT ALLOWED in pseudocode


### Relational Operations
| Operation                |  Operator |
|--------------------------|:---------:|
| Less than                |  <        |
| Greater than             |  >        |
| Less than or equal to    |  <=       |
| Greater than or equal to |  >=       |
| Equal to                 |  =        |
| Not equal to             |  <>       |
- Result is always BOOLEAN
- Not equal to is NOT `!=`


### Logic Operators
- AND, OR, NOT
- Result is always BOOLEAN

<br/><br/><br/>

## Selection
### IF
IF without ELSE<br/>
````
IF <condition>
  THEN
    <statement>
ENDIF
````

IF with ELSE<br/>
````
IF <condition>
  THEN
    <statement>
  ELSE
    <statement>
ENDIF
````

ELSEIF<br/>
````
IF <condition>
  <statement>
ELSE IF <condition>
  <statement>
ENDIF
ENDIF
````


### CASE
aka switch statements<br/>
````
CASE OF <VarName>
  <value1> : <statement1>
  <value2> : <statement2>
  OTHERWISE <statement>
ENDCASE
````
- Try to keep statements to one-liners, or use IF-ELSE
- `OTHERWISE` is optional
- No need to write `BREAK`

<br/><br/><br/>

## Iteration
### FOR
````
FOR <VarName> ← <Value1> TO <Value2> STEP <Increment>
  <statement>
ENDFOR
````
- Python's range() is NOT pseudocode
- `STEP` is optional
- `LENGTH(<string>)` to step through each char in `<string>`


### REPEAT UNTIL
aka do...while() in c++<br/>
````
REPEAT
  <statement>
UNTIL <condition>
````


### WHILE
````
WHILE <condition> DO
  <statement>
ENDWHILE
````

<br/><br/><br/>

## Procedures
aka functions without return<br/>
### Defining
Defining procedures without params<br/>
````
PROCEDURE <ProcedureName>
  <statement>
ENDPROCEDURE
````
Defining procedures with params<br/>
````
PROCEDURE <ProcedureName>(<Param1>:<DataType1>, <Param1>:<DataType1>)
  <statement>
ENDPROCEDURE
````


### Calling
Call procedure without params<br/>
````
CALL <ProcedureName>
````
Call procedure with params<br/>
````
CALL <ProcedureName>(<Value1>, <Value2>)
````

<br/><br/><br/>

## Functions
aka procedures but with return<br/>
### Defining
Defining functions without params<br/>
````
FUNCTION <FunctionName> RETURNS <DataType>
  <statement>
ENDFUNCTION
````
Defining functions with params<br/>
````
FUNCTION <FunctionName>(<Param1>:<DataType1>, <Param1>:<DataType1>) RETURNS <DataType>
  <statement>
ENDFUNCTION
````


### Calling
Call function without params<br/>
````
CALL <FunctionName>
````
Call function with params<br/>
````
CALL <FunctionName>(<Value1>, <Value2>)
````
