# Register in CPU

## All register
![All register in CPU](image/CPU-register.gif)

### When you want to use 16-bit variable
- Use AX, BX, CX or DS register

### When you want to use 8-bit variable
- Use AL, BL, CL or DL register
- Use AH, BH, CH or DH register

### List of registers
- [AX (Accumulator Register)](#ax-register-accumulator-register)
- [BX (Base Register)](#bx-register-base-register)
- [CX (Count Register)](#cx-register-count-register)
- [DX (Data Register)](#dx-register-data-register)
- [SI (Source Index Register)](#si-register-source-index-register)
- DI (Destination Index Register)
- SP (Stack Pointer Register)
- BP (Base Pointer Register)
- IP (Instruction Pointer Register)
- CS (Code Segment Register)
- DS (Data Segment Register)
- SS (Stack Segment Register)
- ES (Extra Segment Register)
- Flags (Status Register)


#### AX register (Accumulator Register)

##### Common Uses:
- **Arithmetic operations**: Many arithmetic operations (e.g., MUL, DIV, ADD, SUB) use AX as the default operand.
- **Input/Output operations**: Often used in conjunction with IN and OUT instructions.
- **String operations**: AX is used in instructions like LODSB (load string byte) and STOSB (store string byte).

#### BX register (Base Register)

##### Common Uses:
- **Addressing memory**: BX is often used as a base pointer for memory addressing with instructions like MOV.
- **Data manipulation**: General-purpose data storage and manipulation.

#### CX register (Count Register)

##### Common Uses:
- **Loop counters**: CX is traditionally used as a loop counter with the LOOP instruction.
- **Shift/rotate operations**: The CL register is used to specify the count in shift and rotate instructions (e.g., SHL, SHR, ROL, ROR).

#### DX register (Data Register)

##### Common Uses:
- **I/O operations**: Often used to specify ports in IN and OUT instructions.
- **Multiplication and Division**: DX:AX pair is used for the results of multiplication (MUL) and division (DIV) operations, where DX holds the high-order word.
- **Data transfer**: Used in conjunction with AX for data transfer operations.

#### SI register (Source Index Register)

##### Common Uses:
- **Source Index**: As its name implies, SI is often used as a pointer to the source data in string operations.
- **16-bit Register**: SI is a 16-bit register, meaning it can address memory locations up to 65535 in real mode.