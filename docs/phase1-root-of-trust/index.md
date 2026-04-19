# Phase 1: Root of Trust

## 1. Overview

Phase 1 defines the foundational trust anchor for Boot2Trust. This phase describes the initial hardware and firmware assumptions required to establish a secure chain of trust for an embedded Linux ECU.

The Root of Trust is the immutable starting point from which all later stages—verified boot, runtime integrity, access control, and isolation—derive their security guarantees.

## 2. Goals

- Establish the hardware/firmware trust anchor for the platform
- Define the bootloader trust model and key storage assumptions
- Clarify which components are trusted implicitly and which are measured or verified
- Prepare the platform for Phase 2: Secure Boot & Chain of Trust

## 3. Core concepts

- Hardware root of trust: a minimal trusted component that anchors cryptographic identity and measurement
- Immutable boot firmware: trusted bootloader code loaded from a protected, write-once source
- Bootloader key material: secure storage and use of verification keys or certificates
- Trust boundaries: delineate what is assumed trusted, what is measured, and what is validated later

## 4. Approach

1. Document the platform trust model and threat assumptions
2. Identify the entry point for trust in the system
3. Define how firmware and bootloader integrity are established
4. Specify the chain of custody for boot keys and signed artifacts

## 5. Automotive scenario

In an ECU-style platform, Phase 1 assumes the device boots from a trusted boot ROM or write-protected bootloader region. The platform must resist:

- firmware replacement attacks on the primary bootloader
- unauthorized modification of boot verification keys
- early-stage compromise before runtime integrity controls are active

## 6. Outcome

Phase 1 delivers a baseline trust model and secure boot assumptions for the Boot2Trust project. It establishes the foundation for Phase 2, where verified boot and cryptographic validation of firmware images are implemented.

---

👉 Proceed to Phase 2: [Secure Boot & Chain of Trust](../phase2-secure-boot/)
