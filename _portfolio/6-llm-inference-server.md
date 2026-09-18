---
title: "LLM Inference Testbed for Performance and Agentic-Quality Analysis"
excerpt: "Single-socket EPYC workstation running frontier-class 600B+ parameter language models locally, with 2TB RAM and 128GB VRAM across four AMD Radeon Pro V620 GPUs."
collection: portfolio
category: infrastructure
weight: 41
---

![LLM inference server build showing four AMD Radeon Pro V620 GPUs and EPYC 7713 in a Jonsbo N5 chassis](/images/llm-server-build.jpg)

A single-chassis system that runs frontier-class open-weight language models — Mixture-of-Experts systems in the hundreds-of-billions-of-parameters class — locally, at interactive speeds and without cloud API dependency.

Its primary purpose is security and litigation research conducted on local, self-hosted models. Running inference in-house, with no external API dependency, keeps sensitive material — source code, forensic images, and case data — on controlled infrastructure, makes analyses reproducible, and keeps capability available during confidential investigations, with full control over the models, prompts, and system configuration used to evaluate workloads such as vulnerability analysis, code understanding, and forensic reconstruction. The system also serves as a testbed for measuring local inference performance and evaluating the agentic quality of open-weight models, and a complementary AMD Strix Halo laptop runs smaller but still capable models on the go.

The build centers on an AMD EPYC 7713 (64-core, 8-channel DDR4) with 2TB of ECC RAM and four AMD Radeon Pro V620 GPUs providing 128GB of total VRAM. The EPYC's 8-channel memory bandwidth is the critical bottleneck for Mixture of Experts inference, where active expert weights must be loaded from system RAM on every forward pass; MoE weights reside in system RAM while the GPUs handle attention layers and the KV cache. The V620s are passive datacenter cards that required custom 3D-printed fan shrouds paired with high-static-pressure server fans to cool adequately in a desktop chassis.

The measurement program built on this system is published as the [LLM Performance Engineering Notebook](https://github.com/pauldmartinphd/llm-performance-engineering-notebook), an open lab notebook of experiments in finding and raising the inference speed limits of large MoE models. It documents the methodology — measure the hard physical limit first, predict from a model, then change one variable at a time — along with a scheduler patch to llama.cpp that raised prefill throughput and is being submitted upstream, a table of refuted hypotheses, and per-model results that are re-baselined as models and builds change.

The system runs under Proxmox and shares a chassis with the storage and networking described in [Research Computing Infrastructure](/portfolio/research-computing-infrastructure/); consolidating those roles into a single box added LLM inference as an entirely new capability.
