# 7-Day Foundations-First Electronics, PCB & Embedded Systems Plan

This repository documents my focused 7-day learning sprint to **convert partial / intuitive knowledge into solid engineering fundamentals** across **electronics, PCB design, and embedded systems**.

The goal is not just to build things, but to **understand WHY they work**.

---

## 🧠 Why This Plan Exists

I realized that much of my work so far has been based on:
- intuition
- examples
- trial and error
- “it works” thinking

This plan is designed to **fill foundational gaps** and eliminate *half-knowledge* by deeply understanding:
- trace width
- current flow
- return paths
- grounding
- power integrity
- signal integrity

---

## 🎯 Core Goals
- Strengthen **fundamentals behind real-world designs**
- Understand **PCB decisions mathematically and physically**
- Be able to **explain every trace, capacitor, and resistor**
- Build confidence as a **system-level engineer**

---

## ⏱ Time Commitment
- **2–3 hours per day**
- Learning + applying + documenting

---

## 📅 Day-wise Learning Plan

---

### 🔹 Day 1 – Core Electronics (No Assumptions)
**Focus**
- Ohm’s Law (real current flow, not formulas)
- KCL & KVL in actual circuits
- What voltage really means
- Pull-up vs pull-down resistors
- Voltage dividers (loading effect)
- Why decoupling capacitors are mandatory

**Hands-on**
- Take one old schematic
- For **every component**, answer:
  - What happens if I remove this?
  - What happens if its value doubles?

**Deliverable**
- `day1-electronics-basics.md`
- Annotated schematic screenshots

---

### 🔹 Day 2 – Power Design & Current Thinking
**Focus**
- How current flows from source to load
- LDO vs Buck vs Boost (efficiency math)
- Battery basics (internal resistance)
- Reverse polarity protection
- TVS diodes & ESD
- Why bulk + ceramic capacitors are both needed

**Hands-on**
- Redesign power input section
- Calculate:
  - expected current
  - power loss
  - thermal risk

**Deliverable**
- Power path diagram
- `day2-power-and-current.md`

---

### 🔹 Day 3 – PCB Trace Width & Copper Fundamentals (CRITICAL)
**Focus**
- What trace width actually means
- Current density in copper
- IPC trace width basics
- Why short & wide traces matter
- Copper pours vs traces
- Via current limits

**Hands-on**
- Take one PCB
- Identify:
  - under-sized power traces
  - unnecessary thin routes
  - missing copper pours

**Deliverable**
- Trace width calculations
- Before/After PCB images
- `day3-trace-width.md`

---

### 🔹 Day 4 – Grounding, Return Paths & EMI Basics
**Focus**
- What “ground” really is
- Return current paths
- Why signals don’t travel alone
- Ground loops
- Why split grounds often fail
- Stitching vias and planes

**Hands-on**
- Highlight return paths for:
  - SPI
  - I2C
  - Power rails
- Fix broken ground paths

**Deliverable**
- Return-path diagrams
- `day4-grounding.md`

---

### 🔹 Day 5 – Signal Integrity (Basics Only, Done Right)
**Focus**
- Digital vs analog signals
- Crystal routing rules
- Why clock traces fail
- SPI vs I2C routing mistakes
- Series resistors & damping

**Hands-on**
- Audit one board for:
  - crystal placement
  - noisy analog routing
- Improve layout

**Deliverable**
- Signal checklist
- `day5-signal-basics.md`

---

### 🔹 Day 6 – Embedded Firmware + Hardware Interaction
**Focus**
- MCU boot sequence
- GPIO electrical limits
- Interrupts vs polling
- Sleep modes & power impact
- Firmware mistakes that damage hardware

**Hands-on**
- Map firmware behavior to hardware events
- Identify power leaks in code

**Deliverable**
- Firmware flow diagram
- `day6-firmware-hardware.md`

---

### 🔹 Day 7 – System Thinking & Proof of Understanding
**Focus**
- How all blocks interact
- Design trade-offs
- Cost vs performance vs power
- Manufacturing constraints
- What I would redesign today

**Hands-on**
- Write one **complete case study**
- Explain:
  - design decisions
  - mistakes
  - learnings

**Deliverable**
- `case-study.md`
- Final polished repo

---

## 📂 Repository Structure
