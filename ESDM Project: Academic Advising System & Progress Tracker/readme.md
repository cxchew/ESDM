# ESDM Project: Integrated Academic Advising & Early Warning System (UTHM Case Study) 🎓🏫

## 1. Project Summary
As part of our major capstone project for **Enterprise Systems Design and Modeling (SECJ3744)**, our team engineered a conceptual and high-fidelity prototype framework for an **Integrated Academic Advising and Progress Tracker System** tailored for **Universiti Tun Hussein Onn Malaysia (UTHM)** under the Work-Based Learning (WBL) structure. The core business purpose of this enterprise blueprint is to eliminate traditional higher-education data silos that prevent academic advisors from easily viewing student CGPAs or attendance records, thereby mitigating student retention drops and graduation delays. 

Using the **TOGAF ADM Framework** as our design methodology, we structured the application architecture to ensure continuous cross-module data streams, pulling master records via Single Sign-On (SSO) authentication from UTHM’s master databases (SMP/SMS) while managing live transactional data within localized cloud databases. 

The application architecture is explicitly divided into six highly specialized technical modules, each assigned to distinct engineering components:
* **Module 1 (Advising Appointment Scheduling):** Manages the full lifecycle of academic counseling sessions by generating unique `Appointment ID` tokens, enabling students and advisors to orchestrate, schedule, and confirm virtual or physical consultation slots.
* **Module 2 (Advising Notes & Recommendations):** Consumes the active `Appointment ID` from Module 1 to capture, catalog, and archive detailed advising notes, personalized study paths, and specific corrective action items generated during active sessions.
* **Module 3 (Academic Progress Validation for Graduation):** Automates the mapping of student academic records against rigorous institutional graduation requirements to provide real-time checklists that highlight credit deficits and prevent graduation delays.
* **Module 4 (Comprehensive Academic Progress Dashboard):** Aggregates cross-departmental data feeds into a centralized, high-visibility user dashboard to present advisors and students with holistic trends regarding CGPA vectors, course logs, and educational histories.
* **Module 5 (Early Warning & At-Risk Student Detection):** Acts as the system’s predictive analytics engine by consuming data layers from Modules 3 and 4 to instantly detect steep grade drops or critical attendance exceptions, automatically flagging and categorizing at-risk students into granular warning levels.
* **Module 6 (Advising Records & Document Management):** Serves as the system's central secure data repository, using the `Appointment ID` to manage, verify, and store formal academic records, exception letters, and historical counseling documentation.

---

## 2. Reflection

**What I have learnt:**

* This project completely changed how I approach large-scale software design. Learning how to apply the TOGAF framework showed me that engineering a system for thousands of campus users requires a structured plan—moving methodically from initial high-level business goals down to data schemas and infrastructure deployments to keep every part aligned.
* Working with SAP Build Apps taught me how modern enterprises accelerate their engineering lifecycles. I realized that by utilizing visual low-code development platforms, software architects can instantly turn complex database schemas and business logic into high-fidelity working applications, allowing for quick user feedback without wasting months writing boilerplate code.
* Designing the data connections between performance monitors, early warnings, and advising portals taught me the core purpose of enterprise systems. I learned that by breaking down data silos and replacing slow, manual processes with real-time predictive warnings, software can actively step in to help users before administrative problems grow too big.

---

### 👥 Team Credits (Group Assignment)
* **Lau Yan Kai** (A23CS0098)
* **Joanne Ching Yin Xuan** (A23CS0084)
* **Chew Chiu Xian** (A23CS0061)
* **Lim Yu Han** (A23CS0104)
* **Evelyn Goh Yuan Qi** (A23CS0072)
* **Elijah She Yu Sheng** (A23CS0070)
* **Course Instructor:** Dr. Noorminshah binti A.Iahad
