# 🧮 Language Lab – STM32 Fibonacci FreeRTOS Project

## Overview

This project uses an **STM32L452RE (NUCLEO board)** with a **16x2 LCD** and the **on-board red LED** to show the Fibonacci sequence in real time.  
It’s built to help me understand how to use **FreeRTOS** — how tasks work, how timing is handled, and how different parts of a system talk to each other.

---

## 🎯 Purpose

The goal is simple:  
Make the MCU calculate Fibonacci numbers and show them live on the LCD while I learn how to write FreeRTOS code from scratch.  
This lab is about learning by doing — understanding how the OS works, not just using it.

---

## ⚙️ How It Works

1. When the board powers up, it initializes **FreeRTOS**, **LCD**, and **LED**.  
2. The system waits for an input — how many Fibonacci numbers to calculate.  
3. At first, the input will just be written directly in the code.  
4. Later, a **Python CLI (fully AI-generated)** will send that number through **UART**.  
5. The MCU will catch the data with an interrupt, save it in a buffer, and start the Fibonacci task.

---

## 🧠 What I’m Coding vs. What AI Handles

| Component | Who Codes It | Why |
|------------|--------------|-----|
| **FreeRTOS tasks (creation, delay, sync)** | **Me** | To fully learn how the API and scheduling work |
| **Fibonacci logic & LCD updates** | **Me** | To practice algorithm design and real-time display |
| **UART interrupt & buffer** | **Me** | To learn data handling and interrupt flow |
| **System integration & debugging** | **Me + AI** | To connect everything cleanly and fix timing issues |
| **LCD driver (I2C)** | **AI-generated** | Already done, saves time for core learning |
| **Python CLI** | **AI-generated** | Focus is on MCU side, not PC scripting |

> 🧩 **No vibe-coding** for: FreeRTOS APIs, Fibonacci logic, and interrupt handling — these are written fully by me for learning.

---

## 💡 Why It Matters

- Shows FreeRTOS in action on real hardware  
- Combines human learning with AI assistance  
- Builds a complete workflow: PC → MCU → LCD  
- Turns abstract OS ideas into something visible and alive  

---

**Hardware:** STM32L452RE (NUCLEO) + LCD 16x2 (I2C) + onboard LED  
**Focus:** Learn FreeRTOS step by step through a working Fibonacci system  
**Next Phase:** Add Python CLI → UART → Interrupt → Buffer → FreeRTOS Task
