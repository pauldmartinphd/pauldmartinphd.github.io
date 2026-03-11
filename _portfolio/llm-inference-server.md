---
title: "Local LLM Inference Server"
excerpt: "Single-socket EPYC workstation running frontier-class 600B+ parameter language models locally, with 768GB RAM, 128GB VRAM across four AMD Radeon Pro V620 GPUs, and 200TB of integrated storage."
collection: portfolio
category: professional
date: 2026-03-01
---

A single-chassis system designed to run frontier-class large language models — including DeepSeek V3, GLM-5, Kimi K2.5, and Qwen3.5 397B — at interactive speeds without cloud API dependency.

The build centers on an AMD EPYC 7713 (64-core, 8-channel DDR4) with 768GB of ECC RAM and four AMD Radeon Pro V620 GPUs providing 128GB of total VRAM. The EPYC's 8-channel memory delivers approximately 190 GB/s of sustained bandwidth, which is the critical bottleneck for Mixture of Experts inference where active expert weights must be loaded from system RAM on every forward pass. The GPUs handle attention layers, KV cache, and draft model inference, keeping the CPU memory bus reserved for expert loading.

Running under Proxmox, the system also serves as primary network infrastructure: a TrueNAS VM manages 156TB of RAIDZ2 HDD storage and 46TB of RAIDZ2 SSD storage, while an OPNsense VM with direct PCIe passthrough of the onboard dual 10GbE handles routing and firewall duties. This single box replaced an entire rack of dedicated appliances — a separate TrueNAS server, VM host, 16-bay JBOD, and dedicated OPNsense firewall — while adding LLM inference as an entirely new capability.

All hardware was sourced from the used enterprise market at a total build cost of approximately $14,000.
