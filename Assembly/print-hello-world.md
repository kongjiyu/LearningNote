# Print Hello World in Assembly
Note:
```
{} mean u can write any name to replace the bracket
For example:
{variable name} -> msg
```
There is 3 thing you need to do to print a value in assembly
## 1. Declare a variable in .data section
- $ is something like /0 in c
```
{variable name} DB value
Example:
msg DB "Hello World!$"
```
## 2. let DX register reference to the variable
```
LEA DX, msg
```
## 3. move 09H to AH register and call INT 21H
```
MOV AH, 09H
INT 21H
```