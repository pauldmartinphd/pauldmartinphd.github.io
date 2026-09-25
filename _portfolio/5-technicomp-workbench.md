---
title: "Technicomp Benchtop Linux"
excerpt: "The operating system for the technical workbench: an immutable GNOME desktop with an LTS core, released in alpha in 2026."
collection: portfolio
category: infrastructure
weight: 40
featured: true
---

Technicomp Benchtop Linux is a Linux distribution that Dr. Martin designed, built, and released in alpha in 2026. It is the operating system for the technical workbench: an immutable GNOME desktop for x86 and ARM workstations, built on openSUSE Tumbleweed and MicroOS.

Even though the system uses a rolling release model, its core packages track LTS releases and its desktop is GNOME Oldstable, so the system stays stable while security fixes arrive promptly. Every update is a snapshot that can be rolled back. The distribution ships LTS and Current kernels, both patched for hardware support, and is tuned for low interactive latency so that the desktop remains responsive under heavy load. Applications come from Flatpak and command-line tools from Homebrew, both managed per user.

Benchtop Linux is configured for security analysis, reverse engineering, virtualization, software development, system administration, and AI work without additional setup.

Dr. Martin is separately researching whether its release model also improves security compared with conventional stable distributions, whose incomplete backports can let a package's real vulnerability exposure diverge from its upstream version.

The project is developed and released through [Technicomp Labs](https://technicomplabs.io/benchtop/), with source and packaging on [GitHub](https://github.com/TechnicompLabs).
