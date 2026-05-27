# ⚡ RTL Design & Synthesis Workshop — VSD × SKY130

<p align="center">
  <img src="https://img.shields.io/badge/Workshop-RTL%20Design%20%26%20Synthesis-blueviolet?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0xMyAyLjA1djIuMDJjMy45NS41NCA3IDMuOTkgNyA4LjE4YzAgMy45NS0yLjU4IDcuMzctNiA4LjU4VjIyaC00di0xLjE3Yy0zLjQyLTEuMjEtNi00LjYzLTYtOC41OEMxIDcuMDIgNS4yOCAzLjQ1IDExIDMuMDVWMnptMiA4aDJsLTMgN3YtNUgxMmwzLTd2NXoiLz48L3N2Zz4=" />
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
  <b>A 10-day hands-on journey from Verilog RTL coding to gate-level synthesis using open-source tools and the SKY130 PDK.</b><br/>
  Organized by <a href="https://www.vlsisystemdesign.com">VLSI System Design (VSD)</a>
</p>

---

## 📌 Table of Contents

- [About the Workshop](#-about-the-workshop)
- [Tools & Environment](#-tools--environment)
- [Workshop Schedule](#-workshop-schedule)
- [Daily Lab Logs](#-daily-lab-logs)
- [Key Concepts Covered](#-key-concepts-covered)
- [Repository Structure](#-repository-structure)
- [Acknowledgements](#-acknowledgements)

---

## 🎯 About the Workshop

This workshop, offered by **VSD** under their **VSD-IAT** platform, covers the complete RTL-to-netlist design flow using industry-aligned open-source tools. Over 10 days, participants learn how to write synthesizable Verilog, simulate designs, debug waveforms, and map RTL to real silicon cells using the **SKY130 standard cell library**.

### 🔍 What this workshop teaches:
- Writing **RTL in Verilog** — modules, ports, always blocks, testbenches
- Simulating designs with **iverilog** and viewing waveforms in **GTKWave**
- Understanding **synthesis concepts** — why RTL maps differently from what you expect
- Running **Yosys synthesis** — from RTL to gate-level netlist
- Working with real **SKY130 standard cells** — the same PDK used in open-source tapeouts

> 💡 This repo documents my personal lab work, screenshots, observations, and learnings across all 10 days.

---

## 🛠 Tools & Environment

| Tool | Purpose | Version / Notes |
|------|---------|-----------------|
| `iverilog` | Verilog simulation compiler | Open-source HDL simulator |
| `GTKWave` | Waveform viewer | Reads `.vcd` files from iverilog |
| `Yosys` | Logic synthesis | Open-source synthesis suite |
| `SKY130 PDK` | Standard cell library | Google + SkyWater open PDK |
| `Linux Terminal` | All commands run here | Ubuntu / WSL compatible |
| `git` | Version control | For this repo |

---

## 📅 Workshop Schedule

| Day | Date | Module | Topics |
|-----|------|--------|--------|
| Day 1 | 27 May 2026 | Module 1 | Intro to Verilog, iverilog setup, GTKWave simulation |
| Day 2 | 28 May 2026 | Module 1 | RTL coding styles, testbench basics, simulation flow |
| Day 3 | 29 May 2026 | Module 2 | Module design, port connections, debugging simulations |
| Day 4 | 30 May 2026 | Module 2 | Sequential circuits, D flip-flop coding styles |
| Day 5 | 31 May 2026 | Module 3 | RTL labs — MUX, adders, comparators |
| Day 6 | 01 Jun 2026 | Module 3 | Testbench writing for digital blocks |
| Day 7 | 02 Jun 2026 | Module 4 | Yosys intro, synthesis concepts, Liberty files |
| Day 8 | 03 Jun 2026 | Module 4 | Synthesis runs, reading netlists, understanding reports |
| Day 9 | 04 Jun 2026 | Module 5 | RTL → gate-level with SKY130 cells |
| Day 10 | 05 Jun 2026 | Module 5 | Optimization, final synthesis labs, review |

---

## 📂 Daily Lab Logs

> Click each day to view detailed notes, commands, waveforms, and observations.

| # | Folder | Status | Topics |
|---|--------|--------|--------|
| 🟢 | [Day_1](./Day_1/) | ✅ Complete | iverilog + GTKWave setup, first simulation |
| ⚪ | Day_2 | 🔜 Upcoming | RTL coding styles, testbenches |
| ⚪ | Day_3 | 🔜 Upcoming | Module design, debugging |
| ⚪ | Day_4 | 🔜 Upcoming | Sequential RTL, DFFs |
| ⚪ | Day_5 | 🔜 Upcoming | Combinational RTL labs |
| ⚪ | Day_6 | 🔜 Upcoming | Testbench development |
| ⚪ | Day_7 | 🔜 Upcoming | Yosys intro, synthesis |
| ⚪ | Day_8 | 🔜 Upcoming | Synthesis runs, netlist analysis |
| ⚪ | Day_9 | 🔜 Upcoming | SKY130 cell mapping |
| ⚪ | Day_10 | 🔜 Upcoming | Final labs, optimization |

---

## 🧠 Key Concepts Covered

<details>
<summary><b>🔷 RTL Design & Simulation</b></summary>

- Writing synthesizable Verilog (always blocks, assign, module hierarchy)
- Behavioral vs structural modeling
- Writing testbenches and applying stimulus
- Simulating with `iverilog` and dumping `.vcd` files
- Viewing and analyzing waveforms in GTKWave

</details>

<details>
<summary><b>🔶 Synthesis with Yosys</b></summary>

- Understanding what synthesis does (RTL → Boolean → gates)
- Reading Liberty (`.lib`) files for cell timing data
- Running `synth`, `abc`, `show` commands in Yosys
- Reading and understanding the synthesized netlist
- Difference between simulation and synthesis results

</details>

<details>
<summary><b>🟣 SKY130 PDK Awareness</b></summary>

- Structure of the SKY130 standard cell library
- How cells are mapped during synthesis
- Gate-level simulation on the synthesized netlist
- Real silicon relevance — these cells are used in actual tapeouts

</details>

---

## 🗂 Repository Structure

```
RTL-Design-Workshop/
│
├── README.md               ← You are here
│
├── Day_1/
│   ├── README.md           ← Day 1 lab notes & observations
│   ├── *.v                 ← Verilog source files
│   ├── *.vcd               ← Waveform dump files
│   └── screenshots/        ← GTKWave / terminal screenshots
│
├── Day_2/                  ← (added after Day 2 session)
│   └── ...
│
└── ...                     ← Each day follows the same structure
```

> 📸 **Screenshots policy**: Every lab output (waveform, synthesis report, terminal output) is captured and stored in the respective day's `screenshots/` folder and linked in that day's README.

---

## 🙏 Acknowledgements

- **[Kunal Ghosh](https://www.linkedin.com/in/kunal-ghosh-vlsisystemdesign-com-28084836/)** — Founder, VSD; course instructor
- **[Shon Taware](https://www.linkedin.com/in/shon-taware/)** — Co-instructor
- **[VLSI System Design (VSD)](https://www.vlsisystemdesign.com)** — Workshop organizer and platform
- Open-source contributors behind **Yosys**, **iverilog**, **GTKWave**, and the **SKY130 PDK**

---

<p align="center">
  <img src="https://img.shields.io/badge/Made%20with-❤️%20%26%20Verilog-blueviolet?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Open%20Source-Yes-brightgreen?style=for-the-badge" />
</p>

<p align="center"><i>This repository grows daily as the workshop progresses. Check back each day for new lab logs! 🚀</i></p>
