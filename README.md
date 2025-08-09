# 8×8 LED Matrix Multiplexing with Two 74HC595 Shift Registers

## Overview

This project demonstrates how to control an **8×8 LED matrix** using **two 74HC595 shift registers** and simple multiplexing.

---

### Prerequisites

- A **basic** understanding of electronics
- **1 × Arduino** (Uno, Nano, or compatible)
- **2 × 74HC595 shift registers**
- **1 × 8×8 LED matrix**
- Breadboard & jumper wires

---

## Basic Idea
- **Shift register #1** controls the `columns`.
- **Shift register #2** controls the `rows`.
- Data is shifted into the shift registers while the `latch` pin is **low**, then the `latch` pin is pulled **high**, and then back to **low**.
- When the `latch` pin is **low**, the data is not being output from the **shift registers**.
- The active `column` is changed so quickly that it appears to form a still image.
