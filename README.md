# 
# Table of Content

- [WHAT IS DIGITAL ELECTRONICS](#WHAT-IS-DIGITAL-ELECTRONICS)
- [APPLICATIONS OF DIGITAL ELECTRONICS](#APPLICATIONS-OF-DIGITAL-ELECTRONICS)
- [DIGITAL VS ANALOG SIGNALS](#DIGITAL-VS-ANALOG-SIGNALS)
- [LOGIC LEVELS](#LOGIC-LEVELS)
- [NUMBER SYSTEM](#NUMBER-SYSTEM)
- [CONVERSION BETWEEN NUMBER SYSTEM](#CONVERSION-BETWEEN-NUMBER-SYSTEM)
- [BASIC LOGIC GATES](#BASIC-LOGIC-GATES)
- [INTEGRATED CIRCUITS](#INTEGRATED-CIRCUITS)
- [IMPLEMENTATION OF GATES](#IMPLEMENTATION-OF-GATES)
- [IMPLEMENTATAION OF HALF ADDER](#IMPLEMENTATAION-OF-HALF-ADDER)
- [IMPLEMENTATION OF FULL ADDER](#IMPLEMENTATION-OF-FULL-ADDER)
- [IMPLEMENTATION OF 2X1 MULTIPLEXER](#IMPLEMENTATION-OF-2X1-MULTIPLEXER)
- [IMPLEMENTATION OF 4X1 MULTIPLEXER](#IMPLEMENTATION-OF-4X1-MULTIPLEXER)





# WHAT IS DIGITAL ELECTRONICS

DEFINATION:
Definition	Digital electronics is a branch of electronics that deals with digital signals — signals that have only two discrete levels: HIGH (1) and LOW (0). It is the foundation of computers, digital communication, and modern electronic devices.

# APPLICATIONS OF DIGITAL ELECTRONICS
Applications	Used in:
• Computers, Laptops
• Digital Watches
• Mobile Phones
• Calculators
• Robotics
• Digital Control Systems
Applications	Found in almost all modern electronics: computers, smartphones, digital cameras, smart TVs, automotive systems, robotics, automation, and more.

# DIGITAL VS ANALOG SIGNALS

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
# Logic Levels Table

| Logic Level | Digital Value | Voltage Range (Typical for TTL) | Voltage Range (Typical for CMOS) |
|-------------|---------------|-------------------------------|----------------------------------|
| LOW         | 0             | 0V to 0.8V                    | 0V to 1.5V                       |
| HIGH        | 1             | 2V to 5V                      | 3.5V to 5V (or 3.3V, depending)  |
| Undefined   | -             | 0.8V to 2V                    | 1.5V to 3.5V                     |


- LOGIC LEVELS

Logic 0 (LOW)

Logic 1 (HIGH)

- Digital circuits operate using only these two levels to interpret data, control operations, and perform computations.

# 1.Logic LOW (0)

- Logic 0, also called LOW, represents the binary value 0.



# 2.Logic HIGH (1)

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

# CONVERSION BETWEEN NUMBER SYSTEM

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

# AND GATE IC:

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

- A curved-shaped gate with two inputs and one output.

# OR GATE IC:

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

# NOT GATE IC:

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

# NAND GATE IC:

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

# NOR GATE IC:

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

# XOR GATE IC:

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

# XNOR GATE IC:

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


# INTEGRATED CIRCUITS

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



# 1.IC 7408 – Quad 2-Input AND Gate

# AND IC:


![image](https://github.com/user-attachments/assets/ed0ed833-5f75-4234-8cda-cc4699b29a34)

# CIRCUIT:


![image](https://github.com/user-attachments/assets/da9170d8-2fc2-467c-9ca0-b9a9da11b05d)

- TINKERCARD LINK:


🔗 [Open AND Gate on Tinkercad](https://www.tinkercad.com/things/fOfobxMCEBW-and-gate?sharecode=j_8n2KSpD3f5LKcmzVvaJSIw6A7fhyE-jNRnOHJxFiU)

# Applications
- Logic circuits where two conditions must be true.
- Digital control systems.
- Signal enable logic.
- Arithmetic logic units (ALUs).
- Microcontroller decision-making circuits.
- Security systems and alarms.



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


# OR IC:


![image](https://github.com/user-attachments/assets/7ef3fdec-fbe4-4d61-ad2e-118e1b3dde40)


# CIRCUIT:


![image](https://github.com/user-attachments/assets/10ac8c08-0811-42b0-a41d-490cc82e747c)


- TINKERCARD LINK:


🔗 [Open OR Gate on Tinkercad](https://www.tinkercad.com/things/lKZPyXAEMNc-or-gate?sharecode=jXxd-SpDmHHTyQdyUw5pfSnHZphy83RyIUHRacghbL4)



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

# Applications 

- Used in logic decision circuits to output HIGH if any input is HIGH  
- Applied in alarm systems (e.g., fire or security alarms)  
- Enables signal routing and multiplexing in digital circuits  
- Used in start/stop control and industrial automation logic  
- Combines multiple interrupt signals in microprocessors  
- Detects presence of any input signal in monitoring systems  
- Implements digital switching with multiple input triggers  
- Used in Arithmetic Logic Units (ALUs) for logic operations  
- Controls traffic light systems based on multiple conditions  
- Ideal for designing custom logic functions in digital systems  

 
--------------

# 3.IC 7404 – Hex Inverter (NOT Gate) 

# NOT IC:

![image](https://github.com/user-attachments/assets/e84ef774-e2cc-4efa-a19a-45cfacb87de5)

# CIRCUIT:


![image](https://github.com/user-attachments/assets/22034bbc-c72a-4fa7-946b-444948094d4c)


- TINKERCARD LINK:

🔗 [Open NOT Gate on Tinkercad](https://www.tinkercad.com/things/kjzNcYUMK6G-not-gate?sharecode=Vb2GaxG-duD78K0ltgJJCpkjuwf-6Ok3Lm5GJyQdh3M)



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

# NAND IC:

![image](https://github.com/user-attachments/assets/647c6d40-c4ea-4672-99ba-66ef014f2e96)

# CIRCUIT:

![image](https://github.com/user-attachments/assets/c89e046a-52be-4e93-ae92-cac6461062ad)


- TINKERCARD LINK:


🔗 [Open NAND Gate on Tinkercad](https://www.tinkercad.com/things/2XV8GgJ122T-nand-gate?sharecode=o5mKUq-mFiG7vqqcQ8XPHlrK9F9bOICSzB8Q4UYYgjA)



-  Each gate performs the logic NAND operation:  
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

# NOR IC:


![image](https://github.com/user-attachments/assets/dc9d0145-3454-4e7e-8aaf-b86ddae5c897)

# CIRCUIT:


![image](https://github.com/user-attachments/assets/929632b7-d039-436e-841f-94e8d3956b02)

- TINKERCARD LINK:

🔗 [Open NOR Gate on Tinkercad](https://www.tinkercad.com/things/kUF9XcC3WpI-nor-gate?sharecode=Z_KnyAls3l5EHdBE3Pxy_3yfP6z07jgeFZfannSjekw)




- The **IC 7402** contains **four independent 2-input NOR gates**. Each gate performs the logical NOR operation:  
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

## Applications

- Basic NOR logic circuits  
- Universal logic gate design  
- Digital control systems  
- Alarm and signal detection  
- Memory decoding  
- Timers and counters  
- Combinational logic  
- Inverter logic (tie inputs)  
- Computer logic systems  
- Pulse and waveform shaping  



---------


# 6.IC 7486 – Quad 2-Input XOR Gate

# XOR IC:

![image](https://github.com/user-attachments/assets/e41ad834-44a2-404f-ab73-9b47b577d948)

# CIRCUIT:

![image](https://github.com/user-attachments/assets/e9cff2dc-8b95-4d0f-99ad-c39f58d462f3)


- TINKERCARD LINK:

🔗 [Open XOR Gate on Tinkercad](https://www.tinkercad.com/things/fEuDCj6Gk6n-xor-gate?sharecode=JM9vHWwbif3Lj7GUjIkPhpUnfeIfCduufKzjAw9Ub5M)





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

# Applications 

- Parity generation/checking  
- Binary adders/subtractors  
- Digital comparators  
- ALUs and logic circuits  
- Error detection in data transmission  
- Signal modulation  
- Bitwise comparison  
- Logic switching  
- Phase detection  
- Basic cryptographic logic  


-------------

# 7.IC 74266 – Quad 2-Input XNOR Gate

# XNOR IC:

![image](https://github.com/user-attachments/assets/215b2a6c-f8fa-491d-9f5b-91f3a5258f59)


# CIRCUIT:

![image](https://github.com/user-attachments/assets/1c150e22-4891-4d7a-918a-df9af5b03d31)

- TINKERCARD LINK:

🔗 [Open XNOR Gate on Tinkercad](https://www.tinkercad.com/things/fq6O6knnfkm-xnor-gate?sharecode=iquvjY0KZAv2Xnp_AIUeW8Bal-Pdzds6_HhS5X_aW7I)





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

# Applications 

- Equality comparison circuits  
- Logic comparators  
- Digital error detection  
- Parity checking  
- Signal matching logic  
- Controlled inverters (with strobe)  
- Phase detection circuits  
- Arithmetic logic designs  
- Encoder/decoder logic  
- Identity logic circuits  


------------------
# IMPLEMENTATION OF GATES

# 1.OR 0PERATION USING NAND IC

![image](https://github.com/user-attachments/assets/a802f3e2-c5e4-4c12-9ff2-a3cfa0da22d8)

- TINKERCARD LINK:

🔗 [Open NOT Gate (using NAND gate) on Tinkercad](https://www.tinkercad.com/things/5w8bod8q7ur-not-using-nand?sharecode=D-DyCMSv-YGMq35g7hoicR_AEPAQf8I7sO8UzXPx-JM)


-----------------
# 2.NOT OPERATION USING NAND IC


![image](https://github.com/user-attachments/assets/8f4f86c8-a94c-439b-9fb5-9d7746b8d7b5)

- TINKERCARD LINK:

🔗 [Open NOT Gate (using NAND gate) on Tinkercad](https://www.tinkercad.com/things/5w8bod8q7ur-not-using-nand?sharecode=D-DyCMSv-YGMq35g7hoicR_AEPAQf8I7sO8UzXPx-JM)


-------------

# 3.AND OPERATION USING NOR IC


![image](https://github.com/user-attachments/assets/4a1e84af-57e6-470c-b6f2-d69b08dba5ed)

- TINKERCARD LINK:

🔗 [Open AND Gate (using NOR gates) on Tinkercad](https://www.tinkercad.com/things/kraNCAj0oeY-and-gate-using-nor?sharecode=K05LbFGCjSuXIB2nc3DUGTdqU6wGF_pnOMgy6-TrdCU)



# 4.AND OPERATION USINF NAND GATE 7400IC

![image](https://github.com/user-attachments/assets/aeb90e9c-c0d1-4a98-9c4c-5d3c5927e6c0)

- TINKERCARD LINK:

🔗 [Open AND Gate (using NAND gates) on Tinkercad](https://www.tinkercad.com/things/jblMKUMEH3Z-and-using-nand?sharecode=fz_ZTUGbdwoSjJ146oipzZ_LefaPlFxyRZ3M0XJHxdg)


# 5.OR OPERATION USING NOR GATE 7402

![image](https://github.com/user-attachments/assets/f3e48ecb-946a-4a31-ba0f-9e76db056de0)

- TINKERCARD LINK:

🔗 [Open OR Gate (using NOR gates) on Tinkercad](https://www.tinkercad.com/things/ffe7yMd2Aw0-or-using-nor-gate?sharecode=NSY0rSpOb4RoGHuoJT7nnqgRu4DArxJWNijnrNV1Kcw)


# 6.NOT OPERATION USING NOR GATE 7402

![image](https://github.com/user-attachments/assets/14cc26b6-ffd4-4e03-a616-d4e10716ed36)


- TINKERCARD LINK:


🔗 [Open NOT Gate (using NOR gate) on Tinkercad](https://www.tinkercad.com/things/iybnVqVjyDm-not-using-nor-gate?sharecode=P9JA-w9YDAR5kGd5mgF3HLFWbfoJr1Rt089Tm0iB9eE)



-----------------
# IMPLEMENTATAION OF HALF ADDER

# HALF ADDER

# Pin Daigram

![image](https://github.com/user-attachments/assets/214baa9c-3bc1-474c-b154-5bacbd642091)


# Truth Table

![image](https://github.com/user-attachments/assets/a0b77db8-7df0-462d-92f6-ff94e49f8665)



![image](https://github.com/user-attachments/assets/e1d013ed-be95-48c2-87b9-4be842dc7632)

🔗 [Open Half Adder on Tinkercad](https://www.tinkercad.com/things/79egzPqBmSh-half-adder?sharecode=EXGfGBb40zthoJItsJMCrU7bsacctC5z47_1Cod10WM)



# Half Adder using EXOR (7486) and AND (7408) IC – Pin-to-Pin Connection Table

This configuration uses:
- **7486 IC** for the XOR operation (SUM output)
- **7408 IC** for the AND operation (CARRY output)


| S.No | From Pin            | To Pin             | Comment                                        |
|------|---------------------|--------------------|------------------------------------------------|
| 1    | A (Input Switch)    | 7486 Pin 1         | Input A to XOR Gate 1                          |
| 2    | B (Input Switch)    | 7486 Pin 2         | Input B to XOR Gate 1                          |
| 3    | 7486 Pin 3          | SUM Output LED     | Output of XOR Gate 1 = A ⊕ B (SUM)             |
| 4    | A (Input Switch)    | 7408 Pin 1         | Input A to AND Gate 1                          |
| 5    | B (Input Switch)    | 7408 Pin 2         | Input B to AND Gate 1                          |
| 6    | 7408 Pin 3          | CARRY Output LED   | Output of AND Gate 1 = A • B (CARRY)           |
| 7    | 7486 Pin 7          | GND                | Connect XOR IC GND to Ground                   |
| 8    | 7486 Pin 14         | +5V Vcc            | Connect XOR IC Vcc to +5V supply               |
| 9    | 7408 Pin 7          | GND                | Connect AND IC GND to Ground                   |
| 10   | 7408 Pin 14         | +5V Vcc            | Connect AND IC Vcc to +5V supply               |

# Logic Notes

- **SUM** = A ⊕ B → using 7486 XOR gate  
- **CARRY** = A • B → using 7408 AND gate  
- Both ICs have 4 gates each; only 1 gate from each is used here.

-------------

# IMPLEMENTATION OF FULL ADDER

# FULL ADDER

# PIN DAIGRAM

![image](https://github.com/user-attachments/assets/7e61f4ee-77ec-485c-b0b3-2b37458271cf)


# TRUTH TABLE


![image](https://github.com/user-attachments/assets/46e54667-623e-4d4e-8d4d-bb102d049982)

# CIRCUIT:

![image](https://github.com/user-attachments/assets/9a0fa9fa-8536-4037-a9fa-b79ee9a6040d)

- TINKERCARD LINK:

🔗 [Open Full Adder on Tinkercad](https://www.tinkercad.com/things/g4lCLiKjXc9-full-adder?sharecode=TuKP4uzOq6iB7cw8YDw9qI4viTGbj3Jr4UGfm4jWwVo)



# Full Adder using 7486 (XOR), 7408 (AND), and 7432 (OR) ICs – Pin-to-Pin Connection Table

A Full Adder adds three 1-bit binary numbers: A, B, and Cin (Carry In), and outputs:
- **SUM** = A ⊕ B ⊕ Cin
- **CARRY** = (A • B) + (Cin • (A ⊕ B))

# Pin Connections

| S.No | From Pin             | To Pin              | Comment                                           |
|------|----------------------|---------------------|---------------------------------------------------|
| 1    | A (Input Switch)     | 7486 Pin 1          | Input A to XOR Gate 1                             |
| 2    | B (Input Switch)     | 7486 Pin 2          | Input B to XOR Gate 1                             |
| 3    | 7486 Pin 3           | 7486 Pin 4          | A ⊕ B output to input of second XOR gate          |
| 4    | Cin (Input Switch)   | 7486 Pin 5          | Carry In to second XOR gate                       |
| 5    | 7486 Pin 6           | SUM Output LED      | SUM = A ⊕ B ⊕ Cin                                 |
| 6    | A (Input Switch)     | 7408 Pin 1          | Input A to AND Gate 1                             |
| 7    | B (Input Switch)     | 7408 Pin 2          | Input B to AND Gate 1                             |
| 8    | 7408 Pin 3           | 7432 Pin 1          | A • B to OR Gate 1                                |
| 9    | 7486 Pin 3           | 7408 Pin 4          | A ⊕ B output to AND Gate 2                        |
| 10   | Cin (Input Switch)   | 7408 Pin 5          | Cin to AND Gate 2                                 |
| 11   | 7408 Pin 6           | 7432 Pin 2          | Cin • (A ⊕ B) to OR Gate 1                        |
| 12   | 7432 Pin 3           | CARRY Output LED    | Carry = (A • B) + (Cin • (A ⊕ B))                 |
| 13   | 7486 Pin 7           | GND                 | Ground for XOR IC                                 |
| 14   | 7486 Pin 14          | +5V Vcc             | Power supply for XOR IC                           |
| 15   | 7408 Pin 7           | GND                 | Ground for AND IC                                 |
| 16   | 7408 Pin 14          | +5V Vcc             | Power supply for AND IC                           |
| 17   | 7432 Pin 7           | GND                 | Ground for OR IC                                  |
| 18   | 7432 Pin 14          | +5V Vcc             | Power supply for OR IC                            |

# Logic Notes

- **SUM** = A ⊕ B ⊕ Cin → using 2 XOR gates from IC 7486
- **CARRY** = (A • B) + (Cin • (A ⊕ B)) → using 2 AND gates (IC 7408) and 1 OR gate (IC 7432)

Only 2 gates from XOR and AND ICs are used. Remaining gates can be left unconnected or tied off.


---------------

# IMPLEMENTATION OF 2X1 MULTIPLEXER

# Introduction

- A 2X1 Multiplexer (MUX) selects one of two inputs and forwards it to a single output.
 
- Control is based on a single **select line (S)**
  
- This design uses basic gates from standard TTL ICs.


# How a 2X1 MUX Works – Step-by-Step

# It has 3 inputs:

A – Input 1,B – Input 2,S – Select line

It has 1 output:

Y – Output based on selected input

# Logic Operation:

If S = 0, the output Y = A

If S = 1, the output Y = B

- Internally:

- S = 0:

NOT(S) = 1

A is passed through an AND gate (A AND NOT(S))

B is blocked (B AND S = 0)

- S = 1:

NOT(S) = 0

A is blocked

B is passed through (B AND S)

The outputs of both AND gates go into an OR gate, so only the selected input reaches Y.


# Logic Expression
- Output Y = (A AND NOT(S)) OR (B AND S)

# PIN DAIGRAM : 

![image](https://github.com/user-attachments/assets/6ed3bb2b-09f4-4c92-a2f5-c7da4c8d8bda)

# TRUTH TABLE:

![image](https://github.com/user-attachments/assets/baf3ee25-ba8b-45a8-b8da-be753e6ad8f5)

# CIRCUIT:

![image](https://github.com/user-attachments/assets/797841bd-1cd3-411e-8d88-7e1973bbe833) 

- TINKERCARD LINK:

🔗 [Open 2:1 Multiplexer on Tinkercad](https://www.tinkercad.com/things/gmGdlk6Ekrb-21-multiplexer?sharecode=IOVGOv5c3v5PD7PAsjuvPpBAoavy_5nOXjH36SehCMo)



   
# ICs Used:
- **IC 7404** – Hex Inverter (NOT Gate)
- **IC 7408** – Quad 2-Input AND Gate
- **IC 7432** – Quad 2-Input OR Gate


# Multiplexer using 7404 (NOT), 7408 (AND), and 7432 (OR) ICs – Pin-to-Pin Connection Table


| S.No | From Pin         | To Pin         | IC Used | Description                         |
|------|------------------|----------------|---------|-------------------------------------|
| 1    | VCC (+5V)        | Pin 14 (All ICs) | -     | Power Supply                        |
| 2    | GND              | Pin 7 (All ICs)  | -     | Ground                              |
| 3    | Select (S)       | Pin 1 (7404)     | 7404  | Input to NOT gate                   |
| 4    | Pin 2 (7404)     | Pin 1 (7408)     | 7408  | Output of NOT(S) to AND gate 1      |
| 5    | Input A          | Pin 2 (7408)     | 7408  | Input A to AND gate 1               |
| 6    | Input B          | Pin 4 (7408)     | 7408  | Input B to AND gate 2               |
| 7    | Select (S)       | Pin 3 (7408)     | 7408  | S to AND gate 2                     |
| 8    | Pin 3 (7408)     | Pin 1 (7432)     | 7432  | Output of AND1 to OR input1         |
| 9    | Pin 6 (7408)     | Pin 2 (7432)     | 7432  | Output of AND2 to OR input2         |
| 10   | Pin 3 (7432)     | OUTPUT Y         | 7432  | Final Output of MUX                 |


--------------

# IMPLEMENTATION OF 4X1 MULTIPLEXER

# Definition:

A **4x1 Multiplexer (MUX)** is a combinational logic circuit that selects one of **four input data lines (I₀, I₁, I₂, I₃)** and transmits the selected input to a single output line (**Y**) based on the values of **two selection inputs (S₁ and S₀)**.

It functions like a digitally controlled switch, allowing one input line to be passed through based on the control signal


# Summary of IC Usage:

- IC 7411: For 3-input AND gates (one per minterm)

- IC 7404: For inverting selection lines (S0, S1 → S̅0, S̅1)

- IC 7432: For combining the AND outputs (2 OR gates needed)


| **Function**         | **IC Number** | **Description**            | **Number of Gates** |
| -------------------- | ------------- | -------------------------- | ------------------- |
| **3-input AND gate** | **IC 7411**   | Triple 3-input AND gate    | 3 gates             |
| **NOT gate**         | **IC 7404**   | Hex Inverter (6 NOT gates) | 6 gates             |
| **2-input OR gate**  | **IC 7432**   | Quad 2-input OR gate       | 4 gates             |



# PIN DAIGRAM:

![image](https://github.com/user-attachments/assets/2d5bbca6-0900-4f0a-acbc-72970fe3950e)

# IC Implementation:

You can implement a 4x1 multiplexer using:

- IC 74153 – Dual 4-to-1 multiplexer

- Basic gates: AND, OR, NOT (e.g., IC 7408 for AND, IC 7432 for OR, IC 7404 for NOT)



# TRUTH TABLE:

| S₁ | S₀ | Output Y |
|----|----|-----------|
| 0  | 0  | I₀        |
| 0  | 1  | I₁        |
| 1  | 0  | I₂        |
| 1  | 1  | I₃        |

# CIRCUIT:

![image](https://github.com/user-attachments/assets/4f91c5bd-0e60-4e13-8957-0c4472cd5945)

- TINKERCARD LINK:

[Click here to view the circuit on Tinkercad](https://www.tinkercad.com/things/bYPUmelVHe7-4x1-multiplexer?sharecode=rmu7yLv2ocBYOf5FKWxUkhVCvieOy94bcoWxXNHbhO4)



# 4x1 MUX Pin-to-Pin Connection Table (Using IC 7411 - AND, IC 7432 - OR, IC 7404 - NOT)


| S.No | From Pin             | To Pin             | IC Used  | Purpose                          |
|------|----------------------|--------------------|----------|----------------------------------|
| 1    | S0                   | 1A (IC 7404)        | 7404     | Invert S0 to get S̅0             |
| 2    | S1                   | 3A (IC 7404)        | 7404     | Invert S1 to get S̅1             |
| 3    | S̅1, S̅0, I0         | 1A, 1B, 1C (IC 7411)| 7411     | AND gate for I0 path             |
| 4    | S̅1, S0, I1          | 2A, 2B, 2C (IC 7411)| 7411     | AND gate for I1 path             |
| 5    | S1, S̅0, I2          | 3A, 3B, 3C (IC 7411)| 7411     | AND gate for I2 path             |
| 6    | S1, S0, I3           | 4A, 4B, 4C (IC 7411)| 7411     | AND gate for I3 path             |
| 7    | Outputs of all ANDs  | Inputs of OR gates | 7432     | Combine outputs using OR         |
| 8    | Final OR output      | Y (Output)         | 7432     | Output of 4x1 Multiplexer        |



# Applications:

- Data routing in communication systems

- Logic function generation

- Control units in CPUs

- Signal selection in digital systems




























 
