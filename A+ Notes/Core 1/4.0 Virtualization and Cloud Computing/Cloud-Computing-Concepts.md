# Cloud Computing Concepts – CompTIA A+ Core 1 (4.2)

Understand the key service models and deployment types that define cloud computing in modern IT.

---

## ☁️ What is Cloud Computing?

Cloud computing allows users to access shared resources — like storage, apps, or servers — via the internet.

### Key Benefits:
- Scalability
- Pay-as-you-go pricing
- Access from anywhere
- Minimal local hardware requirements

---

## 🧱 Cloud Service Models

| Model | Description                 | Examples                          |
|-------|-----------------------------|-----------------------------------|
| SaaS  | Software-as-a-Service       | Google Docs, Dropbox, Office 365  |
| PaaS  | Platform-as-a-Service       | Heroku, AWS Elastic Beanstalk     |
| IaaS  | Infrastructure-as-a-Service | AWS EC2, Azure Virtual Machines   |

---

## 🌐 Deployment Models

| Type        | Description                             |
|-------------|-----------------------------------------|
| Public      | Open to anyone (e.g., AWS, Google Cloud)|
| Private     | Internal to a single organization       |
| Hybrid      | Combination of public and private       |
| Community   | Shared by organizations with common goals |

---

## 💡 A+ Exam Tips

- Know examples of SaaS, PaaS, and IaaS
- Understand the difference between public, private, hybrid, and community cloud
- Expect real-world use cases (e.g., "A company uses Google Docs...")

---

> “The cloud is where services live — and scale — without limits.”
>
> # CompTIA A+ Study Notes — Cloud Computing (Objective 4.1 and 2.2)

## Cloud Computing
- **Definition**: The practice of using a network of remote servers hosted on the Internet.

---

## Characteristics of the Cloud

### High Availability
- Services experience very little downtime when using the cloud.
- Availability = Percentage of uptime vs. downtime.

### Scalability
- Ability to increase the number of items in a system at a linear rate or less.

#### Vertical Scaling (Scaling Up)
- Increasing the power of the existing resources in the working environment.

#### Horizontal Scaling (Scaling Out)
- Adding additional resources to help handle extra load.

### Rapid Elasticity
- Ability to quickly scale up or down.
- Elasticity = System’s ability to handle demand changes in real-time.

### Metered Utilization
- Charged for service on a pay-per-use basis.
- Cloud typically uses metered billing.

### Measured Services
- Charged based on actual usage of service consumed.

### Shared Resources
- Pooling together hardware (e.g., VMs on shared servers).

### File Synchronization
- Storing data that syncs across locations based on configuration.

---

## Cloud Deployment Models

### Public Cloud
- Devices interact with public networks like the internet and other clouds.

### Private Cloud
- Devices access only within the same private cloud or system.

### Hybrid Cloud
- Mix of private and public clouds.

### Community Cloud
- Infrastructure shared between several orgs with common concerns.

### Multitenancy
- Customers share computing resources in public or private cloud.

### Single-Tenancy
- Resource assigned to a single organization.

---

## Cloud Service Models

### On-Premise Solution
- Organization provides hardware, software, personnel.
- Full control over physical and logical access to servers.

### Hosted Solution
- Third-party maintains all hardware and facilities for cloud access.

---

## IaaS vs PaaS vs SaaS vs On-Prem

| Component     | On-Prem | IaaS | PaaS | SaaS |
|---------------|---------|------|------|------|
| Application   | ✔️      | ❌   | ❌   | ❌   |
| Data          | ✔️      | ✔️   | ❌   | ❌   |
| Runtime       | ✔️      | ✔️   | ✔️   | ❌   |
| Middleware    | ✔️      | ✔️   | ✔️   | ❌   |
| OS            | ✔️      | ✔️   | ✔️   | ❌   |
| Virtualization| ✔️      | ✔️   | ✔️   | ❌   |
| Servers       | ✔️      | ✔️   | ✔️   | ❌   |
| Storage       | ✔️      | ✔️   | ✔️   | ❌   |
| Networking    | ✔️      | ✔️   | ✔️   | ❌   |

---

## Virtual Desktop Infrastructure (VDI)

- **VDI**: Hosts desktop OSs on a centralized server/server farm.
- **Server**: Processes applications and stores data.
- **Centralized Model**: Hosts all desktop instances on one server/farm.
- **Hosted Model / Desktop as a Service (DaaS)**: Provided by third-party to end-user.

---

## Cloud Storage Services

- **Cloud Storage Application**: Cloud-based file storage.
- **File Synchronization**: Syncs files across devices with one account.
- **Content Delivery Network (CDN)**: Uses closest server to reduce delay.

---

## Software-Defined Networking (SDN)

- Centrally controlled, programmed via software applications.
- Can automate via orchestration tools.

---

## SDN Layers

### Application Layer
- Handles communication and requests over the network.

### Control Layer
- Uses app data to determine packet routing.

### Infrastructure Layer
- Contains devices that physically move the data.

### Management Plane
- Monitors network status and traffic.
- Provides abstraction between control/data flow and devices.

---
