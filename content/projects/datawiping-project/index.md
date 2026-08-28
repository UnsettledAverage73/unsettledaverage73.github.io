---
title: "Secure Data Wiping Utility"
summary: "Low-level system utility for secure, unrecoverable data erasure adhering to sanitization standards."
tags:
  - Systems
  - Security
date: 2025-05-01
external_link: ""
---

* **Storage Sanitization:** Implemented multi-pass overwrite patterns (zero-fill, pseudo-random data) directly targeting block storage devices.
* **Kernel & Storage Interaction:** Interfaced with Linux storage APIs to overwrite master boot records (MBR) and partition tables safely.
