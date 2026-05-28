# ⚡ RTL Design & Synthesis Workshop — VSD × SKY130

<p align="center">
  <img src="https://img.shields.io/badge/Workshop-RTL%20Design%20%26%20Synthesis-blueviolet?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Duration-10%20Days-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Batch-May%2027%20–%20Jun%205%202026-brightgreen?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Status-In%20Progress-yellow?style=for-the-badge" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Tool-iverilog-blue?style=flat-square&logo=gnu" />
  <img src="https://img.shields.io/badge/Tool-GTKWave-teal?style=flat-square" />
  <img src="https://img.shields.io/badge/Tool-Yosys-red?style=flat-square" />
  <img src="https://img.shields.io/badge/PDK-SKY130-9cf?style=flat-square" />
  <img src="https://img.shields.io/badge/Language-Verilog-informational?style=flat-square" />
  <img src="https://img.shields.io/badge/Platform-Linux-lightgrey?style=flat-square&logo=linux" />
</p>

<p align="center">
  <b>A hands-on journey from Verilog RTL coding to gate-level synthesis using open-source tools and the SKY130 PDK.</b><br/>
  Organized by <a href="https://www.vlsisystemdesign.com">VLSI System Design (VSD)</a> · Delivered via <a href="https://vsdiat.vlsisystemdesign.com">VSD-IAT Platform</a>
</p>

---

## 📌 Table of Contents

- [About the Workshop](#-about-the-workshop)
- [Tools & Environment](#-tools--environment)
- [Modules Covered](#-modules-covered)
- [Key Concepts](#-key-concepts)
- [Repository Structure](#-repository-structure)
- [Acknowledgements](#-acknowledgements)

---

## 🎯 About the Workshop

This is a self-paced, recorded workshop offered by **VSD** on the **VSD-IAT** platform, covering the complete RTL-to-netlist design flow using industry-aligned open-source tools.

Participants learn to write synthesizable Verilog, simulate designs, debug waveforms, and map RTL to real silicon cells using the **SKY130 standard cell library** — the same PDK used in Google-sponsored open tapeouts.

**What this workshop teaches:**
- Writing **RTL in Verilog** — modules, ports, always blocks, testbenches
- Simulating designs using **iverilog** and viewing waveforms in **GTKWave**
- Understanding **synthesis concepts** — why RTL maps differently than expected
- Running **Yosys synthesis** — from RTL to gate-level netlist
- Working with real **SKY130 standard cells** in an open-source ASIC flow

> 💡 This repo documents my personal lab work, commands, screenshots, and observations across all modules.

---

## 🛠 Tools & Environment

| Tool | Purpose | Notes |
|------|---------|-------|
| `iverilog` | Verilog simulation compiler | Open-source HDL simulator |
| `GTKWave` | Waveform viewer | Reads `.vcd` files from iverilog |
| `Yosys` | Logic synthesis | Open-source synthesis suite |
| `SKY130 PDK` | Standard cell library | Google + SkyWater open PDK |
| `Linux Terminal` | All commands run here | Ubuntu / WSL compatible |
| `git` | Version control | For this repo |

---

## 📚 Modules Covered

| Module | Title | Topics |
|--------|-------|--------|
| **Module 1** | Intro to Verilog & Simulation | iverilog setup, GTKWave, simulation flow, `.vcd` files |
| **Module 2** | RTL Coding Styles & Debugging | Module design, port connections, testbench writing, debugging |
| **Module 3** | RTL Design Labs | Combinational circuits, MUX, adders, comparators, DFFs |
| **Module 4** | Introduction to Yosys | Synthesis concepts, Liberty files, `synth`, `abc`, `show` commands |
| **Module 5** | RTL to Netlist with SKY130 | Gate-level synthesis, SKY130 cell mapping, netlist analysis |

> 📂 Each module has its own folder in this repo with lab notes, Verilog files, waveform dumps, and screenshots.

---

## 🧠 Key Concepts

<details>
<summary><b>🔷 RTL Design & Simulation</b></summary>

- Writing synthesizable Verilog — always blocks, assign statements, module hierarchy
- Behavioral vs structural modeling
- How simulators work — change in input triggers change in output
- Writing testbenches and applying stimulus
- Simulating with `iverilog` → generating `.vcd` → loading in `GTKWave`

</details>

<details>
<summary><b>🔶 Synthesis with Yosys</b></summary>

- What synthesis does: RTL → Boolean logic → gate-level netlist
- Reading Liberty (`.lib`) files — cell timing and area data
- Running `synth`, `abc`, `show` in Yosys
- Understanding the synthesized netlist
- Why synthesis result may differ from simulation (synthesis-simulation mismatch)

</details>

<details>
<summary><b>🟣 SKY130 PDK Awareness</b></summary>

- Structure of the SKY130 standard cell library
- How cells are selected and mapped during synthesis
- Gate-level simulation on the synthesized netlist
- Real silicon relevance — these exact cells are used in open-source tapeouts

</details>

---

## 🗂 Repository Structure

```
RTL-Design-Workshop/
│
├── README.md                  ← You are here
│
├── Module_1/
│   ├── README.md              ← Lab notes, observations, commands
│   ├── *.v                    ← Verilog source and testbench files
│   ├── *.vcd                  ← Waveform dump files
│   └── screenshots/           ← GTKWave / terminal screenshots
│
├── Module_2/
│   └── ...                    ← Same structure
│
├── Module_3/
│   └── ...
│
├── Module_4/
│   └── ...
│
├── Module_5/
│   └── ...
│
└── LICENSE
```

> 📸 Every lab output — waveform, synthesis report, terminal snapshot — is captured in the module's `screenshots/` folder and referenced in that module's README.

---

## 🙏 Acknowledgements

- **[Kunal Ghosh](https://www.linkedin.com/in/kunal-ghosh-vlsisystemdesign-com-28084836/)** — Founder, VSD; course instructor
- **[Shon Taware](https://www.linkedin.com/in/shon-taware/)** — Co-instructor
- **[VLSI System Design (VSD)](https://www.vlsisystemdesign.com)** — Workshop organizer and platform
- Open-source contributors behind **Yosys**, **iverilog**, **GTKWave**, and the **SKY130 PDK**

---

<p align="center">
  <img src="https://img.shields.io/badge/Made%20with-❤️%20%26%20Verilog-blueviolet?style=for-the-badge" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Open%20Source-Yes-brightgreen?style=for-the-badge" />
</p>

<p align="center"><i>This repository grows module by module as the workshop progresses. 🚀</i></p>
