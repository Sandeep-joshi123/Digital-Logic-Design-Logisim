# 8×8 Register File

This project implements an **8×8 Register File** using **Logisim Evolution**. The design consists of eight 8-bit registers with **one write port** and **two independent read ports**, allowing simultaneous access to stored data.

## Features

- 8 Registers (R0–R7)
- 8-bit Data Width
- Single Write Port
- Dual Read Ports
- Decoder-based Register Selection
- Multiplexer-based Read Operation
- Clock-controlled Write Operation

## Inputs

- **WriteData** – 8-bit data to be written
- **WriteAdrs** – 3-bit write address
- **ReadAdrs1** – 3-bit address for Read Port 1
- **ReadAdrs2** – 3-bit address for Read Port 2
- **Clk** – Clock signal for write operation

## Outputs

- **ReadPort1** – Data from the selected register
- **ReadPort2** – Data from the selected register

## Components Used

- 8-bit Registers
- 3-to-8 Decoder
- 8-to-1 Multiplexers
- Clock Signal
- Wiring Logic

## Working

1. The **WriteAdrs** is decoded to select one of the eight registers.
2. On the clock edge, **WriteData** is stored in the selected register.
3. **ReadAdrs1** selects the data for **ReadPort1** through a multiplexer.
4. **ReadAdrs2** independently selects the data for **ReadPort2**, enabling simultaneous reads.

## Learning Outcomes

- Register file organization
- Address decoding
- Multiplexer-based data selection
- Synchronous write and asynchronous read operations
- Processor datapath design

## Tools Used

- Logisim Evolution

## Future Enhancements

- Write Enable control
- Reset functionality
