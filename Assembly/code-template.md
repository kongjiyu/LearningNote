# Template of initial code of Assembly
```asm
.model small
.stack 100

.data
msg db "This is my first assembly program!$"

.code
    mov ax, @data
    mov ds, ax

    ;write your code here

    ;exit
    mov ah, 4ch
    int 21h
end 
```