---
title: "Research Computing Infrastructure"
excerpt: "Design and operation of self-hosted virtualization, storage, compute, and network infrastructure supporting security research, AI inference, and expert analysis."
collection: portfolio
category: infrastructure
weight: 43
---

Dr. Martin designs, builds, and operates the self-hosted computing infrastructure behind his security research, AI inference, and expert witness work. Its purpose is twofold: to provide isolated, reproducible environments in which confidential code and case data can be analyzed entirely under his own control, and to supply the capacity to run compute-intensive analysis at scale. In practice that means rapid provisioning of segmented, multi-OS test networks; controlled handling of sensitive material; and experiments that can be torn down and repeated exactly.

<figure style="margin: 20px 0;">
  <img src="/images/homelab-rack.jpg" alt="Server rack with virtualization host, hot-swap drive bays, and CyberPower UPS" style="width: auto; max-width: 100%; max-height: 480px; border-radius: 4px;" />
  <figcaption>The mobile rack: virtualization host with hot-swap storage bays, KVM, and battery-backed power.</figcaption>
</figure>

## Consolidated virtualization platform

The environment runs on Proxmox, using PCIe passthrough to give dedicated virtual machines direct control of physical hardware — a firewall VM (OPNsense) owns its network interfaces, and a storage VM (TrueNAS) owns its disk controllers. This consolidates what was previously a rack of separate physical appliances into a single chassis without giving up the isolation or performance of dedicated hardware. The same consolidation is what made room for new capability: the platform shares a chassis with the [LLM inference testbed](/portfolio/6-llm-inference-server/) used for local analysis of frontier-class language models.

## Storage and data integrity

Primary storage is high-capacity ZFS with end-to-end data-integrity verification, snapshots, and replication. Checksumming at every layer means silent corruption is detected rather than propagated — a property that matters when the data at rest includes forensic images and case material that must remain demonstrably intact. Hot-swap drive cages keep pool maintenance and capacity changes routine.

<figure style="margin: 20px 0;">
  <img src="/images/server-build-interior.jpg" alt="Server chassis interior showing Noctua CPU cooler, Corsair RM850x power supply, Intel Arc Pro GPU, and dual hot-swap drive cages with routed SATA cabling" style="width: auto; max-width: 100%; max-height: 480px; border-radius: 4px;" />
  <figcaption>Inside a storage and virtualization host: dual hot-swap drive cages with individually routed and labeled SATA runs, Noctua cooling, and an Intel Arc Pro GPU.</figcaption>
</figure>

## Network segmentation and test networks

Custom-built OpenBSD and OPNsense network appliances provide deep packet inspection, traffic shaping, and segmentation. Segmentation is what turns the infrastructure into a research instrument: suspect firmware, malware samples, and multi-OS test environments run on isolated network segments that can be created for an investigation and destroyed when it ends, with sensitive material never crossing onto general-purpose networks.

## Availability

The rack runs on conditioned, battery-backed power, and storage replication provides recovery points for the systems and data behind active casework — capability stays available, under Dr. Martin's control, for the duration of a confidential investigation.
