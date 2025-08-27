---
draft: true
description:
socialDescription:
title: IEC 60601 ChatGPT Notes
tags:
  - highlight/llm
date: 2025-05-18
modified: 2025-08-21
---
about [[IEC 60601]]
### **Design Priorities**
- **Patient safety is #1** – insulation, leakage current, isolation.
- **Reliability and robustness** – redundancy where needed.
- **Traceability** – documentation for every design decision.
- **Long lifecycle** – components and designs must be maintainable over 10+ years.
- **Risk management** – follow ISO 14971 in parallel.


### **General Requirements for Basic Safety & Essential Performance**
- **Means of Protection (MOP)**: You must ensure:
    - **1xMOP** for operator protection.
    - **2xMOP** for patient protection (higher standard).
- **Creepage & Clearance** distances must meet strict minimums.
- **Insulation levels** (basic, supplementary, reinforced) are defined by voltage and use case.
- **Leakage currents** (earth, touch, patient): must be tightly controlled and measured.
- **Protective earth continuity** and **fuse placement** are scrutinized.

### 2. **EMC (60601-1-2)**
- Medical devices must operate safely in noisy environments and not interfere with other equipment.
- Immunity testing includes ESD, EFT, Surge, Conducted & Radiated RF.
### 3. **60601-1-6 / Usability Engineering**
- Ties into UI and system-level design, but affects physical controls, labeling, and indicators.
### 4. **Testing & Documentation**
- You need to **justify all design choices** (e.g. why a specific filter is placed).
- **Test reports** must be kept and traceable to each design revision.
### 🔌 Power & Isolation
- Use **medical-grade isolated power supplies**.
- Optocouplers or transformers for **galvanic isolation** between patient-connected circuits and logic.
- Never trust the USB or wall power ground as system ground.
### 🔬 Component Selection
- Prefer **AEC-Q, industrial or medical-grade** components.
- Avoid components with unknown lifecycle or lack of supply chain support.
- Temperature ratings matter (often −40 °C to +85 °C or higher).
### 🌡️ Thermal Management
- No hot spots reachable by user/patient.
- Must remain **below burn thresholds** (often ~41–45°C max on contact surfaces).
### 📜 Documentation
- Everything must be **verifiable, repeatable, and traceable**.
- Design files, risk analysis, verification & validation plans, test procedures.