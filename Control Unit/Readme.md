# Simple Control Unit

This project implements a **simple processor control unit** using **Logisim Evolution**. The design fetches instructions from memory, decodes the instruction fields, selects source and destination registers, and generates the required control signals for execution.

## Features

- 4 General Purpose Registers (R0–R3)
- Program Counter (PC)
- Instruction Memory (256 × 9)
- Opcode Register
- Source Register Selection
- Destination Register Decoder
- Multiplexer-based Operand Selection
- Controller/Decoder for Control Signal Generation

## Instruction Format

| Field | Size |
|---------|------|
| Opcode | 3 bits |
| Destination Register | 2 bits |
| Source Register 1 | 2 bits |
| Source Register 2 | 2 bits |

**Format:**

```
opcode(3) | dest(2) | src1(2) | src2(2)
```

## Components Used

- Registers
- Multiplexers
- Decoder
- RAM
- Program Counter
- Control Logic

## Working

1. The Program Counter provides the instruction address.
2. The instruction is fetched from instruction memory.
3. The Opcode Register stores the fetched opcode.
4. The Controller decodes the instruction and generates control signals.
5. Source registers are selected through multiplexers.
6. The destination register is selected using the decoder.
7. The result is written back to the selected register.

## Learning Outcomes

- Processor datapath organization
- Instruction fetch and decode
- Register file operations
- Control signal generation
- Basic CPU architecture

## Tools Used

- Logisim Evolution

## Future Enhancements

- ALU integration
- Immediate instructions
- Branch and jump instructions
- Load/Store operations
- Status flag support
