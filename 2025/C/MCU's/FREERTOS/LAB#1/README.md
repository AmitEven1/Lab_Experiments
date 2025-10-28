# 🧮 Language Lab – STM32 Fibonacci FreeRTOS Project

## Overview

This lab integrates **an STM32L452RE microcontroller (NUCLEO board)** with a **16x2 LCD display** and the **on-board red LED**.  
The objective is to design a **real-time Fibonacci sequence generator** using **FreeRTOS**, focusing on how to **structure and code APIs** for multitasking and inter-task communication.

---

## 🎯 Lab Purpose

> **Goal:**  
> Make the CPU calculate the Fibonacci sequence and display the results live on the LCD screen.  

This project emphasizes **learning the architecture and coding style of FreeRTOS APIs** — including task creation, delays, synchronization, and event-driven updates.

---

## ⚙️ System Description

### Boot Sequence

1. When powered on, the **MCU initializes FreeRTOS**, creates the necessary tasks, and configures the peripherals (LCD, LED, UART).  
2. The system **waits for input** specifying how many Fibonacci numbers to calculate.  
3. Initially, this input is **hardcoded or entered by the programmer** through source code (for simplicity).  
4. In the **next phase**, the input will be provided dynamically from the **PC via a Python CLI**.

---


