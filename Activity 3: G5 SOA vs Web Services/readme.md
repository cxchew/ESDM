# Activity 3: Architecture Deep Dive — Service-Oriented Architecture (SOA) vs. Web Services 🌐🔌

## 1. Project Summary
As part of my academic coursework in **Enterprise Systems Design and Modeling (SECJ3744)**, our team conducted a comparative structural analysis to define the boundaries between Service-Oriented Architecture (SOA) as a macro-design paradigm and Web Services as a concrete execution technology. The purpose of this activity was to explore how massive modern enterprises decouple legacy on-premises applications and combine separate organizational modules into flexible, loosely connected systems that prevent programmatic deadlocks.

Our technical evaluation models the distinct layers and execution mechanisms of enterprise application integration:
* **The SOA Conceptual Blueprint:** We evaluated SOA as an architectural philosophy that breaks large systems into small, independent units (e.g., separating an operational footprint into autonomous Account, Book, Order, and Shipping services). Each service executes one specific business function and shares data via a centralized communication highway known as an **Enterprise Service Bus (ESB)**.
* **The Web Service Implementation Layer:** We analyzed Web Services as the programmatic tools used to realize SOA designs across the internet. These connections rely on standardized data formats like HTTP, XML, or JSON to pass message requests and responses between distinct servers, such as a localized mobile app querying external Google Maps or banking API registries.
* **Real-World Ecosystem Mapping:** We contextualized these concepts by mapping a multi-service academic ecosystem. In this setup, an ESB acts as the message router to connect distinct Student Profiles, Finance Payments, Library Fines, and Hostel Maintenance records, allowing secondary client applications (like a CRM) to reuse existing services without being tightly bound to them.

---

## 2. Reflection

**What I have learnt**

* This activity helped me clear up a major point of confusion by showing me that SOA and Web Services are not competing technologies. I learned that SOA is the strategic architectural plan for structuring a whole company's business capabilities, while Web Services are the physical tools and data formats (like REST, SOAP, and JSON) used to connect those pieces over the internet.
* Investigating the ESB taught me how large organizations prevent messy point-to-point connections. I realized that by routing all background service communication through a centralized service bus, different sub-systems—like university finance, library records, and student portals—can talk to each other without becoming tightly dependent on one another.
* I learned that decoupling business logic into independent, reusable services dramatically drives down long-term software maintenance costs. This assignment proved that when services are built with loose connections, a company can easily attach a new mobile app or external CRM to its backend without rewriting the core database logic from scratch.

---

### 👥 Team Credits (Group 5)
* **Sabrina Heng Wei Qi** (A23CS0265)
* **Woo Cheng Shuan** (A23CS0271)
* **Lau Yan Kai** (A23CS0098)
* **Chew Chiu Xian** (A23CS0061)
* **Neo Li Xin** (A23CS0246)
* **Course Instructor:** Dr. Noorminshah binti A.Iahad
