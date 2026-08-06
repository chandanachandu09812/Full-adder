# Full Adder using Verilog

## Project Overview

A Full Adder is a combinational logic circuit that adds three binary inputs:

- A
- B
- Cin (Carry Input)

It produces two outputs:

- Sum
- Cout (Carry Output)

This project contains the Verilog implementation, testbench, and simulation of a Full Adder.

---

## Truth Table

| A | B | Cin | Sum | Cout |
|---|---|-----|-----|------|
|0|0|0|0|0|
|0|0|1|1|0|
|0|1|0|1|0|
|0|1|1|0|1|
|1|0|0|1|0|
|1|0|1|0|1|
|1|1|0|0|1|
|1|1|1|1|1|

---

## Logic Equations

Sum  = A ⊕ B ⊕ Cin

Cout = (A & B) | (Cin & (A ⊕ B))

---

## Files

- full_adder.v → Verilog design
- full_adder_tb.v → Testbench
- simulation_results.png → Simulation waveform

---

## Simulation

Run using ModelSim, Vivado, or Icarus Verilog.

Example:

iverilog full_adder.v full_adder_tb.v
vvp a.out
gtkwave dump.vcd

---

## Expected Output

All eight input combinations are tested and verified.
