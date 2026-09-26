---
title: "Technicomp Benchtop Linux"
excerpt: "The operating system for the technical workbench: an immutable, stabilized workstation rolling release derived from openSUSE Tumbleweed and MicroOS, in alpha since 2026."
collection: portfolio
category: infrastructure
weight: 40
featured: true
---

Technicomp Benchtop Linux is a Linux distribution that Dr. Martin designed, built, and released in alpha in 2026. It is the operating system for the technical workbench: an immutable, stabilized workstation rolling release derived from openSUSE Tumbleweed and MicroOS, for x86 and ARM.

Most of the system follows Tumbleweed and stays current, while the kernel and desktop move more cautiously: an LTS kernel by default, with a current kernel for hardware enablement, and the previous upstream-supported GNOME release, which still receives upstream bug and security fixes. Every update is a snapshot that can be rolled back. Both kernels are patched for hardware support, and the system is tuned for low interactive latency so that the desktop remains responsive under heavy load. Applications come from Flatpak and command-line tools from Homebrew, both managed per user.

Benchtop Linux is configured for security analysis, reverse engineering, virtualization, software development, system administration, and AI work without additional setup.

Dr. Martin is separately researching whether its release model also improves security compared with conventional stable distributions, whose incomplete backports can let a package's real vulnerability exposure diverge from its upstream version.

The project is developed and released through [Technicomp Labs](https://technicomplabs.io/benchtop/), with source and packaging on [GitHub](https://github.com/TechnicompLabs).
