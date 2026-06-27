---
title: "LLM Inference Testbed for Performance and Agentic-Quality Analysis"
excerpt: "Single-socket EPYC workstation running frontier-class 600B+ parameter language models locally, with 1TB RAM, 128GB VRAM across four AMD Radeon Pro V620 GPUs, and 200TB of integrated storage."
collection: portfolio
category: infrastructure
weight: 41
---

![LLM inference server build showing four AMD Radeon Pro V620 GPUs and EPYC 7713 in a Jonsbo N5 chassis](/images/llm-server-build.jpg)

A single-chassis system designed to run frontier-class large language models — including MiniMax M3, GLM-5.2, and Kimi K2.6 — at interactive speeds without cloud API dependency. It doubles as a testbed for measuring local inference performance and evaluating the agentic quality of open-weight models.

The build centers on an AMD EPYC 7713 (64-core, 8-channel DDR4) with 1TB of ECC RAM and four AMD Radeon Pro V620 GPUs providing 128GB of total VRAM. The EPYC's 8-channel memory bandwidth is the critical bottleneck for Mixture of Experts inference, where active expert weights must be loaded from system RAM on every forward pass. MoE model weights reside in system RAM, while the GPUs handle attention layers and the KV cache.

The V620s are passive datacenter cards that required custom 3D-printed fan shrouds paired with high-static-pressure server fans to achieve adequate cooling in a desktop chassis.

A primary use case for this system is security research: running uncensored open-weight models that provide unrestricted assistance for vulnerability analysis, exploit development, and forensic reconstruction — tasks where commercial API-based models frequently refuse to assist due to safety guardrails. This complements an AMD Strix Halo laptop for running smaller but still capable models on the go.

Running under Proxmox, the system also serves as primary network infrastructure: a TrueNAS VM manages 156TB of RAIDZ2 HDD storage and 48TB of RAIDZ2 SSD storage, while an OPNsense VM with direct PCIe passthrough of the onboard dual 10GbE handles routing and firewall duties. This single box replaced an entire rack of dedicated appliances — a separate TrueNAS server, VM host, 16-bay JBOD, and dedicated OPNsense firewall — while adding LLM inference as an entirely new capability.

All hardware was sourced from the used enterprise market at a total build cost of approximately $14,000.
