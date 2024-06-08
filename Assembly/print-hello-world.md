# Print Hello World in Assembly
Note:
```
{} mean u can write any name to replace the bracket
For example:
{variable name} -> msg
```
There is 3 thing you need to do to print a value in assembly
## 1. Declare a variable in .data section
- 10, 13 is the ASCII code for newline and carriage return
- When add 10, 13, it will print the variable in a new line
- $ is something like /0 in c
```
{variable name} DB value
Example:
msg DB 10, 13, "Hello World!$"
```
## 2. let DX register reference to the variable address
```
LEA DX, msg
```
## 3. move 09H to AH register and call INT 21H
```
MOV AH, 09H
INT 21H
```

# You can create a function to print a string
```assembly
;LEA DX, {variable name}
print_string PROC
    MOV AH, 09H
    INT 21H
    RET
print_string ENDP
```