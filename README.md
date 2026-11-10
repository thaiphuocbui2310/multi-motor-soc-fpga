# Multi-Motor Control SoC on FPGA

> 🎓 **Thesis Project** — Danang University of Science and Technology  
> 📅 Sep 2026 – Present &nbsp;|&nbsp; Status: **In Progress**

---

## 📌 Overview

An FPGA-based System-on-Chip (SoC) designed for **multi-axis PMSM (Permanent Magnet Synchronous Motor) servo control**, following a published reference architecture.

The system integrates:
- A **3-stage pipelined 32-bit RISC-V CPU** as the main processor
- A **hardware control coprocessor** supporting up to **6 servo axes** in parallel

This project serves as my undergraduate thesis and is planned to be extended into a research publication.

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────┐
│                  FPGA SoC System                    │
│                                                     │
│  ┌─────────────────┐    ┌────────────────────────┐  │
│  │  32-bit RISC-V  │    │  Hardware Control      │  │
│  │  CPU (3-stage   │◄──►│  Coprocessor           │  │
│  │  pipeline)      │    │  (up to 6 PMSM axes)   │  │
│  └─────────────────┘    └────────────────────────┘  │
│                                                     │
│  ┌──────────────────────────────────────────────┐   │
│  │          Memory & Peripheral Bus             │   │
│  └──────────────────────────────────────────────┘   │
└─────────────────────────────────────────────────────┘
```

---

## 🛠️ Tech Stack

| Component | Technology |
|-----------|-----------|
| HDL | Verilog |
| Simulation | ModelSim |
| Synthesis | Quartus Prime |
| Target Board | Intel/Altera FPGA |
| CPU ISA | RISC-V (RV32I) |

---

## 📋 Progress

- [x] Study reference architecture & published design
- [x] Learn RTL design fundamentals in Verilog
- [ ] Implement RISC-V CPU (3-stage pipeline)
- [ ] Implement hardware control coprocessor
- [ ] ModelSim functional verification
- [ ] FPGA synthesis & place-and-route
- [ ] Hardware testing on FPGA board
- [ ] Research paper draft

---

## 👨‍💻 Author

**Bui Thai Phuoc**  
Control and Automation Engineering, DUT  
📧 thaiphuocbui2310@gmail.com  
🔗 [linkedin.com/in/thaiphuocbui](https://linkedin.com/in/thaiphuocbui)

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.
