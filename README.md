# 
# Table of Content

- [what is digital electronics](#what-is-digital-electronics)
- [Applications of Digital Electronics](#Applications-of-Digital-Electronics)
- [Digital vs Analog signals](#Digital-vs-Analog-signals)
- [LOGIC LEVELS](#LOGIC-LEVELS)
- [NUMBER SYSTEM](#NUMBER-SYSTEM)
- [Conversion between number system](#Conversion-between-number-system)
- [BASIC LOGIC GATES](#BASIC-LOGIC-GATES)
- [ Integrated Circuits](#Integrated-Circuits)
- [ IMPLEMENTATION OF GATES](#IMPLEMENTATION-OF-GATES)
- [ IMPLEMENTATAION OF HALF ADDER](#IMPLEMENTATAION-OF-HALF-ADDER)
- [IMPLEMENTATION OF FULL ADDER](IMPLEMENTATION-OF-FULL-ADDER)


- 





# what is digital electronics

DEFINATION:
Definition	Digital electronics is a branch of electronics that deals with digital signals — signals that have only two discrete levels: HIGH (1) and LOW (0). It is the foundation of computers, digital communication, and modern electronic devices.

# Applications of Digital Electronics

Applications	Used in:
• Computers, Laptops
• Digital Watches
• Mobile Phones
• Calculators
• Robotics
• Digital Control Systems
Applications	Found in almost all modern electronics: computers, smartphones, digital cameras, smart TVs, automotive systems, robotics, automation, and more.

# Digital vs Analog signals

| **Feature**                | **Digital Electronics**                                                  | **Analog Electronics**                                                          |
| -------------------------- | ------------------------------------------------------------------------ | ------------------------------------------------------------------------------- |
| **Signal Type**            | Discrete (two levels: 0 and 1)                                           | Continuous (infinite range of values)                                           |
| **Representation**         | Binary numbers (e.g., 101010)                                            | Voltage or current that varies smoothly over time                               |
| **Accuracy**               | High precision due to fixed logic levels                                 | Susceptible to noise and distortion, reducing accuracy                          |
| **Noise Immunity**         | High – digital signals are easily distinguished from noise               | Low – small noise can cause significant distortion                              |
| **Circuit Complexity**     | Can be complex in structure but easier to analyze and design using logic | Generally simpler circuits but harder to analyze due to varying signal behavior |
| **Data Storage**           | Easy and efficient (in binary format)                                    | Difficult and less reliable                                                     |
| **Examples of Components** | Logic gates, flip-flops, microcontrollers, FPGAs                         | Resistors, capacitors, transistors, op-amps                                     |
| **Signal Processing**      | Based on binary logic, uses processors and algorithms                    | Continuous-time processing, uses amplifiers, filters, and mixers                |
| **Conversion Required**    | Requires ADC/DAC to interface with the real world                        | No conversion needed for real-world analog signals                              |
| **Power Consumption**      | Generally lower (especially CMOS), though varies with speed              | Can be higher due to continuous operation                                       |
| **Application Examples**   | Computers, smartphones, calculators, digital watches, robotics           | Audio amplifiers, radio, analog sensors, old televisions                        |
| **Scalability**            | Highly scalable (integrated circuits, miniaturization possible)          | Less scalable for complex systems                                               |
| **Design Tools**           | Boolean algebra, logic circuits, HDLs                                    | Kirchhoff’s laws, differential equations, frequency analysis                    |
| **Reliability**            | More reliable due to error correction and immunity to signal degradation | Less reliable in long-distance transmission or noisy environments               |
| **Cost (Modern Era)**      | Often lower due to mass production and integration                       | May be higher in complex analog signal environments                             |

# LOGIC LEVELS 
In digital electronics, logic levels refer to the specific voltage ranges that represent binary states — typically 0 (LOW) and 1 (HIGH). These levels indicate how the digital system interprets voltages as logical TRUE (1) or FALSE (0).
## Logic Levels Table

| Logic Level | Digital Value | Voltage Range (Typical for TTL) | Voltage Range (Typical for CMOS) |
|-------------|---------------|-------------------------------|----------------------------------|
| LOW         | 0             | 0V to 0.8V                    | 0V to 1.5V                       |
| HIGH        | 1             | 2V to 5V                      | 3.5V to 5V (or 3.3V, depending)  |
| Undefined   | -             | 0.8V to 2V                    | 1.5V to 3.5V                     |


LOGIC LEVELS

Logic 0 (LOW)

Logic 1 (HIGH)

- Digital circuits operate using only these two levels to interpret data, control operations, and perform computations.

1. Logic LOW (0)

- Logic 0, also called LOW, represents the binary value 0.



2. Logic HIGH (1)

- Logic 1, also called HIGH, represents the binary value 1.




# TTL (Transistor-Transistor Logic) – typically 5V system:

Logic 0 (LOW): 0V to 0.8V

Logic 1 (HIGH): 2V to 5V

Undefined Zone: 0.8V to 2V (should be avoided)


# CMOS (Complementary Metal-Oxide-Semiconductor) – flexible with V<sub>DD</sub>:


If V<sub>DD</sub> = 5V:


Logic 0: 0V to ~1.5V


Logic 1: ~3.5V to 5V


CMOS systems have higher noise immunity and can operate at lower voltages (e.g., 3.3V, 1.8V).


 # NUMBER SYSTEM

 A number system is a way to represent and express numbers using a set of symbols or digits. In digital electronics, number systems are used to represent data and perform calculations inside digital circuits and computers.

# Different number systems are BINARY, OCTAL,DECIMAL, HEXADECIMAL


| Number System | Base | Symbols Used       | Example | Description                                 |
|---------------|------|---------------------|---------|---------------------------------------------|
| **Binary**     | 2    | 0, 1                | 1011    | Used in all digital circuits and logic gates |
| **Octal**      | 8    | 0–7                 | 75      | Compact representation of binary (3 bits)   |
| **Decimal**    | 10   | 0–9                 | 245     | Standard human-readable number system       |
| **Hexadecimal**| 16   | 0–9, A–F            | 3F      | Common in memory addresses and color codes  |

# Conversion between number system

# 1.Binary → Decimal
Binary: 1011₂

= (1×2³) + (0×2²) + (1×2¹) + (1×2⁰)

= 8 + 0 + 2 + 1

= 11₁₀

-------------

# 2.Decimal → Binary

 Decimal `13` to Binary

| Step | Division      | Quotient | Remainder |
|-------|---------------|----------|-----------|
| 1     | 13 ÷ 2 = 6   | 6        | 1         |
| 2     | 6 ÷ 2 = 3    | 3        | 0         |
| 3     | 3 ÷ 2 = 1    | 1        | 1         |
| 4     | 1 ÷ 2 = 0    | 0        | 1         |

Read remainders bottom to top: 1101

Decimal 13 = Binary 1101

---------------

# 3.Binary → Octal
Binary: 110110₂

Group in 3 bits → 110 | 110

110₂ = 6₈

110₂ = 6₈

Result → 66₈

-----------
# 4.Octal → Binary

 Octal: 725 to Binary

| Octal Digit | Binary (3 bits) |
|-------------|-----------------|
| 7           | 111             |
| 2           | 010             |
| 5           | 101             |

Result →  
Octal 725 = Binary 111010101

----------------

# 5.Binary → Hexadecimal
Convert Binary: 10111110 to Hexadecimal

| Binary Group | Decimal Equivalent | Hexadecimal Digit |
|--------------|--------------------|-------------------|
| 1011         | 11                 | B                 |
| 1110         | 14                 | E                 |

Result → 
Binary 10111110 = Hexadecimal **BE**

---
 

# 6.Hexadecimal → Binary
Hexadecimal `3F9` to Binary

| Hex Digit | Binary (4 bits) |
|-----------|-----------------|
| 3         | 0011            |
| F         | 1111            |
| 9         | 1001            |

Result → 
Hexadecimal 3F9 = Binary 001111111001


----------------


# 7.Decimal → Octal
 Convert Decimal `156` to Octal

| Step | Division        | Quotient | Remainder |
|-------|-----------------|----------|-----------|
| 1     | 156 ÷ 8 = 19    | 19       | 4         |
| 2     | 19 ÷ 8 = 2      | 2        | 3         |
| 3     | 2 ÷ 8 = 0       | 0        | 2         |

Read remainders from bottom to top: 2 3 4

Decimal 156 = Octal 234


------------------


# 8.Octal → Decimal
Octal: 745₈

= (7×8²) + (4×8¹) + (5×8⁰)

= (7×64) + (4×8) + (5×1)

= 448 + 32 + 5

= 485₁₀

----------------

# 9.Decimal → Hexadecimal
   
Decimal: 254₁₀

254 ÷ 16 = 15 remainder 14 (E)

15 ÷ 16 = 0 remainder 15 (F)

Read remainders bottom to top → FE₁₆

-------------------

# 10.Hexadecimal → Decimal
Hex: 2A₁₆

= (2×16¹) + (A×16⁰)

= (2×16) + (10×1)

= 32 + 10

= 42₁₀

-------------------

# 11.Octal → Hexadecimal
Octal: 745₈

Step 1: Octal → Binary

7 → 111

4 → 100

5 → 101

Binary = 111100101₂

Step 2: Binary → Hex

Group 4 bits: 0011 | 1100 | 101 (pad left 0 → 0101)

0011 → 3

1100 → C

0101 → 5

Result → 3C5₁₆

--------------------

# 12.Hexadecimal → Octal
Hex: 2F₁₆

Step 1: Hex → Binary

2 → 0010

F → 1111

Binary = 00101111₂

Step 2: Binary → Octal
Group 3 bits: 000 | 101 | 111

000 → 0

101 → 5

111 → 7

Result → 057₈

-------------------

# BASIC LOGIC GATES

# 1.AND GATE

# Symbol:

![image](https://github.com/user-attachments/assets/cc423310-cf10-4e14-910a-b006e5131efe)

A curved-shaped gate with two inputs and one output.

# AND GATE IC

![image](https://github.com/user-attachments/assets/9a380fcd-28bc-47af-b809-bfcf3ebffa23)


# Function:
The AND gate outputs 1 (true) only when both inputs are 1. Otherwise, it outputs 0.

 *A.B=X.
 
 *The value of X will be True when both the inputs will be True.
 
# Truth Table:


| Input A | Input B | Output (A · B) |
|---------|---------|----------------|
|    0    |    0    |       0        |
|    0    |    1    |       0        |
|    1    |    0    |       0        |
|    1    |    1    |       1        |

# Logic Expression:
Output = A · B

- The AND gate outputs `1` only when **both inputs are 1**.

- ---------


# 2.OR GATE

# SYMBOL:


![image](https://github.com/user-attachments/assets/fd0fd89d-c013-41de-9802-c5674e83aee4)

A curved-shaped gate with two inputs and one output.

# OR GATE IC

![image](https://github.com/user-attachments/assets/e4a702a7-a101-43b8-8801-1c53a4e272f5)


# Function:
The OR gate outputs 1 (true) if at least one input is 1.

 *It outputs 0 only when both inputs are 0.

 # Truth Table:

| Input A | Input B | Output (A + B) |
|---------|---------|----------------|
|    0    |    0    |       0        |
|    0    |    1    |       1        |
|    1    |    0    |       1        |
|    1    |    1    |       1        |

# Logic Expression:
Output = A + B

- The OR gate outputs `1` if **at least one input is 1**.

--------------------------

# 3.NOT GATE

# Symbol:

![image](https://github.com/user-attachments/assets/11c5c4c7-a58d-4198-9339-0568330a39d7)


The NOT gate symbol represents a digital logic inverter, and it is visually distinct from other logic gates. It typically consists of:

 - A triangle pointing to the right

 - A small circle (called a "bubble") at the output, which indicates inversion

# NOT GATE IC

![image](https://github.com/user-attachments/assets/1c4510a3-9296-4f81-8e98-936fe8e6d9b3)


# Function:
The output Y is the negation of the input A, respresented as, Y = Ā Returns 1, if the input is 0. Returns 0, if the input is 1.


# Truth Table:

| Input A | Output (¬A or A̅) |
|---------|-------------------|
|    0    |         1         |
|    1    |         0         |

# Logic Expression:
Output = A̅ or ¬A

- The NOT gate **inverts** the input:
  - If input is `0`, output is `1`
  - If input is `1`, output is `0`
 
  - ---------

# 4.NAND GATE

# Symbol:

![image](https://github.com/user-attachments/assets/36e984b1-5ce3-41dd-8c14-e88d41a6bbd3)

# NAND GATE IC

![image](https://github.com/user-attachments/assets/5eb4bce8-3dd5-43e2-a4d9-29fd66eb375c)



# Function:
A NAND (Not AND) gate gives an output of 0 only when both inputs are 1.

- It is the inverse of the AND gate.

 
# Truth Table:

| Input A | Input B | Output (¬(A · B)) |
|---------|---------|-------------------|
|    0    |    0    |         1         |
|    0    |    1    |         1         |
|    1    |    0    |         1         |
|    1    |    1    |         0         |

# Logic Expression:
Output = ¬(A · B)** or **(A · B)̅**

- The NAND gate outputs `0` **only when both inputs are 1**.
- It is the inverse of the

# 5.NOR GATE
# Symbol :


![image](https://github.com/user-attachments/assets/b2b4d83d-6829-4038-a0ea-257c468c63a3)

# NOR GATE IC

![image](https://github.com/user-attachments/assets/8d964cce-7978-42e5-b4a4-ef121c473178)


# Function :
A NOR (Not OR) gate gives an output of 1 only when both inputs are 0.

- It is the inverse of the OR gate.

# Truth Table:

| Input A | Input B | Output (¬(A + B)) |
|---------|---------|-------------------|
|    0    |    0    |         1         |
|    0    |    1    |         0         |
|    1    |    0    |         0         |
|    1    |    1    |         0         |

# Logic Expression:
Output = ¬(A + B)** or **(A + B)̅**

- The NOR gate outputs `1` **only when both inputs are 0**.
- It is the inverse of the OR gate.


# 6.XOR GATE
# Symbol :


![image](https://github.com/user-attachments/assets/22181ba3-da25-4cbf-9f1e-6d48b90333b1)

# XOR GATE IC

![image](https://github.com/user-attachments/assets/a9279cdd-fc5b-4be6-bc3c-addb651009da)



# Function :

The XOR (Exclusive OR) gate gives an output of 1 only when the inputs are different.

- Boolean Expression : Y = A ⊕ B = A̅·B + A·B̅


# Truth Table:

| Input A | Input B | Output (A ⊕ B) |
|---------|---------|----------------|
|    0    |    0    |       0        |
|    0    |    1    |       1        |
|    1    |    0    |       1        |
|    1    |    1    |       0        |

# Logic Expression:
Output = A ⊕ B**

- The XOR gate outputs `1` **only when the inputs are different**.


# 7.XNOR GATE :
# Symbol :

![image](https://github.com/user-attachments/assets/cc454957-c040-4244-ac74-eb705f4e0ff5)

# XNOR GATE IC

![image](https://github.com/user-attachments/assets/7525d41a-e8ce-4bb1-a067-da51bf29a261)



# Function :
The XNOR (Exclusive NOR) gate gives an output of 1 only when the inputs are the same.

- Boolean Expression : Y = (A ⊕ B)̅ = A·B + A̅·B̅

# Truth Table:

| Input A | Input B | Output (A ⊙ B) |
|---------|---------|----------------|
|    0    |    0    |       1        |
|    0    |    1    |       0        |
|    1    |    0    |       0        |
|    1    |    1    |       1        |

# Logic Expression:
Output = A ⊙ B** (also written as \(\overline{A \oplus B}\))

- The XNOR gate outputs `1` **only when the inputs are the same**.

------


# Integrated Circuits

An IC (Integrated Circuit) is a compact, miniaturized electronic circuit built into a small chip of semiconductor material, usually silicon. It can contain millions of transistors, resistors, capacitors, and other components — all embedded together to perform specific functions.

# Types of Logic Gates and Their IC Numbers

- Logic gates are the basic building blocks of digital circuits. Each gate performs a specific logic function and is available in the form of an Integrated Circuit (IC).



# Types of Logic Gates with IC Numbers, Pin Count & Description

| Logic Gate | IC Number | No. of Gates | Total Pins | Description |
|------------|-----------|--------------|------------|-------------|
| **AND**    | 7408      | 4 AND gates  | 14 pins    | Quad 2-input AND gate |
| **OR**     | 7432      | 4 OR gates   | 14 pins    | Quad 2-input OR gate |
| **NOT**    | 7404      | 6 NOT gates  | 14 pins    | Hex inverter (NOT gates) |
| **NAND**   | 7400      | 4 NAND gates | 14 pins    | Quad 2-input NAND gate |
| **NOR**    | 7402      | 4 NOR gates  | 14 pins    | Quad 2-input NOR gate |
| **XOR**    | 7486      | 4 XOR gates  | 14 pins    | Quad 2-input XOR gate |
| **XNOR**   | 74266     | 4 XNOR gates | 14 pins    | Quad 2-input XNOR gate with open collector outputs |


# General Pin Description for 14-Pin Logic Gate ICs:

| Pin Number | Function               |
|------------|------------------------|
| 1–13       | Input/Output for gates |
| 7          | Ground (GND)           |
| 14         | Supply Voltage (Vcc)   |

 **Note**: Pin configuration varies slightly between ICs, but **Pin 7 (GND)** and **Pin 14 (Vcc)** are almost always the same in standard 14-pin DIP logic ICs.

---


# 1.IC 7408 – Quad 2-Input AND Gate


![image](https://github.com/user-attachments/assets/ed0ed833-5f75-4234-8cda-cc4699b29a34)


![Screenshot 2025-05-22 132514](https://github.com/user-attachments/assets/876670f0-ffbb-4ed9-a70e-f32735b80657)



The IC 7408 has **4 independent AND gates**, each with **2 inputs** and **1 output**. Below is the pin-by-pin description:

| Pin No | Pin Name | Description                             |
|--------|----------|-----------------------------------------|
| 1      | A1       | Input A of Gate 1                       |
| 2      | B1       | Input B of Gate 1                       |
| 3      | Y1       | Output of Gate 1 (A1 · B1)              |
| 4      | A2       | Input A of Gate 2                       |
| 5      | B2       | Input B of Gate 2                       |
| 6      | Y2       | Output of Gate 2 (A2 · B2)              |
| 7      | GND      | Ground (0V)                             |
| 8      | Y3       | Output of Gate 3 (A3 · B3)              |
| 9      | A3       | Input A of Gate 3                       |
| 10     | B3       | Input B of Gate 3                       |
| 11     | Y4       | Output of Gate 4 (A4 · B4)              |
| 12     | A4       | Input A of Gate 4                       |
| 13     | B4       | Input B of Gate 4                       |
| 14     | Vcc      | Supply Voltage (+5V for TTL logic)      |

---

- **Pins 1–6** → Gate 1 & Gate 2
- **Pins 8–13** → Gate 3 & Gate 4
- **Pin 7** → Ground  
- **Pin 14** → Power Supply

- Consists of four independent 2-input AND gates in a single 14-pin DIP package.

- Each gate outputs HIGH only when both inputs are HIGH.

- Designed to operate with standard TTL voltage levels, typically 5V.

- Commonly used in digital logic systems for control, decision-making, and signal validation.


---


# 2.IC 7432 – Quad 2-Input OR Gate



![image](https://github.com/user-attachments/assets/7ef3fdec-fbe4-4d61-ad2e-118e1b3dde40)


![Screenshot 2025-05-22 132905](https://github.com/user-attachments/assets/eee06759-2123-4044-ac00-41cd39070b6f)



The IC **7432** consists of **four independent 2-input OR gates** in a 14-pin Dual In-Line Package (DIP). Each gate performs a logical OR operation.

# Logic Expression:
**Y = A + B**


| Pin No | Pin Name | Description                             |
|--------|----------|-----------------------------------------|
| 1      | A1       | Input A of Gate 1                       |
| 2      | B1       | Input B of Gate 1                       |
| 3      | Y1       | Output of Gate 1 (A1 + B1)              |
| 4      | A2       | Input A of Gate 2                       |
| 5      | B2       | Input B of Gate 2                       |
| 6      | Y2       | Output of Gate 2 (A2 + B2)              |
| 7      | GND      | Ground (0V)                             |
| 8      | Y3       | Output of Gate 3 (A3 + B3)              |
| 9      | A3       | Input A of Gate 3                       |
| 10     | B3       | Input B of Gate 3                       |
| 11     | Y4       | Output of Gate 4 (A4 + B4)              |
| 12     | A4       | Input A of Gate 4                       |
| 13     | B4       | Input B of Gate 4                       |
| 14     | Vcc      | Supply Voltage (+5V for TTL)            |


 Internal Gate Mapping:

| Gate | Inputs | Output | Pins Used           |
|------|--------|--------|---------------------|
| 1    | A1, B1 | Y1     | Pins 1, 2, 3        |
| 2    | A2, B2 | Y2     | Pins 4, 5, 6        |
| 3    | A3, B3 | Y3     | Pins 9, 10, 8       |
| 4    | A4, B4 | Y4     | Pins 12, 13, 11     |

 Power Supply:
- **Pin 14** → Vcc (+5V)
- **Pin 7**  → GND

- Contains four independent 2-input OR gates in a single 14-pin DIP package.

- Each gate performs the logical OR operation: Output is HIGH if any input is HIGH.

- Operates typically at 5V supply voltage with TTL logic compatibility.

- Widely used in digital circuits for combining multiple logic signals or enabling control logic.


- 
--------------

# 3.IC 7404 – Hex Inverter (NOT Gate)

![image](https://github.com/user-attachments/assets/e84ef774-e2cc-4efa-a19a-45cfacb87de5)

![Screenshot 2025-05-22 133415](https://github.com/user-attachments/assets/8990fc98-6935-443b-919f-0500b569400f)



The **IC 7404** contains **six independent NOT gates (inverters)**. Each inverter accepts a logic-level input and outputs the opposite logic level. Packaged in a **14-pin DIP**.


- **Logic Expression:** `Y = ¬A` or `Y = A̅`



| Pin No | Pin Name | Description                          |
|--------|----------|--------------------------------------|
| 1      | A1       | Input of Inverter 1                  |
| 2      | Y1       | Output of Inverter 1 (A1̅)           |
| 3      | A2       | Input of Inverter 2                  |
| 4      | Y2       | Output of Inverter 2 (A2̅)           |
| 5      | A3       | Input of Inverter 3                  |
| 6      | Y3       | Output of Inverter 3 (A3̅)           |
| 7      | GND      | Ground (0V)                          |
| 8      | Y4       | Output of Inverter 4 (A4̅)           |
| 9      | A4       | Input of Inverter 4                  |
| 10     | Y5       | Output of Inverter 5 (A5̅)           |
| 11     | A5       | Input of Inverter 5                  |
| 12     | Y6       | Output of Inverter 6 (A6̅)           |
| 13     | A6       | Input of Inverter 6                  |
| 14     | Vcc      | Power Supply (+5V for TTL logic)    |


# Inverter Mapping:

| Inverter | Input | Output | Pins Used     |
|----------|--------|--------|---------------|
| 1        | A1     | Y1     | 1 → 2         |
| 2        | A2     | Y2     | 3 → 4         |
| 3        | A3     | Y3     | 5 → 6         |
| 4        | A4     | Y4     | 9 → 8         |
| 5        | A5     | Y5     | 11 → 10       |
| 6        | A6     | Y6     | 13 → 12       |

# Power Supply:
- **Pin 14** → Vcc (+5V)
- **Pin 7**  → GND (0V)

- Contains six independent NOT gates (inverters) in a single 14-pin DIP package.

- Each gate inverts the input logic level: Output = NOT(Input).

- Operates with a wide supply voltage range: typically 4.75V to 5.25V.

- used in digital logic circuits for signal inversion, waveform shaping, and logic level shifting

# Applications:
- Signal inversion
- Buffering and level shifting
- Oscillators and waveform generators

- ----------


# 4.IC 7400 – Quad 2-Input NAND Gate

![image](https://github.com/user-attachments/assets/647c6d40-c4ea-4672-99ba-66ef014f2e96)

![Screenshot 2025-05-22 133600](https://github.com/user-attachments/assets/e4a768d5-bb4f-43e9-a4a2-2bac2661c520)



> Each gate performs the logic NAND operation:  
> **Y = ¬(A · B)**


| Pin No | Pin Name | Description                          |
|--------|----------|--------------------------------------|
| 1      | A1       | Input A of Gate 1                    |
| 2      | B1       | Input B of Gate 1                    |
| 3      | Y1       | Output of Gate 1 (A1 NAND B1)        |
| 4      | A2       | Input A of Gate 2                    |
| 5      | B2       | Input B of Gate 2                    |
| 6      | Y2       | Output of Gate 2 (A2 NAND B2)        |
| 7      | GND      | Ground (0V)                          |
| 8      | Y3       | Output of Gate 3 (A3 NAND B3)        |
| 9      | B3       | Input B of Gate 3                    |
| 10     | A3       | Input A of Gate 3                    |
| 11     | Y4       | Output of Gate 4 (A4 NAND B4)        |
| 12     | B4       | Input B of Gate 4                    |
| 13     | A4       | Input A of Gate 4                    |
| 14     | Vcc      | Power Supply (+5V for TTL)           |


# Power Pins:
- **Pin 14** – Vcc (+5V)
- **Pin 7**  – GND (0V)



-IC 7400 consists of four independent 2-input NAND gates in a 14-pin DIP package.

-Each gate performs the logic operation: Y = ¬(A · B) (NAND function).

-Operates on +5V DC supply with pin 14 as Vcc and pin 7 as GND.

-Widely used in digital logic circuits, such as timers, latches, and control systems.


# Applications:
- Digital logic circuits
- Signal blocking
- Flip-flop construction

------


# 5.IC 7402 – Quad 2-Input NOR Gate


![image](https://github.com/user-attachments/assets/dc9d0145-3454-4e7e-8aaf-b86ddae5c897)

![Screenshot 2025-05-22 133209](https://github.com/user-attachments/assets/7712b10c-10a1-428d-91cc-ef71e4222e72)




The **IC 7402** contains **four independent 2-input NOR gates**. Each gate performs the logical NOR operation:  
**Y = ¬(A + B)**



| Pin No | Pin Name | Description                          |
|--------|----------|--------------------------------------|
| 1      | A1       | Input A of Gate 1                    |
| 2      | B1       | Input B of Gate 1                    |
| 3      | Y1       | Output of Gate 1 (A1 NOR B1)         |
| 4      | A2       | Input A of Gate 2                    |
| 5      | B2       | Input B of Gate 2                    |
| 6      | Y2       | Output of Gate 2 (A2 NOR B2)         |
| 7      | GND      | Ground (0V)                          |
| 8      | Y3       | Output of Gate 3 (A3 NOR B3)         |
| 9      | B3       | Input B of Gate 3                    |
| 10     | A3       | Input A of Gate 3                    |
| 11     | Y4       | Output of Gate 4 (A4 NOR B4)         |
| 12     | B4       | Input B of Gate 4                    |
| 13     | A4       | Input A of Gate 4                    |
| 14     | Vcc      | Power Supply (+5V for TTL)           |

- Contains four independent 2-input NOR gates in a single 14-pin package.

- Each gate performs the logical NOR operation, outputting HIGH only when both inputs are LOW.

- Widely used in digital logic circuits for implementing NOR logic functions.

- Operates typically at 5V supply voltage with standardized TTL logic levels.


---------


# 6.IC 7486 – Quad 2-Input XOR Gate

![image](https://github.com/user-attachments/assets/e41ad834-44a2-404f-ab73-9b47b577d948)

![image](https://github.com/user-attachments/assets/e9cff2dc-8b95-4d0f-99ad-c39f58d462f3)




| Pin Number | Pin Name | Description                  |
|------------|-----------|-----------------------------|
| 1          | 1A        | Input 1 of Gate 1           |
| 2          | 1B        | Input 2 of Gate 1           |
| 3          | 1Y        | Output of Gate 1            |
| 4          | 2A        | Input 1 of Gate 2           |
| 5          | 2B        | Input 2 of Gate 2           |
| 6          | 2Y        | Output of Gate 2            |
| 7          | GND       | Ground (0V)                 |
| 8          | 3Y        | Output of Gate 3            |
| 9          | 3A        | Input 1 of Gate 3           |
| 10         | 3B        | Input 2 of Gate 3           |
| 11         | 4Y        | Output of Gate 4            |
| 12         | 4A        | Input 1 of Gate 4           |
| 13         | 4B        | Input 2 of Gate 4           |
| 14         | Vcc       | Positive Power Supply (+5V) |


- Contains four independent 2-input XOR gates in a single 14-pin package.

- Each gate outputs HIGH only when the number of HIGH inputs is odd (i.e., inputs are different).

- Commonly used for parity checking, arithmetic circuits, and digital comparison.

- Operates typically at 5V supply voltage with TTL-compatible logic levels.

-------------

# 7.IC 74266 – Quad 2-Input XNOR Gate

![image](https://github.com/user-attachments/assets/215b2a6c-f8fa-491d-9f5b-91f3a5258f59)

![image](https://github.com/user-attachments/assets/1c150e22-4891-4d7a-918a-df9af5b03d31)




| Pin Number | Pin Name | Description                  |
|------------|-----------|-----------------------------|
| 1          | 1A        | Input 1 of Gate 1           |
| 2          | 1B        | Input 2 of Gate 1           |
| 3          | 1Y        | Output of Gate 1            |
| 4          | 2A        | Input 1 of Gate 2           |
| 5          | 2B        | Input 2 of Gate 2           |
| 6          | 2Y        | Output of Gate 2            |
| 7          | GND       | Ground (0V)                 |
| 8          | 3Y        | Output of Gate 3            |
| 9          | 3A        | Input 1 of Gate 3           |
| 10         | 3B        | Input 2 of Gate 3           |
| 11         | 4Y        | Output of Gate 4            |
| 12         | 4A        | Input 1 of Gate 4           |
| 13         | 4B        | Input 2 of Gate 4           |
| 14         | Vcc       | Positive Power Supply (+5V) |


- Contains four independent 2-input XNOR gates in a 14-pin DIP package.
- Each gate outputs HIGH when both inputs are the same (both HIGH or both LOW).
- Used in equality detection, digital comparators, and parity circuits.
- Operates at 5V supply voltage with TTL-compatible logic levels.
- 




# TINKER CARD LOGIC GATES
# 1.AND GATE

![image](https://github.com/user-attachments/assets/da9170d8-2fc2-467c-9ca0-b9a9da11b05d)


https://www.tinkercad.com/things/fOfobxMCEBW-and-gate?sharecode=j_8n2KSpD3f5LKcmzVvaJSIw6A7fhyE-jNRnOHJxFiU

---------------

# 2.OR GATE

![image](https://github.com/user-attachments/assets/10ac8c08-0811-42b0-a41d-490cc82e747c)


https://www.tinkercad.com/things/lKZPyXAEMNc-or-gate?sharecode=jXxd-SpDmHHTyQdyUw5pfSnHZphy83RyIUHRacghbL4

------------------

# 3.NOT GATE


![image](https://github.com/user-attachments/assets/929632b7-d039-436e-841f-94e8d3956b02)


https://www.tinkercad.com/things/kUF9XcC3WpI-nor-gate?sharecode=Z_KnyAls3l5EHdBE3Pxy_3yfP6z07jgeFZfannSjekw

-------------

# 4.NOT GATE


![image](https://github.com/user-attachments/assets/22034bbc-c72a-4fa7-946b-444948094d4c)


https://www.tinkercad.com/things/kjzNcYUMK6G-not-gate?sharecode=Vb2GaxG-duD78K0ltgJJCpkjuwf-6Ok3Lm5GJyQdh3M

-----------------

# 5.NAND GATE


![image](https://github.com/user-attachments/assets/c89e046a-52be-4e93-ae92-cac6461062ad)


https://www.tinkercad.com/things/2XV8GgJ122T-nand-gate?sharecode=o5mKUq-mFiG7vqqcQ8XPHlrK9F9bOICSzB8Q4UYYgjA

------------------------------

# 6.XOR GATE


![image](https://github.com/user-attachments/assets/01e0fd5d-6e7c-4a26-99dc-545c6acc6cdc)


https://www.tinkercad.com/things/fEuDCj6Gk6n-xor-gate?sharecode=JM9vHWwbif3Lj7GUjIkPhpUnfeIfCduufKzjAw9Ub5M

----------------

# 7.XNOR GATE


![image](https://github.com/user-attachments/assets/e1358f44-5082-4008-b12d-ed6b93ff72db)


https://www.tinkercad.com/things/fq6O6knnfkm-xnor-gate?sharecode=iquvjY0KZAv2Xnp_AIUeW8Bal-Pdzds6_HhS5X_aW7I

------------------
# IMPLEMENTATION OF GATES

# 1.OR 0PERATION USING NAND IC

![image](https://github.com/user-attachments/assets/a802f3e2-c5e4-4c12-9ff2-a3cfa0da22d8)


https://www.tinkercad.com/things/aCpoxpxbirs-or-gate-using-nand?sharecode=ZOp1-zOUNptig09f4d1teMcVSrW1eIOsRRoHr1fFo4E

-----------------
# 2.NOT OPERATION USING NAND IC


![image](https://github.com/user-attachments/assets/8f4f86c8-a94c-439b-9fb5-9d7746b8d7b5)


https://www.tinkercad.com/things/5w8bod8q7ur-not-using-nand?sharecode=D-DyCMSv-YGMq35g7hoicR_AEPAQf8I7sO8UzXPx-JM

-------------

# 3.AND OPERATION USING NOR IC


![image](https://github.com/user-attachments/assets/4a1e84af-57e6-470c-b6f2-d69b08dba5ed)


https://www.tinkercad.com/things/kraNCAj0oeY-and-gate-using-nor?sharecode=K05LbFGCjSuXIB2nc3DUGTdqU6wGF_pnOMgy6-TrdCU

-----------------
# IMPLEMENTATAION OF HALF ADDER

# HALF ADDER

# Pin Daigram

![image](https://github.com/user-attachments/assets/214baa9c-3bc1-474c-b154-5bacbd642091)


# Truth Table

![image](https://github.com/user-attachments/assets/a0b77db8-7df0-462d-92f6-ff94e49f8665)


![image](https://github.com/user-attachments/assets/e1d013ed-be95-48c2-87b9-4be842dc7632)

https://www.tinkercad.com/things/79egzPqBmSh-half-adder?sharecode=EXGfGBb40zthoJItsJMCrU7bsacctC5z47_1Cod10WM 

-------------

# IMPLEMENTATION OF FULL ADDER

# FULL ADDER

# Pin Daigram

# Truth Table

![image](https://github.com/user-attachments/assets/d64f68ac-4278-4f27-b687-1e637b18b15d)




![image](https://github.com/user-attachments/assets/b4203910-0a80-4cfb-b272-b651fedab863)


https://www.tinkercad.com/things/g4lCLiKjXc9-full-adder?sharecode=TuKP4uzOq6iB7cw8YDw9qI4viTGbj3Jr4UGfm4jWwVo




















 
