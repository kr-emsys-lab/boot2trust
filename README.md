# Boot2Trust – Embedded Linux Security Lab

Boot2Trust is a hands-on, phase-driven project demonstrating **end-to-end security in embedded Linux systems**, inspired by automotive ECU architectures.

The project focuses on building and validating a **chain of trust from bootloader to application isolation**, with reproducible experiments and attack scenarios showing secure behavior and failure cases.

---

## 🔧 Tech Stack

- QEMU (ARM64)
- U-Boot (Verified Boot)
- Buildroot
- dm-verity
- IMA
- SELinux
- Linux namespaces, cgroups, LXC

---

## 📚 Project Phases

1. Root of Trust (Phase 1)
2. Secure Boot & Chain of Trust (Phase 2)
3. Runtime Integrity
4. Access Control
5. Isolation
6. Platform Comparison (Linux vs QNX / AAOS / AGL)

---

## 🚗 Real-World Focus

Each phase includes:
- Problem definition from an automotive or embedded scenario
- Architecture overview
- Implementation code and configuration
- Attack simulation (tampering / misuse)
- Observed system behavior and logs
- Regulatory mapping

---

## 🛡️ Compliance Alignment

The project maps key mechanisms to:
- Cyber Resilience Act (CRA)
- ISO/SAE 21434

This is not a certified system, but a **portfolio-grade demonstration of security engineering aligned with industry expectations**.

---

## 🎯 Goal

To demonstrate system-level expertise in:
- Embedded Linux platform security
- Automotive cybersecurity
- System integration and platform bring-up

---

## 🌐 Viewing the Project Documentation

The documentation for this project is hosted on GitHub Pages. You can view the live site here: **[Boot2Trust Project Website](https://kr-emsys-lab.github.io/boot2trust/)**

### Local Development (Docker)

To view and run the GitHub Pages site locally with Docker:

```bash
docker run --rm -v "$PWD:/srv/jekyll" -p 4000:4000 jekyll/jekyll jekyll serve
```

Then open `http://127.0.0.1:4000/boot2trust/`.

---

👉 Start here: `docs/phase1-root-of-trust/`
