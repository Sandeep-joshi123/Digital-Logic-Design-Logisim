# 2×2 Array Multiplier

This project implements a **2×2 Binary Array Multiplier** using **Logisim Evolution**. The circuit generates partial products using AND gates and combines them using combinational logic to produce a 4-bit multiplication result.

## Features

- 2-bit × 2-bit Binary Multiplication
- Partial Product Generation
- Combinational Logic Implementation
- 4-bit Product Output

## Inputs

- `a1 a0` – First 2-bit operand
- `b1 b0` – Second 2-bit operand

## Outputs

- `p[3:0]` – 4-bit multiplication result

## Components Used

- AND Gates
- XOR Gates
- Basic Combinational Logic

## Working

1. Partial products are generated using AND gates.
2. The partial products are added using XOR and AND gates.
3. The final 4-bit product is obtained as `p[3:0]`.

## Learning Outcomes

- Binary multiplication using array architecture
- Partial product generation
- Combinational arithmetic circuit design
- Hardware implementation of multiplication logic

## Tools Used

- Logisim Evolution
