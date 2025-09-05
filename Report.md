# Digital DNA
**Prerequisite:** An elementary understanding of Digital Logic
**Objective:** Mastering Verilog Through Creative Circuit Design
**Task:** Begin your journey into Verilog HDL by building meaningful projects.
## What is Verilog?
Verilog is a hardware description language (HDL) used to design and model digital electronic systems such as microprocessors, FPGAs, and ASICs..
**Purpose:** Instead of drawing circuits with gates and wires, you describe hardware behavior in code.
**Usage:** Widely used in VLSI design, FPGA programming, and ASIC development.
**Nature:** Unlike software languages (C, Python), Verilog doesn’t write instructions for a CPU—it describes actual hardware circuits.
### Types of modelling in Verilog 
1. Structural Modelling: Describe how gates/wires are connected.
2. Behavioral Modelling Describe circuit behavior using always blocks, if, case, etc.
3. Dataflow Modelling: Use Boolean expressions.

**Task 1**:Design and test an 8-bit signed arithmetic unit with operations:
Addition (00),Subtraction (01),Comparison (10) & Absolute difference (11)
Generate 3 status flags: overflow, zero, negative
**Outcomes and Process**
- Using of case statemes for each operation.
- Assigning status for each flag.
- Getting familiar with AMD Vivado .
![](IMG-20250811-WA0001.jpg)

**Task2**:Design a 2D Population Count Circuit that analyzes a 4×4 binary matrix and provides comprehensive bit counting statistics.
A population count (often called Hamming weight, bit count, or ones count) is the process of counting the number of 1s in the binary representation of a number.
**Outcomes and Process**
  - Using of 4X4 matrix and changing its possible values.
  - Obtain the count of ones in it.
  - The population count has been done.
![](IMG-20250811-WA0002.jpg)

**Task 3**:Design and test a 4-bit Ripple Carry Adder using a Generate Block. Each gate has a Rise, Fall, and Turn-Off Delay of 3ns, 6ns, and 2ns respectively.
**Note** The version in MARVEL does not support 3 delays i.e Rise,fall and Turn off. I had to do with 2 delays.
- A Ripple Carry Adder is a type of digital circuit used to add two binary numbers. It’s built by connecting full adders in series.
- Each full adder adds 2 input bits + a carry-in.
The carry-out from one adder is given to the carry-in of the next adder.
The carry “ripples” through the chain, hence the name.
**Disadvantages**
  Slow for large numbers because the carry must ripple through all stages.
**Outcomes**
  - Module Instantiation
  - Usage of delays
![](IMG-20250905-WA0001.jpg)

**Bonus Challenge** Design and test a Cellular Automaton of your choice: Rule 90, Rule 110, or 16x16 Conway's Game of Life.
**Rule 90**
Rule 90 is a one-dimensional cellular automaton with interesting properties.
The rules are simple. There is a one-dimensional array of cells (on or off). At each time step, the next state of each cell is the XOR of the cell's two current neighbours. A more verbose way of expressing this rule is the following table, where a cell's next state is a function of itself and its two neighbours.
The name "Rule 90" comes from reading the "next state" column: 01011010 is decimal 90.
![](IMG-20250905-WA0002.jpg)
[Github Codes](https://github.com/Nash1126/digitaldna)
