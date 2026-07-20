---
layout: archive
title: "Expert Witness Experience"
permalink: /expert-witness/
description: "Software and cybersecurity expert witness Paul D. Martin, Ph.D.: source code review, reverse engineering, embedded and medical device security across 100+ litigation matters."
author_profile: true
---

Dr. Martin serves as both a testifying and consulting expert in complex litigation involving software systems, cybersecurity, artificial intelligence, embedded devices, and computer architecture. His work frequently involves large-scale source code review, reverse engineering of complex systems, analysis of embedded firmware, and the explanation of computing systems and technical evidence to judges and juries.

He has served as a testifying or consulting expert in over 100 matters across federal and state courts, the International Trade Commission, inter partes reviews before the Patent Trial and Appeal Board, criminal proceedings, and international regulatory actions. Unlike many experts whose experience is limited to analysis, Dr. Martin has written production code deployed in FDA-regulated medical devices, identified remote code execution vulnerabilities in life-critical medical systems, and designed cryptographic protocols implemented in production healthcare environments. He is a current member of the IEEE 7024 Working Group on the "Standard for the Procurement, Verification and Validation, and Life Cycle Management of Forensic Technologies." He designs and conducts custom experiments tailored to the specific technical questions at issue and regularly works cases where source code is incomplete or unavailable through binary reverse engineering and forensic reconstruction.

