---
title: "LLM Inference Testbed for Performance and Agentic-Quality Analysis"
excerpt: "Single-socket EPYC workstation running frontier-class 600B+ parameter language models locally, with 1TB RAM and 128GB VRAM across four AMD Radeon Pro V620 GPUs."
collection: portfolio
category: infrastructure
weight: 41
---

![LLM inference server build showing four AMD Radeon Pro V620 GPUs and EPYC 7713 in a Jonsbo N5 chassis](/images/llm-server-build.jpg)

A single-chassis system designed to run frontier-class large language models — including MiniMax M3, GLM-5.2, and Kimi K2.6 — at interactive speeds without cloud API dependency. It doubles as a testbed for measuring local inference performance and evaluating the agentic quality of open-weight models.

The build centers on an AMD EPYC 7713 (64-core, 8-channel DDR4) with 1TB of ECC RAM and four AMD Radeon Pro V620 GPUs providing 128GB of total VRAM. The EPYC's 8-channel memory bandwidth is the critical bottleneck for Mixture of Experts inference, where active expert weights must be loaded from system RAM on every forward pass. MoE model weights reside in system RAM, while the GPUs handle attention layers and the KV cache.

The V620s are passive datacenter cards that required custom 3D-printed fan shrouds paired with high-static-pressure server fans to achieve adequate cooling in a desktop chassis.

A primary use case is security research conducted on local, self-hosted models. Running inference in-house, with no external API dependency, keeps sensitive material — source code, forensic images, and case data — on controlled infrastructure, makes analyses reproducible, and keeps capability available during confidential investigations. It also gives full control over the models, prompts, and system configuration used to evaluate security-research workloads such as vulnerability analysis, code understanding, and forensic reconstruction. A complementary AMD Strix Halo laptop runs smaller but still capable models on the go.

The system runs under Proxmox and shares a chassis with the storage and networking described in [Research Computing Infrastructure](/portfolio/research-computing-infrastructure/); consolidating those roles into a single box added LLM inference as an entirely new capability.
