# DIGITAL ELECTRONICS
# DIGITAL ELECTRONICS INTERNSHIP
- [what is digital electronics](#what-is-digital-electronics)
- [Applications of Digital Electronics](#Applications-of-Digital-Electronics)
- [Digital vs Analog signals](#Digital-vs-Analog-signals)
- [LOGIC LEVELS](#LOGIC-LEVELS)
- [NUMBER SYSTEM](#NUMBER-SYSTEM)
- [Conversion between number system](#Conversion-between-number-system)
- [BASIC LOGIC GATES](#BASIC-LOGIC-GATES)
- [ What is an IC](#What-is-an-IC)

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
In digital electronics, a logic level is a specific voltage or range of voltages used to represent binary states:

Logic 0 (LOW)

Logic 1 (HIGH)

Digital circuits operate using only these two levels to interpret data, control operations, and perform computations.

1. Logic LOW (0)
Logic 0, also called LOW, represents the binary value 0.

It typically corresponds to a voltage close to 0 volts.

The exact voltage range depends on the technology used (e.g., TTL, CMOS).

2. Logic HIGH (1)
Logic 1, also called HIGH, represents the binary value 1.

It corresponds to a voltage close to the supply voltage, commonly 3.3V or 5V.

Again, the range may differ depending on the logic family.

⚙️ Logic Level Standards
Different digital logic families (like TTL or CMOS) define specific voltage ranges for logic levels:

✅ TTL (Transistor-Transistor Logic) – typically 5V system:
Logic 0 (LOW): 0V to 0.8V

Logic 1 (HIGH): 2V to 5V

Undefined Zone: 0.8V to 2V (should be avoided)

✅ CMOS (Complementary Metal-Oxide-Semiconductor) – flexible with V<sub>DD</sub>:
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

1. Binary → Decimal
Binary: 1011₂

= (1×2³) + (0×2²) + (1×2¹) + (1×2⁰)

= 8 + 0 + 2 + 1

= 11₁₀

-------------

2. Decimal → Binary

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

3. Binary → Octal
Binary: 110110₂

Group in 3 bits → 110 | 110

110₂ = 6₈

110₂ = 6₈

Result → 66₈

-----------
4. Octal → Binary

 Octal: 725 to Binary

| Octal Digit | Binary (3 bits) |
|-------------|-----------------|
| 7           | 111             |
| 2           | 010             |
| 5           | 101             |

Result →  
Octal 725 = Binary 111010101

----------------

5. Binary → Hexadecimal
Convert Binary: 10111110 to Hexadecimal

| Binary Group | Decimal Equivalent | Hexadecimal Digit |
|--------------|--------------------|-------------------|
| 1011         | 11                 | B                 |
| 1110         | 14                 | E                 |

Result → 
Binary 10111110 = Hexadecimal **BE**

---
 

6. Hexadecimal → Binary
Hexadecimal `3F9` to Binary

| Hex Digit | Binary (4 bits) |
|-----------|-----------------|
| 3         | 0011            |
| F         | 1111            |
| 9         | 1001            |

Result → 
Hexadecimal 3F9 = Binary 001111111001


----------------


7. Decimal → Octal
 Convert Decimal `156` to Octal

| Step | Division        | Quotient | Remainder |
|-------|-----------------|----------|-----------|
| 1     | 156 ÷ 8 = 19    | 19       | 4         |
| 2     | 19 ÷ 8 = 2      | 2        | 3         |
| 3     | 2 ÷ 8 = 0       | 0        | 2         |

Read remainders from bottom to top: 2 3 4

Decimal 156 = Octal 234


------------------


8. Octal → Decimal
Octal: 745₈

= (7×8²) + (4×8¹) + (5×8⁰)

= (7×64) + (4×8) + (5×1)

= 448 + 32 + 5

= 485₁₀

----------------

9. Decimal → Hexadecimal
   
Decimal: 254₁₀

254 ÷ 16 = 15 remainder 14 (E)

15 ÷ 16 = 0 remainder 15 (F)

Read remainders bottom to top → FE₁₆

-------------------

10. Hexadecimal → Decimal
Hex: 2A₁₆

= (2×16¹) + (A×16⁰)

= (2×16) + (10×1)

= 32 + 10

= 42₁₀

-------------------

11. Octal → Hexadecimal
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

12. Hexadecimal → Octal
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

1.AND GATE

# Symbol:

![image](https://github.com/user-attachments/assets/cc423310-cf10-4e14-910a-b006e5131efe)

A curved-shaped gate with two inputs and one output.

# Function:
The AND gate outputs 1 (true) only when both inputs are 1. Otherwise, it outputs 0.

 *A.B=X.
 
 *The value of X will be True when both the inputs will be True.
 
# Truth Table 


| Input A | Input B | Output (A · B) |
|---------|---------|----------------|
|    0    |    0    |       0        |
|    0    |    1    |       0        |
|    1    |    0    |       0        |
|    1    |    1    |       1        |

### Logic Expression:
Output = A · B

- The AND gate outputs `1` only when **both inputs are 1**.

2.  OR GATE

# SYMBOL


![image](https://github.com/user-attachments/assets/fd0fd89d-c013-41de-9802-c5674e83aee4)

A curved-shaped gate with two inputs and one output.

# Function:
The OR gate outputs 1 (true) if at least one input is 1.

 *It outputs 0 only when both inputs are 0.

 # Truth Table

| Input A | Input B | Output (A + B) |
|---------|---------|----------------|
|    0    |    0    |       0        |
|    0    |    1    |       1        |
|    1    |    0    |       1        |
|    1    |    1    |       1        |

### Logic Expression:
**Output = A + B**

- The OR gate outputs `1` if **at least one input is 1**.



3. NOT GATE
# Symbol:

![image](https://github.com/user-attachments/assets/11c5c4c7-a58d-4198-9339-0568330a39d7)


The NOT gate symbol represents a digital logic inverter, and it is visually distinct from other logic gates. It typically consists of:

 *A triangle pointing to the right

 *A small circle (called a "bubble") at the output, which indicates inversion

# Function :
The output Y is the negation of the input A, respresented as, Y = Ā Returns 1, if the input is 0. Returns 0, if the input is 1.


# Truth Table

| Input A | Output (¬A or A̅) |
|---------|-------------------|
|    0    |         1         |
|    1    |         0         |

### Logic Expression:
**Output = A̅** or **¬A**

- The NOT gate **inverts** the input:
  - If input is `0`, output is `1`
  - If input is `1`, output is `0`

4.NAND GATE
Symbol:

![image](https://github.com/user-attachments/assets/36e984b1-5ce3-41dd-8c14-e88d41a6bbd3)


Function :
A NAND (Not AND) gate gives an output of 0 only when both inputs are 1.

*It is the inverse of the AND gate.

 
# Truth Table

| Input A | Input B | Output (¬(A · B)) |
|---------|---------|-------------------|
|    0    |    0    |         1         |
|    0    |    1    |         1         |
|    1    |    0    |         1         |
|    1    |    1    |         0         |

### Logic Expression:
**Output = ¬(A · B)** or **(A · B)̅**

- The NAND gate outputs `0` **only when both inputs are 1**.
- It is the inverse of the

5.NOR GATE
Symbol :


![image](https://github.com/user-attachments/assets/b2b4d83d-6829-4038-a0ea-257c468c63a3)


Function :
A NOR (Not OR) gate gives an output of 1 only when both inputs are 0.

*It is the inverse of the OR gate.

# Truth Table

| Input A | Input B | Output (¬(A + B)) |
|---------|---------|-------------------|
|    0    |    0    |         1         |
|    0    |    1    |         0         |
|    1    |    0    |         0         |
|    1    |    1    |         0         |

### Logic Expression:
**Output = ¬(A + B)** or **(A + B)̅**

- The NOR gate outputs `1` **only when both inputs are 0**.
- It is the inverse of the OR gate.


6. XOR GATE
Symbol :


![image](https://github.com/user-attachments/assets/22181ba3-da25-4cbf-9f1e-6d48b90333b1)


Function :
The XOR (Exclusive OR) gate gives an output of 1 only when the inputs are different.

*Boolean Expression : Y = A ⊕ B = A̅·B + A·B̅
Truth Table :

# Truth Table

| Input A | Input B | Output (A ⊕ B) |
|---------|---------|----------------|
|    0    |    0    |       0        |
|    0    |    1    |       1        |
|    1    |    0    |       1        |
|    1    |    1    |       0        |

### Logic Expression:
**Output = A ⊕ B**

- The XOR gate outputs `1` **only when the inputs are different**.


7. XNOR GATE :
Symbol :

![image](https://github.com/user-attachments/assets/cc454957-c040-4244-ac74-eb705f4e0ff5)


Function :
The XNOR (Exclusive NOR) gate gives an output of 1 only when the inputs are the same.

*Boolean Expression : Y = (A ⊕ B)̅ = A·B + A̅·B̅

# Truth Table

| Input A | Input B | Output (A ⊙ B) |
|---------|---------|----------------|
|    0    |    0    |       1        |
|    0    |    1    |       0        |
|    1    |    0    |       0        |
|    1    |    1    |       1        |

### Logic Expression:
**Output = A ⊙ B** (also written as \(\overline{A \oplus B}\))

- The XNOR gate outputs `1` **only when the inputs are the same**.

------


# What is an IC

An IC (Integrated Circuit) is a compact, miniaturized electronic circuit built into a small chip of semiconductor material, usually silicon. It can contain millions of transistors, resistors, capacitors, and other components — all embedded together to perform specific functions.

# Types of Logic Gates and Their IC Numbers

Logic gates are the basic building blocks of digital circuits. Each gate performs a specific logic function and is available in the form of an Integrated Circuit (IC).



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










 
