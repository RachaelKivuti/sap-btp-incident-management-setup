# Setup and Deployment the SAP CAP Incident Management App on SAP BTP 

This repository documents my hands-on process of setting up, and deploying an enterprise-grade cloud application from scratch.

---

## Application Overview
The **Secure Incident Management** application is a sample enterprise ticketing and tracking system built on the **SAP Cloud Application Programming Model (CAP)**. 

While it functions like a standard internal helpdesk tool (managing incidents, statuses and users), it is purposely designed as a **security and compliance playground**. It bridges the gap between enterprise cloud architecture and application security, preparing us to explore real-world vulnerabilities.

---

## Why this project? (Exploring SAP Application Security)
In modern cloud security, you cannot secure what you don't understand. Setting up this architecture teaches you the critical layers of enterprise applications:
1. **Cloud Infrastructure:** Deploying multi-tier apps onto **SAP BTP (Business Technology Platform)** and **SAP HANA Cloud**.
2. **Identity & Access Management (IAM):** Configuring Custom Identity Providers (IAS), importing users via SCIM 2.0 and assigning Role Collections. (In the real world, misconfigured permissions here lead to major security breaches!)
3. **The Foundation for Security Testing:** This setup is the launching pad. With a working, fully deployed environment, we can move straight into offensive security exercises; testing authorization logic, role bypasses and access controls.

---

## Quick Navigation
1. [Environment & Identity Setup](docs/01-environment-and-identity-setup.md)
2. [Database Provisioning](docs/02-database-provisioning.md)
3. [MTA Deployment](docs/03-deployment.md)
4. [Work Zone Configuration](docs/04-workzone-configuration.md)
5. [Known Issues & Troubleshooting](docs/issues-and-troubleshooting.md)
