# SAP BTP Secure Incident Management: Setup 

This repository documents my hands-on process of setting up, and deploying an enterprise-grade cloud application from scratch.

---

## What is this project?
The **Secure Incident Management** application is a sample enterprise ticketing and tracking system built on the **SAP Cloud Application Programming Model (CAP)**. 

While it functions like a standard internal helpdesk tool (managing incidents, statuses and users), it is purposely designed as a **security and compliance playground**. It bridges the gap between enterprise cloud architecture and application security, preparing us to explore real-world vulnerabilities like **Broken Access Control**.

---

## Why deploy this as a beginner?
In modern cloud security, you cannot secure what you don't understand. Setting up this architecture teaches you the critical layers of enterprise applications:
1. **Cloud Infrastructure:** Deploying multi-tier apps onto **SAP BTP (Business Technology Platform)** and **SAP HANA Cloud**.
2. **Identity & Access Management (IAM):** Configuring Custom Identity Providers (IAS), importing users via SCIM 2.0 and assigning **Role Collections**. (In the real world, misconfigured permissions here lead to major security breaches!)
3. **The Foundation for Security Testing:** This setup is the launching pad. With a working, fully deployed environment, we can move straight into offensive security exercises—testing authorization logic, role bypasses and access controls.

---

## Repository Structure

* `docs/` - Step-by-step, beginner-friendly deployment guides and terminal command walkthroughs.
* `screenshots/` - Visual checkpoints for every configuration step to keep you on track.
* `issues-and-troubleshooting.md` - A personal log of real roadblocks hit along the way (endpoint routing, landscape variations and CLI targeting errors) and their solutions.

---

## Quick Navigation
1. [Subaccount & Environment Setup](docs/01-subaccount-setup.md)
2. [Database Provisioning & Deployment Guide](docs/deployment-guide.md)
3. [Known Issues & Troubleshooting](issues-and-troubleshooting.md)
