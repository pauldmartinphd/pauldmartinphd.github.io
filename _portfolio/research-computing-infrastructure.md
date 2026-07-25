---
title: "Research Computing Infrastructure"
excerpt: "Design and operation of self-hosted virtualization, storage, compute, and network infrastructure supporting security research, AI inference, and expert analysis."
collection: portfolio
category: infrastructure
weight: 43
---

<img src="/images/homelab-rack.jpg" alt="Server rack with virtualization host, hot-swap drive bays, and CyberPower UPS" style="max-height: 520px; border-radius: 4px;" />

Dr. Martin designs, builds, and operates the self-hosted computing infrastructure behind his security research, AI inference, and expert witness work. Its purpose is to provide isolated, reproducible environments in which confidential code and case data can be analyzed under his own control, and the capacity to run compute-intensive analysis at scale — rapid provisioning of segmented, multi-OS test networks; controlled handling of sensitive material; and repeatable experiments.

The environment runs on Proxmox with PCIe passthrough for dedicated firewall (OPNsense) and storage (TrueNAS) virtual machines, consolidating what was previously a rack of separate appliances into a single chassis. Supporting systems include high-capacity ZFS storage with end-to-end data-integrity verification, snapshots, and replication; distributed compute clusters; and custom OpenBSD and OPNsense network appliances providing deep packet inspection, traffic shaping, and segmentation.
