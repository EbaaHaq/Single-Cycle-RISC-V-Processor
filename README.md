# Single-Cycle RISC-V Processor  

This project implements a **RISC-V processor using a single-cycle architecture**. Each instruction is executed within a single clock cycle, offering simplicity in design. The processor also includes **Control and Status Register (CSR)** functionality for system-level control and seamless exception handling.  

---

## Features  

### Key Highlights  
- **Single-Cycle Architecture:** Executes each instruction in one clock cycle.  
- **Control and Status Registers (CSR):** Provides efficient exception handling and system control.  
- **Simple Design:** Ideal for educational purposes and demonstrating the core concepts of processor design.  

### Supported Instruction Types  
- **R-Type:** ADD, SUB, AND, OR, XOR, etc.  
- **I-Type:** ADDI, SLTI, LW, etc.  
- **U-Type:** LUI, AUIPC.  
- **B-Type:** BEQ, BNE, BLT, etc.  
- **J-Type:** JAL, JALR.  

### Load and Store Instructions  
- **Load:** LW (Load Word), LH/UH (Load Halfword/Unsigned), LB/UB (Load Byte/Unsigned).  
- **Store:** SW (Store Word), SH (Store Halfword), SB (Store Byte).  

---

## Prerequisites  

To run and simulate the project, ensure you have the following tools installed:  
- **SystemVerilog:** For designing and implementing the processor.  
- **VSCode:** Recommended for editing SystemVerilog files with ease.  
- **ModelSim/Vivado:** For simulating and testing the design.  
- **GTKWave:** For visualizing waveforms (requires Multisim for functionality).  

---

## How to Use  

1. Clone the repository:  
   ```bash  
   git clone https://github.com/your-username/single-cycle-riscv-processor.git  
   ```  
2. Open the project in **VSCode** and ensure SystemVerilog extensions are installed.  
3. Compile the SystemVerilog files:  
   ```bash  
   vlog *.sv  
   ```  
4. Simulate the design:  
   ```bash  
   vsim -c tb_processor -voptargs=+acc -do "run -all"  
   ```  
5. Visualize waveforms in **GTKWave**:  
   ```bash  
   gtkwave processor.vcd  
   ```  

---

## Educational Purpose  

This project is designed to help students and enthusiasts understand the basics of processor architecture. It demonstrates the simplicity and functionality of a single-cycle processor while highlighting the role of Control and Status Registers (CSR) in system-level tasks.  

---

## License

This project is not licensed yet. Please feel free to use it with proper attribution.
