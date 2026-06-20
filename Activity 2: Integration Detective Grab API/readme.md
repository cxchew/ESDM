# Activity 2: System Integration Detective — Grab Platform Case Study 🚗📱

## 1. Project Summary
As part of my academic coursework in **Enterprise Systems Design and Modeling (SECJ3744)**, our team assumed the roles of "System Integration Detectives" to analyze the multi-layered digital architecture of the **Grab super-app**. The objective of this investigation was to dissect the data exchange mechanisms that tie customer endpoints to downstream fulfillment systems, mapping out what happens under the hood when a user executes an order and classifying how system failures ripples across business workflows.

Our structural analysis maps out Grab's integration dependencies and failure vulnerabilities across multiple categories:
* **Decoupled System Architecture Mapping:** We tracked data streams moving concurrently between six core sub-systems: the Customer and Driver Mobile Apps, the Restaurant Inventory Management System, the Payment Gateway System, the central Dispatch and Routing engine, the Customer Relationship Management (CRM) platform, and the core Backend Servers/Databases.
* **API Handshake Protocols:** We evaluated execution mechanics, separating **Synchronous API Calls** (where the Order Management System freezes process loops to await instant token validation from the payment gateway) from **Asynchronous Callbacks/Webhooks** (where systems are alerted out-of-band when a payment state changes or a merchant updates food inventory).
* **Integration Failure Taxonomy:** We classified platform bugs into two structural categories to study operational risk profiles:
  * **Logical Integration Issues:** Occur due to design flaws and race conditions (e.g., inconsistent menu data where a customer successfully orders a "sold out" item because store data updates via slow batch files, causing driver frustration, high cancel rates, and customer support bottlenecks).
  * **Physical Integration Issues:** Occur due to concrete infrastructure timeouts (e.g., network disconnects, server downtime at Grab's backend, database crashes losing live trip records, or Firebase/APNs push notification delivery drops that force support teams to manually manage claims).
* **Architecture Optimisation Strategy:** We proposed replacing rigid batch synchronization scripts with modern, **Event-Driven Webhooks** to ensure that whenever a merchant marks an asset as unavailable in their local POS, the Grab menu refreshes in real time, dramatically driving down refund requests.

---

## 2. Reflection

**What I have learnt:**

* This activity taught me how modern enterprise super-apps balance different communication styles. I learned that while high-security actions like checking a credit card require a rigid synchronous API loop that waits for an instant response, background activities like tracking a driver's GPS location or updating delivery statuses must run asynchronously to prevent app lag.
* Investigating the "sold-out but still orderable" glitch showed me that software bugs are rarely just technical problems—they have huge business costs. I realized that a simple data sync delay between a restaurant's POS system and Grab's app creates a chain reaction of canceled rides, angry customers, and expensive manual customer support intervention.
* Classifying problems into logical design flaws and physical infrastructure crashes changed how I think about system safety. I learned that engineers must design systems assuming things will break, using tools like real-time event-driven webhooks and automatic fallback paths to protect data flow when third-party push networks or payment gateways go offline.

---

### 👥 Team Credits (Group 5)
* **Sabrina Heng Wei Qi** (A23CS0265)
* **Woo Cheng Shuan** (A23CS0271)
* **Lau Yan Kai** (A23CS0098)
* **Chew Chiu Xian** (A23CS0061) — *Portfolio Owner*
* **Neo Li Xin** (A23CS0246)
* **Course Instructor:** Dr. Noorminshah binti A.Iahad
