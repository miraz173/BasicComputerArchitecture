# CPU & RAM Architecture and Design

### Project Overview:
This project explores the fundamental design and interaction between a CPU and RAM, simulating how they work together to execute basic programs. The focus is on illustrating key principles of computer architecture, particularly the processes involved in instruction execution at the hardware level.

Built using **Logisim**, the project features a simple CPU architecture that interacts with RAM to execute instructions. Various components such as an ALU, RAM, registers, and control units are included.

### Features:
- **CPU Word Size:** 3 bits
- **ALU Operations:** ADD, ROL (Rotate Left), OR
- **Number of Registers:** 5
- **RAM Size:** 7 words
- **Word Size of ISA and RAM:** 16 bits
- **Supported Instructions:**
  - Branching (JC - Jump if Carry, JMP - Unconditional Jump)
  - Register and Immediate Operations

### Circuit Components:
The project contains a range of components designed in **Logisim**, including:
- **ALU (Arithmetic Logic Unit):** Handles basic arithmetic and logical operations like addition, bitwise OR, and ROL.
- **Registers:** Hold intermediate values during execution.
- **RAM (Random Access Memory):** Stores program instructions and data.
- **Other components:** Adder, Subtractor, Shifter, AND/OR gates, flip-flops, and multiplexers.

### Instruction Flow:
- **Instruction Fetch:** Instructions are initially loaded from ROM into RAM.
- **Execution:** After ROM is disabled, the program counter (PC) begins fetching instructions from RAM for execution.
- **Branching:** Basic branching instructions (`JC`, `JMP`) are supported.

### Visuals:
The repository includes images and diagrams illustrating the CPU architecture and its components (such as the ALU, registers, RAM). These visuals help to depict the layout and structure of the design.

### Functionality:
In the first 7 clock cycles, instructions are copied from ROM to RAM. Once the `PCenable` pin is activated, ROM is disabled, and instructions are fetched and executed from RAM in each clock cycle.

### Simulation:
The simulation begins with copying instructions to RAM during the first 7 clock cycles. Once enabled, the CPU executes instructions stored in RAM one per clock cycle. A video demonstrating the process can be found here:

[**Watch the Video**](https://youtu.be/Rh-h33NvQTE)

---

### How to Run:
- Use [**Logisim**](https://sourceforge.net/projects/circuit/) to open the provided `.dig` files and run the simulation.

---

### Notes:
This project was initially developed as part of an assignment, but it has since evolved into a hobby exploration of basic CPU and RAM design. Future enhancements may include more complex instructions and expanded functionality.
