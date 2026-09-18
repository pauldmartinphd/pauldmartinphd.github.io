---
title: "Firmware IQ"
excerpt: "Commercial security analysis platform that scans firmware, containers, and virtual machine images for known vulnerabilities and cryptographic implementation flaws, with automated CVE cross-referencing against NIST's National Vulnerability Database."
collection: portfolio
category: embedded
weight: 22
---

Firmware IQ is a commercial security analysis platform Dr. Martin designed and led development of at Harbor Labs. Customers use the system to assess the security posture of embedded device firmware, container images, and virtual machine appliances before deployment.

The platform accepts images through a web-based portal, forwards them through a broker to an analysis engine that unpacks them into constituent components and performs over 100 automated security checks, and returns results to a web-based presentation system. It supports two distinct investigations: examining firmware updates for security issues before deployment, and examining firmware extracted from devices for indicators of compromise. These include identification of known vulnerable software components cross-referenced against NIST's National Vulnerability Database, detection of insecure configurations and hardcoded credentials, and auditing of cryptographic implementations to identify flaws in how cryptographic algorithms are deployed — weak key generation, improper use of initialization vectors, use of deprecated ciphers, and similar implementation-level issues that are distinct from algorithmic weaknesses.

The engine handles a wide range of firmware formats from different embedded device manufacturers as well as container and virtual machine image formats, enabling organizations to scan their entire deployment infrastructure for known vulnerabilities and cryptographic weaknesses at scale.

The component-identification technique at the core of the platform, which identifies software components and versions from binaries and cross-references them against a vulnerability database, is patented as [US 10,762,214 B1](https://patents.google.com/patent/US10762214B1/), with Dr. Martin as the named inventor.

[Learn more at Harbor Labs](https://harborlabs.com/regulatory-support/persistent-vulnerability-monitoring/)
