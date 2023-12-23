
- A (7th bit): Addressing Mode Bit 1
- B (6th bit): Addressing Mode Bit 2
- O (5 bits): Opcode

## Addressing Modes

The 7th and 6th bits determine the addressing mode according to the following table:

| A | B | Addressing Mode |
|---|---|------------------|
| 0 | 0 | Immediate        |
| 0 | 1 | Memory            |
| 1 | 0 | Accumulator       |
| 1 | 1 | Unused            |

## Opcode Table


| Opcode (Binary) | Mnemonic | Description                             | Addressing Modes                 |
|------------------|----------|-----------------------------------------|----------------------------------|
| 00000            | ADD      | Add two operands                        | Memory, Immediate,  Accumulator              |
| 00001            | SUB      | Subtract two operands                   | Memory, Immediate, Accumulator              |
| 00010            | LDA      | Load accumulator from memory            | Memory, Immediate                           |
| 00011            | STR      | Store accumulator to memory             | Memory                           |
| 00100            | JMP      | Jump to a specified address             | Memory                           |
| 00101            | CMP      | Compare two operands                    |Accumulator,Immediate             |
| 00110            | CALL     | Call a subroutine                       | Memory                           |
| 00111            | NOT      | Perform bitwise NOT on the accumulator | Accumulator                      |
| 01000            | HLT      | Halt the CPU                            | Unused                           |
| 01001            | MOV      | Move data from one location to another  | Memory, Accumulator              |
| 01010            | XOR      | Perform bitwise XOR operation           | Memory, Accumulator              |
| 01011            | AND      | Perform bitwise AND operation           | Memory, Accumulator              |
| 01100            | OR       | Perform bitwise OR operation            | Memory, Accumulator              |




