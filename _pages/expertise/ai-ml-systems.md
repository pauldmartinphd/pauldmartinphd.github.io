---
layout: archive
title: "Artificial Intelligence & Machine Learning Systems"
permalink: /expertise/ai-ml-systems/
description: "Paul D. Martin, Ph.D. on his experience with artificial-intelligence and machine-learning systems, from source-code analysis and LLM security to local inference performance research."
author_profile: true
---

I have experience with artificial-intelligence and machine-learning systems through expert-witness engagements, source-code analysis, research, teaching, and development of computing infrastructure for local model execution. My work includes examining machine-learning implementations and AI integration software, investigating large-language-model security, and measuring and optimizing inference performance.

In my expert-witness practice, I have analyzed audience-measurement and identification systems incorporating machine learning. This work included source-code review, analysis of the implemented technology, preparation of expert reports, and testimony at deposition and trial. In related work involving audience-measurement and audio-fingerprinting systems, I performed source-code and algorithm analysis, developed simulations, and testified at trial.

My source-code analysis also extends to the software connecting AI systems with external tools and services. I have evaluated the source code of at least ten Model Context Protocol (MCP) servers. This work complements my broader experience examining software implementations and the behavior of systems composed of interacting components. In 2026, I developed a module on large-language-model security for my teaching at Johns Hopkins University.

I designed and built a [local inference system](/portfolio/6-llm-inference-server/) for running large open-weight language models, including mixture-of-experts models containing hundreds of billions of parameters. The system combines an AMD EPYC processor, two terabytes of system memory, and four GPUs providing an aggregate 128 gigabytes of video memory. I integrated the processing, memory, virtualization, and cooling components into a working platform for research and technical analysis.

My inference research examines how model architecture, quantization, memory bandwidth, CPU and GPU allocation, and execution scheduling affect performance. I have investigated configurations in which routed expert weights reside in system memory while other model components and the key-value cache reside on GPUs. My work distinguishes the processing of an input prompt from the subsequent generation of output tokens, because these phases can encounter different computational and data-transfer bottlenecks.

I have developed and tested performance models relating token-generation time to the amount of model data accessed, measured memory bandwidth, and other execution overhead. I have also investigated how prompt length and processing-batch size affect performance. These analyses combine direct hardware measurements with examination of inference software and controlled experiments, allowing me to compare predicted limits with observed behavior and investigate discrepancies.

My work has included identifying and modifying scheduling behavior in llama.cpp that limited prompt-processing performance. The changes distributed offloaded computations across multiple GPUs and removed an unnecessary transfer of expert-selection information during prompt processing. I tested the changes by examining execution scheduling as well as throughput. I have also investigated speculative decoding, including the effects of draft length and verification costs on performance in systems combining CPU and GPU execution.

I maintain a [public lab notebook](https://github.com/pauldmartinphd/llm-performance-engineering-notebook) documenting these investigations, including experimental methods, hardware configurations, software builds, model files, raw measurements, software changes, and hypotheses that testing did not support. My work has also identified benchmarking pitfalls, including settings that changed the effective processing-batch size and differences in configuration handling between tools. I have repeated measurements under common conditions to distinguish the effects of software updates, hardware changes, and optimization techniques, and I distinguish results specific to a tested configuration from methods applicable to other systems.

My broader research includes evaluating large language models for technical research and analysis, including vulnerability analysis, code understanding, and forensic reconstruction. I also use my infrastructure to evaluate models' ability to perform tasks through sequences of tool use and other actions. Running models locally allows me to retain control over sensitive materials and the models, prompts, and system configurations used in an investigation. My research additionally includes the use of multimodal large language models to investigate disease progression.

This work builds on my experience with operating systems, virtualization, software development, and experimental testing. I design and operate the [infrastructure](/portfolio/research-computing-infrastructure/) supporting these investigations, including storage, hardware access, and segmented networking, and operate a Proxmox cluster at home for AI agent swarms. I also developed and launched [Technicomp Benchtop Linux](/portfolio/5-technicomp-workbench/), a Linux distribution whose target applications include machine learning and data science.

---

[&larr; Expert witness experience](/expert-witness/) &middot; [Testimony record](/expert-witness/#testimony) &middot; [Download CV (PDF)](/files/PaulMartin-CV.pdf)
