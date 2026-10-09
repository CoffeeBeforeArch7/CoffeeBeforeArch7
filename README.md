<!-- Profile README for Pinxu Wang -->

<h1 align="center">Hi, I'm Pinxu 👋</h1>

<p align="center">
  <b>Electrical & Computer Engineering (M.Eng.) @ UIUC</b><br/>
  RTL Design • Computer Architecture • Design Verification • Physical Implementation • FPGA / SoC
</p>

---

## 🚀 About Me
- 🎓 Master of Engineering student in **Electrical & Computer Engineering** at the **University of Illinois Urbana-Champaign**
- 🧠 Focused on **digital design, microarchitecture, and verification**, with hands-on work across the flow from RTL to layout
- 🧩 Worked on an **out-of-order RV32IM core**, a pipelined 4-way cache, a **full-custom bit-sliced RV32I datapath** taken through place and route, and a **UVM environment** for a CNN inference NPU
- 🔬 Verified two features of a configurable **AXI address-remapping IP** as a verification intern, closing 100% line, branch, and functional coverage
- 🧪 Work on both sides of the testbench: RTL on one side, reference models, scoreboards, SVA, and coverage on the other

---

## 🛠️ Technical Stack

### 🔹 Digital Design & Computer Architecture
<p>
  <img src="https://img.shields.io/badge/SystemVerilog-00979D?logo=verilog&logoColor=fff"/>
  <img src="https://img.shields.io/badge/RTL%20Design-555555"/>
  <img src="https://img.shields.io/badge/Microarchitecture-555555"/>
  <img src="https://img.shields.io/badge/Tomasulo%20Out--of--Order%20Execution-555555"/>
  <img src="https://img.shields.io/badge/Pipelined%20Processors-555555"/>
  <img src="https://img.shields.io/badge/Cache%20%26%20Memory%20Systems-555555"/>
  <img src="https://img.shields.io/badge/Branch%20Prediction-555555"/>
  <img src="https://img.shields.io/badge/IEEE--754%20FP16-555555"/>
</p>

---

### 🔹 Verification
<p>
  <img src="https://img.shields.io/badge/UVM-555555"/>
  <img src="https://img.shields.io/badge/UVM%20RAL-555555"/>
  <img src="https://img.shields.io/badge/SystemVerilog%20Assertions-555555"/>
  <img src="https://img.shields.io/badge/Constrained--Random%20Testing-555555"/>
  <img src="https://img.shields.io/badge/Functional%20Coverage-555555"/>
  <img src="https://img.shields.io/badge/Scoreboards%20%26%20Reference%20Models-555555"/>
  <img src="https://img.shields.io/badge/VCS-8A2BE2"/>
  <img src="https://img.shields.io/badge/Verdi-8A2BE2"/>
  <img src="https://img.shields.io/badge/SpyGlass%20(Lint%20%26%20CDC)-8A2BE2"/>
  <img src="https://img.shields.io/badge/RVFI-555555"/>
  <img src="https://img.shields.io/badge/Spike%20(RISC--V)-555555"/>
</p>

---

### 🔹 Physical Design & EDA
<p>
  <img src="https://img.shields.io/badge/Virtuoso-8A2BE2"/>
  <img src="https://img.shields.io/badge/Design%20Compiler-8A2BE2"/>
  <img src="https://img.shields.io/badge/Innovus-8A2BE2"/>
  <img src="https://img.shields.io/badge/Calibre-8A2BE2"/>
  <img src="https://img.shields.io/badge/Full--Custom%20Layout-555555"/>
  <img src="https://img.shields.io/badge/Standard--Cell%20P%26R-555555"/>
  <img src="https://img.shields.io/badge/DRC%20%26%20LVS-555555"/>
  <img src="https://img.shields.io/badge/Liberty%20%26%20LEF-555555"/>
  <img src="https://img.shields.io/badge/FreePDK45-555555"/>
  <img src="https://img.shields.io/badge/Tcl-555555"/>
</p>

---

### 🔹 Languages, Protocols & FPGA
<p>
  <img src="https://img.shields.io/badge/C-00599C?logo=c&logoColor=fff"/>
  <img src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=fff"/>
  <img src="https://img.shields.io/badge/NumPy-013243?logo=numpy&logoColor=fff"/>
  <img src="https://img.shields.io/badge/Shell-4EAA25?logo=gnubash&logoColor=fff"/>
  <img src="https://img.shields.io/badge/Makefile-555555"/>
  <img src="https://img.shields.io/badge/Bazel-43A047?logo=bazel&logoColor=fff"/>
  <img src="https://img.shields.io/badge/Linux-555555?logo=linux&logoColor=fff"/>
  <img src="https://img.shields.io/badge/Git-F05032?logo=git&logoColor=fff"/>
  <img src="https://img.shields.io/badge/AMBA%20AXI4%20%26%20APB-555555"/>
  <img src="https://img.shields.io/badge/SPI-555555"/>
  <img src="https://img.shields.io/badge/Vivado-EE4C2C"/>
  <img src="https://img.shields.io/badge/Zynq%20SoC-555555"/>
