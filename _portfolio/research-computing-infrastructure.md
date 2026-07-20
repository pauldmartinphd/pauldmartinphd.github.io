---
title: "Research Computing Infrastructure"
excerpt: "Design and operation of self-hosted virtualization, storage, compute, and network infrastructure supporting security research, AI inference, and expert analysis."
collection: portfolio
category: infrastructure
weight: 43
---

<img src="/images/homelab-rack.jpg" alt="Server rack with virtualization host, hot-swap drive bays, and CyberPower UPS" style="max-height: 520px; border-radius: 4px;" />

Dr. Martin designs, builds, and operates the self-hosted computing infrastructure that supports his security research, AI inference, and expert witness work. Current infrastructure runs on Proxmox with PCIe passthrough for dedicated firewall (OPNsense) and storage (TrueNAS) virtual machines, consolidating what was previously a full rack of separate appliances into a single chassis; earlier generations ran VMware ESXi on Dell PowerEdge hardware. The environment supports rapid provisioning of isolated, multi-OS test networks and compute-intensive workloads.

Supporting systems include high-capacity ZFS storage appliances (100+ TB, built from enterprise and custom hardware) providing network-attached storage, backup, and snapshot and replication with end-to-end data-integrity verification; distributed compute clusters, including a cross-architecture Hadoop cluster built on PowerPC hardware; and custom network security appliances built on OpenBSD and OPNsense, with deep packet inspection, traffic shaping, and network segmentation.
