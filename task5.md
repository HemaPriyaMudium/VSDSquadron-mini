## 1. FUNCTIONAL SIMULATION

### 1.1 About iverilog and gtkwave
- Icarus Verilog is an implementation of the Verilog hardware description language.
- GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing.
  
### 1.2 Installing iverilog and gtkwave

- **For Ubuntu**

 Open your terminal and type the following to install iverilog and GTKWave
 ```
 $   sudo apt get update
 $   sudo apt get install iverilog gtkwave
 ```

![WhatsApp Image 2024-03-07 at 20 58 07_fc0fb77b](https://github.com/HemaPriyaMudium/VSDSquadron-mini/assets/160724714/e561638c-172b-416c-a254-dbd179a04b9f)


- **To clone the repository and download the netlist files for simulation, enter the following commands in your terminal.**

 ```
 $ git clone https://github.com/Animeshhhh15/VSDSQUADRON-MINI-.git
 $ cd 
```

![WhatsApp Image 2024-03-07 at 20 58 07_2b8be166 (2)](https://github.com/HemaPriyaMudium/VSDSquadron-mini/assets/160724714/024a497c-e586-4fe4-b7c7-266162b16b98)



- **To simulate and run the Verilog code, enter the following commands in your terminal.**

```
$ iverilog -o hello hello.v hello_tb.v
$ ./hello
```
![WhatsApp Image 2024-03-07 at 20 59 47_cd0329ac(3)](https://github.com/HemaPriyaMudium/VSDSquadron-mini/assets/160724714/68244181-9cea-486f-829f-ca57c5ae574c)





- **To see the output waveform in gtkwave, enter the following commands in your terminal.**

`$ gtkwave hello.vcd`

![WhatsApp Image 2024-03-07 at 21 00 38_f6ab8049(4)](https://github.com/HemaPriyaMudium/VSDSquadron-mini/assets/160724714/f51f6ead-fceb-4229-9efd-a6998a2d0b8a)


### 1.3 The output waveform

![WhatsApp Image 2024-03-07 at 21 00 38_ec1ff573(5)](https://github.com/HemaPriyaMudium/VSDSquadron-mini/assets/160724714/65a312a0-4fc4-47a7-b4be-f9e74736d017)


![WhatsApp Image 2024-03-07 at 21 00 41_ce1ac901(6)](https://github.com/HemaPriyaMudium/VSDSquadron-mini/assets/160724714/3aeaa830-1187-4046-b833-aaab452b531c)


