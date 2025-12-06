# Verilog Digital Modules – README

This project contains four basic digital logic modules written in structural Verilog. Each file also includes a testbench to verify functionality in Vivado’s built-in simulator (xsim).

## 📁 Files

### 1. halfAdder.v

Implements a 1-bit Half Adder using:

* `xor` → sum
* `and` → carry

Testbench applies all 4 input combinations.
<img width="774" height="145" alt="image" src="https://github.com/user-attachments/assets/6c0d526f-e20e-4805-a8f4-8a81fd908167" />

### 2. fullAdder.v

Implements a **1-bit Full Adder** using AND, XOR, and OR gates.
Testbench checks all 8 possible inputs.
<img width="770" height="164" alt="image" src="https://github.com/user-attachments/assets/bd6b8546-2244-496f-9221-f87fb3844096" />

### 3. mux2to1.v

A 2:1 multiplexer built from:

* NOT gate
* Two AND gates
* OR gate
Testbench verifies both select states.
<img width="1235" height="390" alt="image" src="https://github.com/user-attachments/assets/2b889902-8a9b-458b-9d11-a59058cde2c4" />

### 4. mux4to1.v

A 4:1 multiplexer using:

* Two NOT gates
* Four AND gates
* One OR gate
Testbench checks all select combinations.
<img width="842" height="217" alt="image" src="https://github.com/user-attachments/assets/f685bf2f-1a75-4b55-b0d6-8885cd62ee98" />

## ▶️ Running in Vivado

1. Open Vivado → *Create New Project*
2. Add the source files (`halfAdder.v`, `fullAdder.v`, `mux2to1.v`, `mux4to1.v`)
3. Add testbench files as **simulation sources**
4. Go to **Flow → Run Simulation → Run Behavioral Simulation**
5. View outputs in the waveform window

## ✔ Notes

* All modules use **structural modeling** (gates-level design).
* Testbenches automatically display results using `$monitor`.

