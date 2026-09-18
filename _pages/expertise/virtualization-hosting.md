---
layout: archive
title: "Virtualization, Containerization & Hosting Infrastructure"
permalink: /expertise/virtualization-hosting/
description: "Paul D. Martin, Ph.D. on his experience with virtualization, containerization, cloud computing, distributed processing, and the infrastructure underlying hosted applications."
author_profile: true
---

I have substantial experience with virtualization, containerization, cloud computing, distributed processing, and the infrastructure underlying hosted applications. My work includes designing and operating computing environments, developing systems that use virtualization, assessing their security, and analyzing their implementation in litigation. I use these technologies in my commercial work, research, and teaching.

Early in my career, I performed a security assessment and wide-scale penetration test of virtualized cloud-based research systems using Amazon EC2 and VMware infrastructure, including penetration testing of VMware ESXi. The systems were intended to provide secure environments for researchers working with confidential information. I developed a formal threat model addressing potential attack vectors, conducted testing, and prepared reports documenting the results.

At Independent Security Evaluators, I built an [automated system](/portfolio/ise-malware-automation/) capable of testing antivirus products against thousands of malware samples for Consumer Reports' annual antivirus analysis. I managed the VMware ESXi server on which the system operated. The system automated testing in Windows virtual machines, including snapshot creation and restoration, to provide repeatable conditions and return environments to a known state between tests. My research at Johns Hopkins University also included generating virtualized computer networks for malware education.

My infrastructure experience includes building a Proxmox cluster for my laboratory at Johns Hopkins University and operating a Proxmox cluster at home for AI agent swarms. These projects involve building and operating clusters as well as individual virtual machines and containers. My courses also use virtualized and emulated environments to give students hands-on experience with different operating systems, software configurations, and security problems.

I served as the technical and development lead for [Firmware IQ](/portfolio/4-firmware-iq/), a commercial security-analysis platform that examines firmware, container images, and virtual-machine appliances. The platform accepts images through a web-based portal, forwards them through a broker to an analysis engine, unpacks them into their constituent components, and performs automated security checks. Results are returned through JSON to a web-based presentation system. My research has also included automated vulnerability analysis of containers and virtual appliances.

I currently design, build, and operate the [virtualization, storage, compute, and network infrastructure](/portfolio/research-computing-infrastructure/) supporting my security research, AI inference, and expert-witness work. This infrastructure allows me to provision isolated environments across multiple operating systems, examine confidential software and forensic material under my control, and conduct experiments that can be repeated with known configurations.

My infrastructure includes Proxmox virtualization, virtual machines, and LXC containers. I use PCIe passthrough to give dedicated virtual machines direct access to physical hardware, including network interfaces assigned to an OPNsense firewall and disk controllers assigned to a TrueNAS storage system. My storage environment uses ZFS with integrity checking, snapshots, and replication. I also build and operate OpenBSD and OPNsense network appliances supporting traffic inspection, traffic shaping, and network segmentation, including isolated environments for examining malware and suspect firmware.

I have integrated substantial AI workloads into this infrastructure. My [local language-model inference environment](/portfolio/6-llm-inference-server/) runs llama.cpp with AMD's ROCm software in an LXC container on Proxmox and uses multiple GPUs together with large amounts of system memory. Building and operating this environment has required coordinating container configuration, access to computing hardware, memory resources, and the software dependencies required for model execution. I use it for inference experiments and technical research involving large open-weight models.

My distributed-computing experience includes developing a Hadoop-based application for large-scale statistical analysis of electronic-medical-record audit logs, together with a web application for presenting the results. My operating-system development work also includes creating Linux distributions and associated build systems. I developed and launched [Technicomp Benchtop Linux](/portfolio/5-technicomp-workbench/), whose intended applications include virtualization, system administration, and software development.

In my expert-witness and consulting practice, I have analyzed emulation and virtualization technologies, virtualization-based security and automated corruption-repair systems, browser sandboxing and process isolation, and cloud-based applications. My engagements have included cloud-based vehicle-management and security systems, cloud-based content aggregation and streaming, and content-delivery networks. This work has involved source-code review, technical analysis supporting claim construction, infringement and non-infringement analysis, validity analysis, preparation of reports and declarations, and deposition testimony. More broadly, the large-scale source-code reviews I have led have included virtualization platforms and numerous web-based enterprise systems.

---

[&larr; Expert witness experience](/expert-witness/) &middot; [Testimony record](/expert-witness/#testimony) &middot; [Download CV (PDF)](/files/PaulMartin-CV.pdf)
