---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Experience
======
* **Research Fellow**, May 2026 – present
  * University of Bologna, PULP Lab (PULP Platform, joint with ETH Zürich), Bologna, Italy
  * Research position on *Deployment on Heterogeneous Parallel Many-Core Architectures*, supervised by Prof. Francesco Conti, in collaboration with Fondazione Chips-IT, the Italian centre for semiconductor integrated-circuit design.
  * Develop cycle-level GVSoC models (C++) of a heterogeneous many-core mesh whose tiles combine RISC-V cores with digital in-memory-computing, matrix and vector accelerators, including the accelerator's scheduling logic and its DMA data path.
  * Map transformer attention workloads (Llama-3-8B, Gemma, SmolVLA) onto the modelled platform and check the outputs bit-exactly against golden references.
  * NeuroSoC project: wrote the Zephyr drivers for the control plane of the in-memory neural processing unit (IMNPU) as an out-of-tree module, covering the clock and reset controller, the interrupt controller, the flag controller, the node control and mesh routing registers, and the Snitch cluster peripheral.

* **Graduate Researcher (M.Sc. thesis and curricular internship)**, October 2025 – March 2026
  * University of Bologna, PULP Lab, Bologna, Italy
  * Deployed MicroLlama, a 526 K-parameter decoder-only transformer, on the eight-core Snitch RISC-V cluster with 128 KiB of scratchpad memory, by extending [Deeploy](https://github.com/pulp-platform/Deeploy), the open-source compiler jointly maintained by ETH Zürich and the University of Bologna, with operator support, multi-core FP32 kernels and DMA-driven tiling; merged upstream in [PR #153](https://github.com/pulp-platform/Deeploy/pull/153).
  * Showed in cycle-approximate simulation (GVSoC) that the tiling scales gracefully: shrinking the scratchpad budget 16×, from 128 KiB to 8 KiB, raises the end-to-end inference cycle count to only 1.43× that of the full-size run.
  * Obtained a 1.50× end-to-end speedup by rewriting MatMul with Snitch stream semantic registers (SSR) and floating-point repeat loops (FREP).

* **Research Intern, Embedded Software (NeuroSoC project)**, April 2025 – September 2025
  * University of Bologna, PULP Lab, Bologna, Italy
  * Brought up bare-metal and Zephyr RTOS applications on a dual-core CVA6 (RISC-V) SoC prototyped on a Genesys 2 FPGA board, loading and debugging each core over JTAG with OpenOCD and GDB.
  * Rewrote the NS16550-based UART driver for Zephyr with its own devicetree binding, as the first step towards the IMNPU driver.

Education
======
* **M.Sc. in Telecommunications Engineering**, University of Bologna, September 2023 – March 2026
  * Thesis: *Tiny LLM Automatic Deployment for RISC-V-Based High-Efficiency Compute Cluster Platforms*. Supervisor: Prof. Francesco Conti.
  * Selected courses: Deep Learning (30/30), Multimedia Services and Applications (30/30 cum laude), Architectures for Artificial Intelligence, Introduction to Computer Architectures.

Skills
======
* **Programming:** C, C++, Python
* **Embedded software:** Zephyr RTOS, device drivers, devicetree, bare-metal RISC-V, OpenOCD/GDB
* **ML deployment:** Deeploy, ONNX, operator kernels, memory tiling
* **Platforms and simulation:** RISC-V (Snitch cluster, CVA6), GVSoC, Xilinx FPGA (Vivado)
* **Tools:** Git, Linux, LaTeX

Languages
======
* Chinese (native), English (CEFR B2)
