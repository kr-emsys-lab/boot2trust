# Boot2Trust – Embedded Linux Security Lab

**[GitHub Repository](https://github.com/kr-emsys-lab/boot2trust)** | **[Project Website (GitHub Pages)](https://kr-emsys-lab.github.io/boot2trust/)**

Boot2Trust is a hands-on project demonstrating **end-to-end security in embedded Linux systems**, inspired by automotive ECU architectures.

The focus is on building a **chain of trust** from bootloader to application isolation, with practical experiments showing both **secure behavior and failure cases**.

---

## 🔧 Tech Stack

- QEMU (ARM64)
- U-Boot (Verified Boot)
- Buildroot
- dm-verity, IMA
- SELinux
- Linux namespaces, cgroups, LXC

---

## 📚 Project Phases

1. Secure Boot & Chain of Trust  
2. Runtime Integrity  
3. Access Control  
4. Isolation  
5. Root of Trust (conceptual)  
6. Platform Comparison (Linux vs QNX / AAOS / AGL)

---

## 🚗 Real-World Focus

Each phase includes:
- Automotive attack scenario (e.g., firmware tampering, malicious devices)
- Implementation and validation
- Logs showing system response (success vs failure)

---

## 🛡️ Compliance Alignment

The project maps key mechanisms to:
- Cyber Resilience Act (CRA)
- ISO/SAE 21434

This is not a certified system, but a **practical demonstration of security principles aligned with industry expectations**.

---

## 🎯 Goal

To demonstrate system-level expertise in:
- Embedded Linux security
- Platform architecture
- Automotive-grade software integrity

---

## 🌐 Viewing the Project Documentation

The documentation for this project is hosted on GitHub Pages. You can view the live site here: **[Boot2Trust Project Website](https://kr-emsys-lab.github.io/boot2trust/)**

### Local Development (Docker)

To view and run the GitHub Pages site locally using Docker, without needing Ruby installed on your host:

1. Serve the site locally:
   ```bash
   docker run --rm -v "$PWD:/srv/jekyll" -p 4000:4000 jekyll/jekyll jekyll serve
   ```
2. Open your web browser and navigate to `http://127.0.0.1:4000/boot2trust/`

---

👉 Start here: `docs/phase1-secure-boot/`
