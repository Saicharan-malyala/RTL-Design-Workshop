<h1 align="center">⚡ RTL Design and Synthesis Workshop — VSD x SKY130</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Workshop-RTL%20Design%20%26%20Synthesis-blueviolet?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Duration-10%20Days-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Status-In%20Progress-yellow?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Platform-VSD--IAT-9cf?style=for-the-badge" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/iverilog-Simulator-blue?style=flat-square" />
  <img src="https://img.shields.io/badge/GTKWave-Waveform%20Viewer-teal?style=flat-square" />
  <img src="https://img.shields.io/badge/Yosys-Synthesis-red?style=flat-square" />
  <img src="https://img.shields.io/badge/SKY130-PDK-lightblue?style=flat-square" />
  <img src="https://img.shields.io/badge/Language-Verilog-informational?style=flat-square" />
  <img src="https://img.shields.io/badge/OS-Linux-lightgrey?style=flat-square&logo=linux" />
</p>

<p align="center">
  <b>A hands-on journey from Verilog RTL coding to gate-level synthesis using open-source tools and the SKY130 PDK.</b><br/>
  Organized by <a href="https://www.vlsisystemdesign.com">VLSI System Design (VSD)</a> · Delivered via <a href="https://vsdiat.vlsisystemdesign.com">VSD-IAT Platform</a>
</p>

---

## 📌 Table of Contents

- [About the Workshop](#-about-the-workshop)
- [Tools and Environment](#-tools-and-environment)
- [Course Structure](#-course-structure)
- [What I Am Learning](#-what-i-am-learning)
- [Repository Structure](#-repository-structure)
- [Acknowledgements](#-acknowledgements)

---

## 🎯 About the Workshop

I am taking this workshop offered by **VSD** on the **VSD-IAT** platform to get hands-on with the complete RTL to gate-level netlist design flow using open-source tools. The workshop runs for **10 days (27 May 2026 to 5 June 2026)**, covering 5 structured days of content with dedicated time each day for lectures and lab practice.

The workshop uses the **SKY130 standard cell library** — the same open PDK backed by Google and SkyWater that is used in real tapeouts — which makes the synthesis labs feel a lot more practical than working with generic libraries.

> This repo is my personal documentation of everything I work through — lab commands, waveform screenshots, netlist outputs, and notes from each session.

---

## 🛠 Tools and Environment

| Tool | Purpose |
|------|---------|
| `iverilog` | Compiles and simulates Verilog designs |
| `GTKWave` | Views `.vcd` waveform dumps from simulation |
| `Yosys` | Synthesizes RTL Verilog to a gate-level netlist |
| `SKY130 PDK` | Standard cell library used during synthesis |
| `gvim` | Viewing Verilog and netlist files in the terminal |
| `git` | Version control for this repo |

---

## 📅 Course Structure

| Day | Topic |
|-----|-------|
| [Day 1](./Day_1/) | Introduction to Verilog RTL Design and Synthesis |
| Day 2 | Timing libs, hierarchical vs flat synthesis |
| Day 3 | Combinational and sequential optimizations |
| Day 4 | GLS, blocking vs non-blocking statements |
| Day 5 | Optimization in synthesis |

---

## 🧠 What I Am Learning

<details>
<summary><b>🔷 Day 1 -- Introduction to Verilog RTL Design and Synthesis</b></summary>

- How a simulator works: any change in input causes a change in output, and that is what gets tracked
- Writing a testbench and linking it with the design using iverilog
- Generating a `.vcd` (Value Change Dump) file and loading it in GTKWave
- What Yosys does: converts RTL Verilog into a gate-level netlist
- Running synthesis commands: `read_verilog`, `synth`, `abc`, `write_verilog`, `show`
- How to verify synthesis output using the same testbench stimulus from RTL simulation

</details>

<details>
<summary><b>🔶 Day 2 -- Timing libs, Hierarchical vs Flat Synthesis</b></summary>

- Understanding the `.lib` Liberty file structure -- what PVT corners mean and why they matter
- Difference between hierarchical and flat synthesis and when each is used
- How sub-modules are preserved or flattened during synthesis
- Efficient synthesis strategies for repeated module instances

</details>

<details>
<summary><b>🟣 Day 3 -- Combinational and Sequential Optimizations</b></summary>

- Combinational logic optimization techniques -- constant propagation and Boolean minimization
- Sequential logic optimizations -- state reduction and retiming
- How Yosys applies these optimizations during the synthesis run
- Special flip-flop coding styles that influence synthesis output

</details>

<details>
<summary><b>🟡 Day 4 -- Gate Level Simulation, Blocking vs Non-Blocking</b></summary>

- What Gate Level Simulation (GLS) is and why it is needed after synthesis
- How to run GLS using the synthesized netlist and SKY130 cell models
- Synthesis-simulation mismatches and what causes them
- The difference between blocking and non-blocking assignments in Verilog
- How blocking vs non-blocking affects the synthesized hardware

</details>

<details>
<summary><b>🟢 Day 5 -- Optimization in Synthesis</b></summary>

- Resource sharing and area optimization during synthesis
- Logic restructuring for timing closure
- Trade-offs between area, power, and performance in RTL-to-netlist mapping
- Final synthesis techniques for cleaner and more efficient gate-level output

</details>

---

## 🗂 Repository Structure

```
RTL-Design-Workshop/
│
├── README.md
│
├── Day_1/
│   ├── README.md          -- lab notes, commands, observations
│   └── screenshots/       -- GTKWave and terminal captures
│
├── Day_2/
│   └── ...
│
├── Day_3/
│   └── ...
│
├── Day_4/
│   └── ...
│
├── Day_5/
│   └── ...
│
└── LICENSE
```

> 📸 Every lab output including waveforms, synthesis reports, and terminal snapshots is saved in the respective day's `screenshots/` folder and referenced inside that day's README.

---

## 🙏 Acknowledgements

- **[Kunal Ghosh](https://www.linkedin.com/in/kunal-ghosh-vlsisystemdesign-com-28084836/)** -- Founder of VSD, course instructor
- **[Shon Taware](https://www.linkedin.com/in/shon-taware/)** -- Co-instructor
- **[VLSI System Design (VSD)](https://www.vlsisystemdesign.com)** -- Workshop organizer and platform
- Open-source contributors behind **Yosys**, **iverilog**, **GTKWave**, and the **SKY130 PDK**

---

<p align="center">
  <img src="https://img.shields.io/badge/Made%20with-❤️%20%26%20Verilog-blueviolet?style=for-the-badge" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Open%20Source-Yes-brightgreen?style=for-the-badge" />
</p>

<p align="center"><i>This repository grows day by day as I progress through the course. 🚀</i></p>
