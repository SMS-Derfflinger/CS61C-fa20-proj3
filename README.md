# CS61CPU

This repository contains my solutions to the CS61C-fa20-proj3: A two-stage pipeline Risc-V CPU.

## Introduction

### Part A

- [x] Task 1: Arithmetic Logic Unit (ALU)
    * create an ALU that supports all the operations needed by the instructions in this ISA
        |Switch value|Introduction|
        |-|-|
        |0|add: `Result = A + B`|
        |1|and: `Result = A & B`|
        |2|or: `Result = A`|
        |3|xor: `Result = A ^ B`|
        |4|srl: `Result = (unsigned) A >> B`|
        |5|sra: `Result = (signed) A >> B`|
        |6|sll: `Result = A << B`|
        |7|slt: `Result = (A < B (signed)) ? 1 : 0`|
        |8|Unused|
        |9|Unused|
        |10|mul: `Result = (signed) (A * B)[31:0]`|
        |11|mulhu: `Result = (A * B)[63:32]`|
        |12|sub: `Result = A - B`|
        |13|bsel: `Result = B`|
        |14|mulh: `Result = (signed) (A * B)[63:32]`|
- [x] Task 2: Register File (RegFile)
    * RISC-V architecture has 32 registers. For this project we will implement all of them. 
- [x] Task 3: The Instruction `addi`
    * implement a CPU that’s capable of executing one instruction `addi` firstly.
    * Improved the single-cycle version to the two-stage pipeline version secondly.

### Part B

- [x] Task 4: More Instructions
    * Let the two-stage pipeline CPU support most RISC-V instructions.

You can see the introduction of this project on the course's home page: [course website](https://cs61c.org/fa20/), or in this website: [cs61c/projects/proj3](https://www.learncs.site/docs/curriculum-resource/cs61c/projects/proj3).
