# Read String in assembly language
Note:
```
{} mean u can write any name to replace the bracket
For example:
{variable name} db "Hello World" -> msg db "Hello World"
```
There is 3 thing you need to do to print a value in assembly
## 1. Define a string buffer
- The first 6 represents the size of the buffer
- The zero means how many characters contain
- The 6 dup(' ') is insert spaces to fill the buffer
```assembly
{variable name} db 6, 0, 6 dup(' ')
Example:
input db 10, 0, 10 dup(' ')
```

## 2. Let DX register reference to the variable address
```assembly
LEA DX, input
```
## 3. Move 0AH to AH register and call INT 21H
```assembly
MOV AH, 0AH
INT 21H
```

# You can create a function to read a string
```assembly
;LEA DX, {variable name} <- do this before call this 
read_string PROC
    MOV AH, 0AH
    INT 21H
    RET
read_string ENDP
```