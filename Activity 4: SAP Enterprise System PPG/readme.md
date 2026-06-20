# Activity 4: Digital Enterprise Exploration — SAP Core Modules & PPG Global Supply Chain 🧪🎨

## 1. Project Summary
As part of my academic coursework in **Enterprise Systems Design and Modeling (SECJ3744)**, our team completed an extensive hands-on research project to analyze how standard **SAP ERP modules** translate into operational workflows within a real-world, global enterprise like **PPG Industries** (a leading global paints and coatings manufacturer). The core purpose of this exploration was to understand the tight integration dependencies between high-scale purchasing, sales, manufacturing, and financials, preparing our architectural mindset ahead of direct industrial ecosystem dialogues.

Our technical evaluation models the real-world operational alignment between private software modules and digital business operations:
* **SAP Core Module Deconstruction:** We investigated the functionalities and cross-module handshakes across five foundational SAP pillars: **MM** (Materials Management for procurement and goods receipt), **SD** (Sales & Distribution for client billing and distribution), **FI** (Financial Accounting for general ledger records), **PP** (Production Planning for factory resource scheduling), and **HCM** (Human Capital Management for payroll and employee logs).
* **Enterprise Process Flow Mapping:** We traced full transaction lifecycles—such as the standard *Procure-to-Pay* cycle—demonstrating how a raw material request or purchase order generated in SAP MM automatically shifts accounting ledger balances in SAP FI and updates stock availability tables inside factory warehouses.
* **PPG Industrial Contextualisation:** We mapped PPG's massive multi-plant supply chain down to these architectural boundaries. We analyzed how a sudden large-scale paint or resin sales order entered by the sales team instantly prompts the PP module to recalculate factory line schedules, while concurrently triggering the MM module to order chemical pigments from international suppliers if local inventory thresholds drop.

---

## 2. Reflection

**What I have learnt:**

* This deep dive completely changed how I look at corporate software. I learned that SAP is not just an isolated database or a data entry tool, but rather acts as the central brain of a global corporation, ensuring that an activity on the factory floor instantly changes accounting sheets, logistics routes, and procurement lists simultaneously.
* Mapping out the transaction flows taught me how different corporate departments rely on automated data handshakes. I realized that the smooth execution of a business lifecycle, like moving from a procurement order to an invoice payment, depends entirely on keeping clean, real-time data consistent across different system modules.
* Investigating PPG's global footprint helped me understand why massive manufacturing entities are forced to deploy highly integrated enterprise systems. I learned that manual data coordination fails when dealing with multiple production plants and constant raw material purchasing, making a digital backbone like SAP absolutely essential to stay competitive.

---
