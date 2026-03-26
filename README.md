# 🔐 VECTOR — IoT Risk Management Framework

> **V**ulnerability **E**limination & **C**ontrol **T**hrough **O**perational **R**emediation

Filling the protocol-layer gaps NIST, ISO, and ETSI leave unaddressed in consumer IoT — with controls that are testable, standards-aligned, and regulator-ready.

---

## 📌 Overview

The Internet of Things has transformed everyday life — but consumer IoT devices remain critically underprotected. Existing standards such as NIST SP 800-183, ISO/IEC 27001, and ETSI EN 303 645 fail to prescribe granular, testable controls at the **protocol layer**, leaving smart home systems, wearables, and health monitors exposed to a wide range of attacks.

**VECTOR** is a protocol-specific cybersecurity risk management framework designed to close these gaps. It addresses vulnerabilities within the core communication protocols used by consumer IoT devices — MQTT, Bluetooth/BLE, Zigbee/Z-Wave, NFC/RFID, and CoAP — across the full device lifecycle.

---

## 🎬 Project Presentation

📊 **[View the full VECTOR framework walkthrough on Canva](https://www.canva.com/design/DAHFDmyNa3o/gSXbexHPDbFGB0tboKStwg/view?utm_content=DAHFDmyNa3o&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=hf5b5037233)**

The presentation covers:
- The problem with existing IoT security standards
- Why a new protocol-specific framework is needed
- The VECTOR four-step design methodology
- Hands-on vulnerability assessment pipeline
- Compliance and regulatory alignment
- Impact, outcomes, and future scope

---

## 🏗️ Framework Design

VECTOR was designed as a four-step process:

```
Step 1 — Gap Analysis
        │
        Review of NIST, ISO/IEC, ETSI, DORA, and IIC frameworks
        Identify unaddressed protocol-level and data-layer gaps
        │
        ▼
Step 2 — Threat Analysis
        │
        Structured threat modelling across 6 consumer IoT protocols
        Map attack scenarios to real-world risk vectors
        │
        ▼
Step 3 — Vulnerability Assessment
        │
        Risk identification, registration and assessment
        Real-world tool-based simulation of actual attack scenarios
        │
        ▼
Step 4 — Layered Control Mapping
        │
        Controls designed across manufacturing, protocol, and data storage phases
        Aligned to NIS2, ISO/IEC 27030, and the EU Cyber Resilience Act
```

---

## 🌐 Protocols Covered

| Protocol | Key Vulnerabilities Addressed |
|---|---|
| MQTT | Lack of TLS enforcement, broker authentication weaknesses |
| Bluetooth / BLE | Absence of mutual authentication, pairing vulnerabilities |
| Zigbee / Z-Wave | Weak key management, replay attack exposure |
| NFC / RFID | Cryptographic weaknesses, device cloning risks |
| CoAP | Plaintext transmission, DoS amplification vectors |
| Wi-Fi | Insecure firmware update channels, legacy protocol exposure |

---

## 🔍 Vulnerability Assessment Pipeline

Hands-on validation was conducted using a suite of real-world security tools:

| Tool | Purpose |
|---|---|
| **Binwalk** | Firmware extraction and analysis — hardcoded credentials, backdoors |
| **QEMU** | Firmware emulation for dynamic testing |
| **Bettercap** | MitM simulation and protocol traffic capture |
| **Hydra** | Brute-force simulation to test authentication strength |
| **OpenSSL** | TLS/SSL configuration testing — TLS 1.3 and forward secrecy validation |
| **Zigbee Sniffers** | Capture of unsecured Zigbee/Z-Wave traffic patterns |

---

## 🛡️ Attack Scenarios Simulated

- Man-in-the-Middle (MitM) attacks across BLE and Zigbee
- Replay attacks on NFC/RFID communication channels
- Command hijacking via unsecured MQTT broker sessions
- Denial-of-Service (DoS) via CoAP amplification
- Device cloning through weak NFC cryptographic schemes
- Malicious firmware injection via insecure OTA update channels
- Brute-force credential attacks on default authentication

---

## 📋 Compliance Alignment

VECTOR maps controls to the following regulatory and standards frameworks:

| Standard | Coverage |
|---|---|
| NIS2 Directive | Network and information security obligations for IoT manufacturers |
| GDPR | Data protection controls for consumer IoT data handling |
| EU Cyber Resilience Act | Secure-by-design requirements for connected products |
| ISO/IEC 27030 | IoT-specific security guidelines |
| NIST SP 800-183 | IoT ecosystem risk assessment |
| NIST SP 800-53 | Security and privacy controls |
| ETSI EN 303 645 | Consumer IoT baseline security requirements |

---

## 📖 Published Work

This framework was accepted for publication in the University of Galway Open Press:

> Parija, N., Padyal, V., and Hiremath, S. (2025) *Securing the Smart Future: An IoT Risk Management Framework*, Chapter 1, in *Perspectives on Cybersecurity Risk Management Vol 1*, University of Galway Open Press, Ireland, ISBN 978-1-911690-20-7.
>
> 🔗 [Read the full paper](https://openpress.universityofgalway.ie/perspectivesoncybersecurityriskmanagementvol1/)

---

## 🔮 Future Scope

- **AI-assisted anomaly detection** — Integrating ML-based threat detection at the protocol layer
- **Industrial IoT extension** — Adapting VECTOR controls for IIoT and OT environments
- **Automated compliance checker** — A tool to assess IoT device configurations against VECTOR controls
- **Secure boot enforcement** — Expanding firmware integrity validation across more device classes
- **MITRE ATT&CK for ICS mapping** — Aligning VECTOR threat scenarios to ATT&CK for ICS TTPs

---

## ⚠️ Disclaimer

This project was developed for **academic and research purposes** as part of the MSc in Cybersecurity at the University of Galway (2024–25). All vulnerability assessments were conducted in controlled, isolated lab environments on devices owned by the research group.

---

## 👩‍💻 Authors

**Nishita Sunil Parija** · **Vedangi Vilas Padyal** · **Sanjana Hiremath**
MSc Cybersecurity — University of Galway (2024–25)

[LinkedIn — Nishita Parija](https://www.linkedin.com/in/nishitaparija) · [GitHub](https://github.com/nishitaparija)

---
