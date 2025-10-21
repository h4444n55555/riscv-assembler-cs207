🧠 RISC-V Assembler — CS207 FCS Lab Project
📘 Overview

This project implements a RISC-V 64-bit assembler that converts RISC-V assembly instructions into their corresponding machine code (binary) format.
It replicates the assembler component of the Venus simulator, handling parsing, encoding, and output formatting for multiple instruction types.

Group Members:

👤 Nongmaithe Hans Nathanael Gabil Momin (2024AIB1011) — SPOC 

👤 Ravikant Sharma (2024AIB1013)

👤 Name 3

⚙️ Features

Converts assembly code from input.asm → machine code in output.mc

Supports RISC-V 64-bit base ISA instructions (RV64I)

Handles label resolution and instruction addressing

Produces detailed machine code output format:
<address> <machine_code> , <assembly_instruction> # <opcode-func3-func7-rd-rs1-rs2-immediate>

Separate handling for .text and .data segments

Basic support for assembler directives:
.text, .data, .byte, .half, .word, .dword, .asciz

🧩 Supported Instructions
R-Format
add, addw, and, or, sll, slt, sra, srl, sub, subw, xor, mul, mulw, div, divw, rem, remw

I-Format
addi, addiw, andi, ori, lb, ld, lh, lw, jalr

S-Format
sb, sw, sh, sd

SB-Format
beq, bne, bge, blt

U-Format
auipc, lui

UJ-Format
jal
