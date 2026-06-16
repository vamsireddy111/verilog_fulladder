# Full Adder using Verilog
# Overview

A Full Adder is a combinational circuit that performs binary addition of three input bits: two significant bits and a carry-in. It produces a Sum and a Carry-out.

This project demonstrates the design and simulation of a Full Adder using Verilog HDL, which is a key building block for arithmetic circuits like adders and ALUs.

# Working Principle

The Full Adder adds:

A → First input bit
B → Second input bit
Cin → Carry input from previous stage
# Outputs:
S → Sum
Cout → Carry output

# Truth Table
A	B	Cin	Sum (S)	Carry (Cout)
0	0	 0	 0	      0
0	0	 1	 1	      0
0	1	 0	 1	      0
0	1	 1	 0	      1
1	0	 0	 1	      0
1	0	 1	 0	      1
1	1	 0	 0	      1
1	1	 1	 1	      1

# Logic Equations
S = A ⊕ B ⊕ Cin
Cout = (A · B) + (B · Cin) + (A · Cin)

# Key Observations
Sum is HIGH when an odd number of inputs are HIGH
Carry is generated when two or more inputs are HIGH
Output updates immediately (combinational logic)