</p>

---

## 📌 Featured Projects

### 🧠 Hardware & RTL Design

| Project | Description | Tech | Repo |
|------|------------|------|------|
| **Out-of-Order RV32IM Core** | Single-issue Tomasulo-style core from the UIUC ECE 411 final project. A RAT renames onto ROB tags, four 4-entry reservation stations (ALU, MDU, LSU, JMP) wake on CDB broadcasts, and a 16-entry ROB commits in order. Bimodal branch predictor with a 16-entry BTB, split 2 KB 4-way write-back I/D caches with tree-PLRU, and a 16-entry store buffer. | SystemVerilog, VCS, Verdi, RVFI, CoreMark | [OoO Core](https://github.com/CoffeeBeforeArch7/sw_OoO_processor) |
| **Pipelined 4-Way Set-Associative Cache** | Two-stage pipelined write-back, write-allocate cache with 16 sets, 4 ways, 32 B lines, and tree-PLRU replacement. One-cycle hit latency and one read per cycle on hits. | SystemVerilog, VCS, Verdi | [Pipelined Cache](https://github.com/CoffeeBeforeArch7/Pipelined-4-Way-Set-Associative-Cache) |
| **RV32I: RTL to GDSII** | Single-cycle, bit-sliced RV32I on FreePDK45. Full-custom cells and a 32×32 register-file macro drawn in Virtuoso (Calibre DRC/LVS clean), then placed and routed with Design Compiler and Innovus next to standard cells. The final layout replaces 1024 flip-flops with 32 macro instances and closes DRC clean. | SystemVerilog, Virtuoso, Design Compiler, Innovus, Calibre, Tcl | [RV32I RTL-to-GDSII](https://github.com/CoffeeBeforeArch7/rv32i-cpu-rtl-to-gdsii) |

---

### ✅ Design Verification

| Project | Description | Tech | Repo |
|------|------------|------|------|
| **LeNet-5 CNN NPU Verification** | UVM environment for a multi-clock-domain FP16 LeNet-5 inference NPU. A virtual sequencer coordinates SPI register and weight writes (Synopsys SPI VIP, 522 registers in UVM RAL) with the pixel stream, and a NumPy FP16 reference model matching the RTL accumulation order drives bit-exact checks. 27 chip-level regressions reached 97.5% line, 96.6% branch, and 100% in-scope functional coverage. Root-caused an adder alignment bug and a CDC FIFO path without full-flag backpressure, then added three SVA checks. | SystemVerilog, UVM, SVA, VCS, Verdi, Python, NumPy | Private (course material, licensed VIP) |
| **Asynchronous FIFO** | Gray-coded-pointer FIFO with parameterized width and depth, plus a class-based SystemVerilog testbench: generator, driver, monitor, scoreboard, and clock/reset generators, with coverage collected in VCS. | SystemVerilog, VCS | [Async FIFO](https://github.com/CoffeeBeforeArch7/Asynchronous_FIFO_Design_and_Verification_Framework) |

---

### ⚙️ FPGA, SoC & Tooling

| Project | Description | Tech | Repo |
|------|------------|------|------|
| **Zynq SoC Lab Series** | Four-part FPGA/SoC lab series (ECE 527 MP1a–d) on a Zynq-based platform, covering the Vivado flow, embedded SoC design, the AXI protocol, and DMA. | Vivado, Zynq, AXI, DMA | [Zynq Labs](https://github.com/CoffeeBeforeArch7/Zynq-based-Accelerator) |
| **drawio-arch-kit** | Python kit that draws dark-theme architecture diagrams in draw.io from code. A four-step text → ASCII → design → draw.io workflow, plus two self-check scripts that catch diagonal wires, lines through boxes, and overlapping text. Sample: a four-page 5-stage RV32I pipeline diagram. Docs in Chinese. | Python, draw.io | [drawio-arch-kit](https://github.com/CoffeeBeforeArch7/drawio-arch-kit) |

---

## 📫 Let's Connect
<p>
  <a href="https://www.linkedin.com/in/pinxu-w-32ba602b8">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?logo=linkedin&logoColor=fff"/>
  </a>
  <a href="mailto:pinxuw@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?logo=gmail&logoColor=fff"/>
  </a>
  <a href="https://coffeebeforearch.com">
    <img src="https://img.shields.io/badge/Website-FF5D01?logo=astro&logoColor=fff"/>
  </a>
</p>

---

<p align="center"><i>From spec to RTL to layout, and the testbenches that check it.</i></p>
