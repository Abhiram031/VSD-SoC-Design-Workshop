# How to talk to Computers?

#### Introduction to QFN-48, Package, chips, pads, core, die and IPs

So, to start how actually we talk to the computers.. Let's dive into this topic

To begin with, each computer has a Processor/SoC which all generally have all of the things shown in the below image.

![image1](Day 1/images/1.png)

Inside the Processor, what lies is the core of the everything. For example take Arduino Leonardo, which has the ATMega32u4 RISC-based microcontroller.

![[images\2.png]]

The interconnects are made between the integrated circuit (IC) and its packaging during semiconductor device fabrication with wire bonds. This can be depicted from the above image, in which to the cental chip wire bonds are connected to all the pins on the packaging.

![[images\3.jpg]]

A chip which is reverse engineered and the inside of the chip is seen, in which the wire bonds are connneted to the chip and all the other pins on the packaging.

![[images\image1.png]]

- **`QFN-48`**: This refers to a type of package used for integrated circuits (ICs). It's a Quad Flat No-Lead package with 48 pins. It's a miniature, square-shaped package.

- **`Package`**: This is the physical container that houses the actual chip, providing protection and a way to connect it to a circuit board.

- **`Chip`**: This is a small piece of silicon that contains the electronic circuits of an IC. It's also called a die. A chip consists of various components
  
  - **`Pads`**: These are small metal landing areas on the package that connect the chip's internal circuitry to the external pins.
  
  - **`Core`:** This can refer to the central processing unit (CPU) of a computer, which is the main chip responsible for processing instructions.
  
  - **`Die`:** Another term for the chip itself, which is the actual piece of silicon containing the transistors and other microscopic circuitry

And inside the core, we can various things like RISC-V SoC, SRAM, PLL, ADC, DAC, SPI etc..

#### Introduction to RISC-V ISA, Instruction Set Architecture

`ISA`: ISA is the set of instructions that a processor can execute.

Imagine giving instructions to your computer in any high level language. That's kind of like your C code. But the computer only understands ones and zeros.

Here's how we bridge the gap:

1. The C code is translated into a simpler language the computer can almost understand, like RISC-V assembly (think of it as instructions in short sentences).
2. Then, that assembly code is translated into the computer's true language: ones and zeros, also called machine code(Binary). This is like the computer finally understanding the instructions.
3. The layout, or the physical chip itself, is where this machine code gets executed, and that's we get the desired results.

Here's an extra detail: There's a special code called HDL (Hardware Description Language) that acts like a bridge between the RISC-V architecture (think of it as the brain of the computer) and the layout (the physical chip).

![[images\4.png]]

So, we will be looking into more on how RTL2GDS is done in the upcoming sections

#### From software applications to hardware

Now, Ever wondered how you click an icon and magic happens on your screen? Let's understand the process

1. **Breaking down the code (Compiler):** Applications start in a language we understand, like English for C code. The operating system (OS) acts as the first translator, breaking it down into a simpler form called assembly code. So, the compiler's job is to take the application code and convert it into the respective instructions for the given hardware.

2. **To 1's and 0's :** Assembly is closer to what the computer understands, but not quite there yet. A program called assembler takes the assembly code and translates it into Binary Code.

3. **Talking to the hardware:** Finally, the machine code, a series of 0s and 1s, is fed to the hardware (the layout or chip). The hardware recognizes patterns in this code and performs the corresponding actions based on its capabilities, which are defined by its architecture (ISA).

4. **Behind the scenes :** This explanation covers the main steps. A special code called RTL helps translate the high-level instructions into detailed blueprints (netlist) for the chip's layout.
   
   This RTL is then synthesized to get the `netlist`. Netlist is synthesized or `gate-level` version of the specification. It is in the form of gates and flip-flops.
   
   Finally the netlist converted into layout using the RTL2GDS flow.

![[images\5.png]]
<p style="text-align: center;">Application to Hardware Layout flow</p>

![[images\6.png]]
<p style="text-align: center;">ISA to Hardware Layout flow</p>
