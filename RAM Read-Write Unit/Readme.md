# RAM Read/Write Unit

This project implements a **RAM Read/Write Unit** using **Logisim Evolution**. The design demonstrates basic memory operations with dedicated registers for address, data, and instruction handling, along with a Program Counter for sequential memory access.

## Features

- 256 × 8 RAM
- Memory Address Register (MAR)
- Memory Data Register (MDR)
- Instruction Register (IR)
- Program Counter (PC)
- PC Incrementer
- Read and Write Operations
- Configurable Initial Address

## Components Used

- RAM (256 × 8)
- Program Counter (PC)
- Memory Address Register (MAR)
- Memory Data Register (MDR)
- Instruction Register (IR)
- Multiplexer
- Adder (PC Incrementer)
- Registers

## Working

1. The **Program Counter (PC)** generates the memory address.
2. The address is loaded into the **Memory Address Register (MAR)**.
3. During a **Read** operation, data from RAM is loaded into the **Memory Data Register (MDR)** and can be transferred to the **Instruction Register (IR)** or Read Data output.
4. During a **Write** operation, input data is stored into the selected RAM location.
5. The **PC Incrementer** updates the Program Counter for sequential memory access.

## Learning Outcomes

- Memory organization
- Read and write cycle implementation
- Program Counter operation
- Register-based memory interfacing
- Basic processor memory subsystem design

## Tools Used

- Logisim Evolution

## Future Enhancements

- Load/Store instructions
- Variable address width