Dr. Martin serves as Chief Scientist at **[Harbor Experts](https://harborexperts.com)**, through which he accepts expert witness and consulting engagements.

---

## Areas of Expertise

**Software, Source Code & Intellectual Property Analysis**
Dr. Martin has led over 100 large-scale source code reviews in litigation, spanning systems from thousands to billions of lines of code. This work covers trade secret misappropriation, copyright infringement, breach of contract, and code-quality disputes, and includes manual review, automated comparison, architectural analysis, development-timeline reconstruction, and identification of exploitable vulnerabilities. He has authored whitepapers on [source code comparison](/files/HL-WP-SourceCodeComparison.pdf), [source code quality assessment](/files/HL-WP-SourceCodeQuality.pdf), and [source code review in litigation](/files/HL-WP-SourceCodeReview.pdf).

**Reverse Engineering, Malware & Digital Forensics**
Disassembly, decompilation, and forensic reconstruction of software behavior when source code is unavailable, lost, or destroyed — including firmware extraction, binary diffing, and work with tools such as Ghidra and IDA Pro. This area encompasses static and dynamic malware analysis and the attribution of intrusions and code to the actors responsible, including nation-state activity; forensic examination of computers and mobile devices across iOS and Android; reconstruction of system and user activity from logs and execution artifacts; and assessment of the reliability and validity of forensic software, including the computerized DNA-analysis software scrutinized in criminal proceedings. Dr. Martin is a member of the IEEE 7024 Working Group on the verification, validation, and life-cycle management of forensic technologies.

**Cybersecurity, Cryptography & Network Security**
Analysis of cryptographic implementations (elliptic curve cryptography, random number generation, key management, TLS/SSL, DRM, and authentication protocols), network security infrastructure (firewalls, IPS, VPNs, content delivery networks, and wireless handoff protocols), and endpoint security products (malware-scanning gateways, URL filtering, and anti-phishing technologies) — covering both correctness of implementation and conformance to standards such as NIST and IEEE.

**Embedded, Hardware & Medical Device Systems**
Security analysis of firmware, microcontrollers, hardware security modules, trusted execution environments (TEEs), and hardware-software interfaces, including BIOS/UEFI analysis, SPI and JTAG interfaces, fTPM implementations, control-flow-integrity mechanisms, and software update mechanisms. It extends to medical devices, patient-data systems, and healthcare computing infrastructure: Dr. Martin's doctoral research focused on securing medical devices, and he has written production code deployed in FDA-regulated medical devices, identified remote code execution vulnerabilities in life-critical infusion pump systems, and designed cryptographic protocols implemented in production healthcare environments.

**Artificial Intelligence, Virtualization & Computing Infrastructure**
Analysis of AI and large language model systems — model hosting infrastructure, inference performance, GPU and memory architecture for model serving, quantization and optimization, training and fine-tuning pipelines, and the security properties of AI systems — together with the virtualization, containerization, and cloud hosting platforms on which they run. Includes hypervisor and container-orchestration analysis, VM and container image forensics, PCIe passthrough and hardware isolation, and storage virtualization.

**Performance Analysis & Experimental Testing**
Measurement, quantification, and tuning of hardware and network system performance across CPU, memory, GPU, storage, and network subsystems — including benchmarking methodology, bottleneck identification, and performance-regression analysis — and the design and execution of custom experiments and system reconstructions built to answer the specific technical questions in dispute. Draws on more than twenty years of hands-on performance engineering across embedded systems, datacenter infrastructure, and consumer devices.

---

## Representative Analyses & Methods

Dr. Martin's engagements typically involve:

- Large-scale source code review and automated and manual comparison across systems ranging from thousands to billions of lines of code, in trade secret, copyright, contract, and code-quality disputes
- Reverse engineering and forensic reconstruction of software behavior from binaries, firmware, execution traces, and logs when source code is unavailable
- Firmware extraction and embedded-system analysis, including boot chains and update mechanisms, using interfaces such as SPI and JTAG
- Malware analysis and cyber-attribution, including large-scale automated sample analysis and evaluation of the reasonableness of an organization's security measures
- Analysis of cryptographic implementations, network and endpoint security products, and conformance to applicable standards
- Design and execution of custom experiments — including performance measurement and benchmarking of CPU, GPU, memory, storage, and network subsystems — to answer specific technical questions in dispute
- Clear technical explanation of complex computing systems to judges and juries in depositions, hearings, and at trial

---

## Teaching & Communication

Dr. Martin teaches C/C++ programming, computer security, and applied cryptography in the Department of Computer Science at Johns Hopkins University, where his security courses require students to read through real codebases, identify exploitable vulnerabilities, and write working exploits — the same analytical discipline he applies in litigation source code review. That experience translates directly to expert testimony, where complex technical concepts must be communicated clearly to judges and juries who may have no prior technical background.

---

## Testimony

Dr. Martin has provided expert testimony eighteen times — at trial, in evidentiary hearings, and at deposition — in the following matters:

**The Nielsen Company v. TVision**
Case No. 25-575-CJB
*Audience measurement and identification systems and audio fingerprinting.*
Services: Source code review, expert report drafting, algorithm analysis and simulations.
Testimony: Trial — Wilmington, DE (June 8–9, 2026)

**Certain Flash-Spun Nonwoven Materials and Products Containing Same**
ITC Investigation No. 337-TA-1424
*Nation-state threat actors, unfair competition, and trade secret misappropriation.*
Services: Malware analysis and reverse engineering, cyber-attribution, computer forensics, reasonableness of security measures.
Testimony: Trial — Washington, DC (January 29, 2026); Deposition — Washington, DC (September 6, 2025)

**Malikie Innovations Ltd., Key Patent Innovations Ltd. v. MARA Holdings, Inc.**
Case No. 7:25-cv-00222-DC-DTG
*Cryptography, elliptic curve cryptography, random number generation, and cryptocurrencies.*
Services: Source code review, expert report drafting, validity analysis.
Testimony: Deposition — Potomac, MD (January 22, 2026)

**Twitch Interactive, Inc. v. Razdog Holdings LLC**
IPR2025-03017
*Cloud-based content aggregation and streaming.*
Services: Invalidity analysis, IPR drafting.
Testimony: Deposition — Washington, DC (October 10, 2025)

**The Nielsen Company v. Hyphametrics, Inc.**
Case No. 23-136-GBW-CJB
*Audience measurement and identification systems and machine learning systems.*
Services: Source code review, expert report drafting, validity analysis.
Testimony: Trial — Wilmington, DE (July 24–25, 2025); Deposition — Potomac, MD (February 5, 2025)

**Jonathan Day and Michelle Dobek v. Advanced Micro Devices, Inc.**
Case No. 3:22-cv-04305
*Computer fTPM and TEE design characteristics.*
Services: Technical analysis and expert reports on the security and performance characteristics of trusted execution environments and the design of NVRAM interfaces through SPI.
Testimony: Deposition — Washington, DC (February 7, 2025)

**State of New Jersey v. Paul Caneiro**
Indictment No. 19-02-283
*Reliability of specific types of computerized DNA analysis in criminal proceedings.*
Services: Source code review, expert report drafting.
Testimony: Evidentiary Hearing — Freehold, NJ (December 6, 2024)

**LoganTree v. Fossil**
Case No. 21-cv-0385-JDW
*Fitness-tracking wearables.*
Services: Technical analysis and expert reports on validity and infringement.
Testimony: Deposition — Monrovia, MD (August 11, 2023)

**ISI v. Intuitive Surgical, Inc.**
Case No. 3:21-cv-03496-VC
*Cryptographic security protections.*
Services: Technical analysis and expert reports on security and technical aspects of surgical devices.
Testimony: Deposition — Monrovia, MD (March 16, 2023)

**United States v. Laffon Ellis**
Case No. 2:19-cr-00369-DWA
*Reliability of specific types of computerized DNA analysis in criminal proceedings.*
Services: Source code review, expert report drafting.
Testimony: Evidentiary Hearing — Monrovia, MD (December 20, 2021)

**Sysmex Corporation and Sysmex America, Inc. v. Beckman Coulter, Inc.**
Case No. 19-1642-RGA-CJB
*Hematology analysis machine patents.*
Services: Source code review, expert report drafting.
Testimony: Deposition — Monrovia, MD (November 22, 2021)

**Certain Routers, Access Points, Controllers, Network Management Devices, Other Networking Products, and Hardware and Software Components Thereof**
ITC Investigation No. 337-TA-1227
*Patents on wireless network handoff, network management, and QoS technologies.*
Services: Source code review, validity and prior art analysis, expert report drafting.
Testimony: Trial — Washington, DC (July 28, 2021); Deposition — Monrovia, MD (June 9–10, 2021)

**Micro Focus, Inc. v. Insurance Services Organization**
DE Civil Action No. 15-252-RGA
*Unlicensed use of runtime environments, libraries, and software compilers.*
Services: Source code review, binary reverse engineering and analysis, affidavit drafting, expert report drafting.
Testimony: Deposition — Wilmington, DE (February 2, 2021)

**loanDepot.com, LLC v. Sigma Infosolutions, Inc.**
AAA Case No. 01-18-0001-5821
*Software development practices.*
Services: Source code analysis, experimentation, report drafting.
Testimony: Deposition — Baltimore, MD (December 17, 2019)

**Cypress Lake Software, Inc. v. Samsung Electronics America and Dell, Inc.**
Case No. 6:18-cv-00030-RWS
*Infringement of UX patents.*
Services: Source code analysis, report drafting.
Testimony: Deposition — Baltimore, MD (July 9, 2019)

---

The matters above reflect Dr. Martin's testimony record. He has been retained as a testifying or consulting expert in over 100 matters in total.

[View the full engagement record &mdash; reports, declarations, and consulting matters &rarr;](/expert-witness/engagements/)
