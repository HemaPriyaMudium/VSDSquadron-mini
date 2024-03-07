# As per the Update given for the next task "Should Use the RISC-V Core Verilog netlist and testbench for functional Simulation.
# Veriog code is being executed and the waveforms are generated using the gtkwave

# Aim: To verify the Functional Simulation:-
# Table of contents
- [1.RISC-V RV32I](#1-RISC-V-RV32I)
 - [2.BLOCK DIAGRAM OF RISC-V RV32I](#2-BLOCK-DIAGRAM-OF-RISC-V-RV32I)
 - [3.INSTRUCTION SET OF RISC-V RV32I](#3-INSTRUCTION-SET-OF-RISC-V-RV32I)
 - [4.FUNCTIONAL SIMULATION](#4-FUNCTIONAL-SIMULATION)
    - [4.1 About iverilog and gtkwave](#41-About-iverilog-and-gtkwave)
    - [4.2 Installing iverilog and gtkwave](#42-Installing-iverilog-and-gtkwave)
    - [4.3 The output waveform](#43-The-output-waveform)
  
   ## 1. RISC-V RV32I

This project provides an insight into the working of a few important instructions of the instruction set of a Single cycle Reduced Instruction Set Computer - Five(RISC-V) Instruction Set Architecture suitable for use across wide-spectrum of Applications from low-power embedded devices to high-performance Cloud-based Server processors. The base RISC-V is a 32-bit processor with 31 general-purpose registers, so all the instructions are 32-bit long. Some Applications where the RISC-V processors have begun to make some significant threads are in Artificial intelligence and machine learning, Embedded systems, ultra-low power processing systems, etc.

## 2. BLOCK DIAGRAM OF RISC-V RV32I
![image](https://github.com/HemaPriyaMudium/VSDSquadron-mini/assets/160724714/020f334b-120d-435c-9f96-a441c688cb75)


## 3. INSTRUCTION SET OF RISC-V RV32I
![image](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/c7f94f2b-3d2f-4bad-84a6-b95af2979f9c)

![image](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/6540c09b-570e-48c7-9569-5a304af15fa4)

## 4. FUNCTIONAL SIMULATION

### 4.1 About iverilog and gtkwave
- Icarus Verilog is an implementation of the Verilog hardware description language.
- GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing.
  
### 4.2 Installing iverilog and gtkwave

- **For Ubuntu**
- **To clone the repository and download the netlist files for simulation, enter the following commands in your terminal.**

 ```
 $ git clone https://github.com/Archanakattii/karchana
 $ cd hello
```
 Open your terminal and type the following to install iverilog and GTKWave
 ```
 $   sudo apt get update
 $   sudo apt get install iverilog gtkwave
 ```
![Screenshot from 2024-03-06 15-34-36](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/817a18ee-9914-4c1f-8700-d14f62b4bcc3)


![Screenshot from 2024-03-06 15-35-29](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/6ede157a-d64b-4a23-b87d-1cb4efc3f139)




- **To simulate and run the Verilog code, enter the following commands in your terminal.**

```
$ iverilog -o hello hello.v hello_tb.v
$ ./hello
```
![WhatsApp Image 2024-03-06 at 4 07 35 PM](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/ca8c05ff-d87b-4688-b930-af33990e8631)

- **To see the output waveform in gtkwave, enter the following commands in your terminal.**

`$ gtkwave hello.vcd`

![WhatsApp Image 2024-03-06 at 4 07 34 PM](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/0a8da2db-9750-4529-8c5b-161b73759095)

### 4.3 The output waveform

 The output waveform showing the instructions performed in a 5-stage pipelined architecture.
 
 Instruction 1:add r6,r2,r1
 ![image](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/0675695c-bf6b-4eba-97c5-e9ba685e3c7b)

 Instruction 2:sub r7,r1,r2
![image](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/d31d779e-105e-495b-9526-7c81125c3f1d)

Instruction 3:and r8,r1,r3
![image](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/6969df03-8b47-44e9-9d95-c177ffaefc7d)


Instruction 4:or r9,r2,r5
![image](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/8115fc18-3b5d-4d59-81ef-45a9ea09a099)


 Instruction 5:xor r10,r1,r4
![image](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/a6794484-f49c-483f-922e-3bdf623ddab1)


 Instruction 6:slt r11,r2,r4
![image](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/e9e6cfbb-2509-4135-a0f7-af9dcf109514)



 Instruction 7:addi r12,r4,5
![image](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/294f0d1c-0724-4aac-a451-a1778eb28c29)

 Instruction 8:sw r3,r1,2
![image](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/6dd649f7-4f42-4809-aea8-b28292c18c44)

 Instruction 9:lw r13,r1,2
![image](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/7d4a796f-80e7-4558-b6af-e1616a5ad982)

 Instruction 10:beq r0,r0,15
 ![image](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/a5527da9-efee-4593-bf5d-0a161dec62ae)

 After branching, performing
 Instruction 11:add r14,r2,r2
 ![image](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/ac89165d-ab48-4f68-8ca6-aed6998c5c44)

  Full 5-stage instruction pipeline and pc-increment description Waveform
  
![image](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/d4f62cd0-2b5d-4205-a6ce-3576addc9bf1)

![WhatsApp Image 2024-03-06 at 4 07 41 PM](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/806fe8ea-4c44-42b3-b028-0f9b32e10f1c)


![WhatsApp Image 2024-03-06 at 4 04 43 PM](https://github.com/Animeshhhh15/VSDSQUADRON-MINI-/assets/160756499/92e741a5-0c62-44a0-9809-61e44b5e6184)

