# 64-bit IEEE 754 Floating Point Unit (FPU) in Verilog

This project implements a **64-bit IEEE 754-compliant Floating Point Unit (FPU)** in Verilog, supporting **addition**, **subtraction**, **multiplication**, and **division** on double-precision values.

---

## Overview

The FPU supports:
- **Double-precision floating point arithmetic** (64-bit IEEE 754 format)
- Modular Verilog design
- Handling of **special cases**: zero, infinity, NaN, and denormalized numbers
- **Two Verilog testbenches** for functionality and edge-case validation

---

## Supported Operations

| Operation      | `op` value |
|----------------|------------|
| Addition       | `2'b00`    |
| Subtraction    | `2'b01`    |
| Multiplication | `2'b10`    |
| Division       | `2'b11`    |

---

## 📁 Project Structure

```bash
.
├── fpu.v                   # Top-level FPU module
├── fpu_add_sub.v           # Addition/Subtraction logic
├── fpu_mul.v               # Multiplication logic
├── fpu_div.v               # Division logic
├── fpu_tb1.v               # Testbench 1 – basic arithmetic with real output
├── fpu_tb2.v               # Testbench 2 – extended tests with edge cases
└── README.md               # This file
