# Simple 8-bit Processor

This project implements a **Simple 8-bit Processor** using **Logisim Evolution**, integrating core processor components such as an Instruction Memory, Register File, ALU, Control Unit, Program Counter, and Status Register. The processor fetches, decodes, and executes basic arithmetic instructions.

## Features

- 8-bit Processor Architecture
- Instruction Fetch and Decode
- Register-based Operations
- 8-bit ALU
- Program Counter (PC)
- Instruction Register (IR)
- Memory Data Register (MDR)
- Register File
- Status Register (N, Z, C, V Flags)
- Control Unit for Instruction Execution

## Instruction Format

| Field | Size |
|---------|------|
| Opcode | 3 bits |
| Destination Register | 3 bits |
| Source Register 1 | 3 bits |
| Source Register 2 | 3 bits |

```
opcode(3) | dest(3) | src1(3) | src2(3)
```

## Supported Instructions

| Opcode | Operation |
|----------|-----------|
| 000 | ADD |
| 001 | SUB |

## Processor Components

- Instruction Memory (256 × 12)
- Program Counter (PC)
- Memory Data Register (MDR)
- Instruction Register (IR)
- Register File
- Arithmetic Logic Unit (ALU)
- Control Unit
- Status Register

## Working

1. The Program Counter fetches an instruction from Instruction Memory.
2. The instruction is loaded into the Instruction Register.
3. The Control Unit decodes the opcode and register fields.
4. Source operands are read from the Register File.
5. The ALU performs the selected arithmetic operation.
6. The result is written back to the destination register.
7. The Status Register updates the N, Z, C, and V flags.

## Learning Outcomes

- Basic processor architecture
- Instruction fetch-decode-execute cycle
- Register file organization
- ALU integration
- Control signal generation
- Status flag management

## Tools Used

- Logisim Evolution

## Future Enhancements

- Logical operations (AND, OR, XOR)
- Load/Store instructions
- Branch and Jump instructions
- Immediate operands
- Shift operations
- Expanded instruction set
