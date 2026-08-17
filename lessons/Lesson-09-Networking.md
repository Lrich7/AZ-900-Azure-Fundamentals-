[Lesson-09-Networking.md](https://github.com/user-attachments/files/31148694/Lesson-09-Networking.md)

# Lesson 9 — Networking

## 📖 Microsoft Learn

**Module:** Azure Networking Fundamentals  
https://learn.microsoft.com/en-us/training/modules/azure-networking-fundamentals/

### Focus
- Virtual Networks (VNets)
- Subnets
- Network Security Groups (NSGs)
- Public Endpoints
- Private Endpoints
- Azure DNS
- Public IP Addresses

---

## 🎥 Recommended Videos — John Savill's Technical Training

| Topic | Length | Link |
|---|:---:|---|
| Benefits and Usage of Core Network Resources | 22:04 | https://youtu.be/aNK0C9Oj2sg |
| Describe Public and Private Endpoints | 7:23 | https://youtu.be/bPNkXwRFsek |

---

# Azure Networking

Azure networking services allow cloud resources to communicate with each other, the internet, and on-premises networks.

Networking also provides ways to organize, isolate, and secure that communication.

---

# Virtual Networks (VNets)

An **Azure Virtual Network (VNet)** is a private network in Azure that allows Azure resources to securely communicate.

A VNet can support communication between:

- Azure resources
- The internet
- On-premises networks

VNets provide isolation, security, and control over network traffic.

### Real-World Thinking

A company can create a VNet for its Azure resources so virtual machines and other services can communicate over a controlled private network.

### Exam Thinking

> **Virtual Network (VNet) = Azure's private network.**

---

# Subnets

A **Subnet** is a smaller network created inside a Virtual Network.

Subnets allow resources to be organized into separate network segments.

```text
Virtual Network
|
+-- Subnet 1
|
+-- Subnet 2
|
+-- Subnet 3
```

## Why Use Subnets?

- Organize resources
- Separate workloads
- Improve network management
- Apply security controls to groups of resources

### Real-World Thinking

A company could place web servers in one subnet and application servers in another.

### Exam Thinking

> **Subnet = smaller network inside a VNet.**

---

# Network Security Groups (NSGs)

**Network Security Groups (NSGs)** are used to filter inbound and outbound network traffic for Azure resources.

NSG rules can evaluate traffic based on:

- Priority
- Source
- Destination
- Port
- Protocol

## Rule Priority

Rules are evaluated by priority number.

Lower priority numbers are processed before higher priority numbers.

## Stateful Traffic

NSGs use stateful connection tracking. Return traffic for an allowed connection is automatically handled.

## Default Rules

Azure provides default NSG rules that support basic internal Azure networking while restricting unsolicited external inbound traffic.

## Where NSGs Can Be Applied

### Subnet
An NSG can protect resources connected to a subnet.

### Network Interface (NIC)
An NSG can also be associated with an individual network interface.

### Real-World Thinking

An administrator could use an NSG rule to allow required web traffic while blocking unwanted inbound connections.

### Exam Thinking

> **NSG = traffic-filtering security rules for Azure networking.**

Think **virtual firewall rules**.

---

# Public Endpoints

A **Public Endpoint** allows an Azure resource to be accessed through the public internet.

Public access can still be protected using:

- Authentication
- Firewalls
- Network security rules
- Other access controls

The important distinction is that the resource remains reachable through a public network path.

### Exam Thinking

> **Public Endpoint = access through the public internet.**

---

# Private Endpoints

A **Private Endpoint** provides access to a supported Azure service through a private IP address in a VNet.

This reduces exposure to the public internet and allows traffic to use private network connectivity.

### Real-World Thinking

A company may want an application to access an Azure service privately from its VNet rather than exposing the service through a public endpoint.

### Exam Thinking

> **Private Endpoint = private IP access from a VNet.**

---

# Public vs. Private Endpoints

| Feature | Public Endpoint | Private Endpoint |
|---|---|---|
| Network path | Public network / internet | Private VNet connectivity |
| Addressing | Public-facing address or URL | Private IP address |
| Exposure | Publicly reachable path | Reduced public exposure |
| Typical Goal | Internet accessibility | Private service access |

### Easy Way to Remember

```text
Public Endpoint  = Front door
Private Endpoint = Private employee entrance
```

---

# Azure DNS

**Azure DNS** is a cloud-based Domain Name System hosting service.

DNS translates human-readable domain names into IP addresses that computers use to locate resources.

```text
www.contoso.com
       |
       v
    DNS Lookup
       |
       v
   IP Address
```

### Real-World Thinking

People remember names more easily than IP addresses. DNS allows users and applications to use names while the network uses IP addresses.

### Exam Thinking

> **Azure DNS = hosts DNS records and resolves names to IP addresses.**

---

# Public IP Addresses

A **Public IP Address** is an internet-routable IP address that can be associated with Azure resources that require public network communication.

Public IP addresses can be used with services such as:

- Virtual machines
- Load balancers
- Other internet-facing Azure resources

### Exam Thinking

> **Public IP Address = internet-facing address for an Azure resource.**

---

# Office Building Analogy

Think of Azure networking like an office building:

| Azure Concept | Office Building |
|---|---|
| **Virtual Network** | Entire office building |
| **Subnet** | Department or floor |
| **Public Endpoint** | Front entrance for visitors |
| **Private Endpoint** | Secure employee-only entrance |
| **Azure DNS** | Company directory |
| **Public IP Address** | Building's public street address |
| **NSG** | Security rules controlling who can enter or leave |

---

# Comparing the Core Networking Concepts

| Concept | Remember |
|---|---|
| **VNet** | Private Azure network |
| **Subnet** | Smaller network inside a VNet |
| **NSG** | Filters inbound and outbound traffic |
| **Public Endpoint** | Public network access |
| **Private Endpoint** | Private VNet access |
| **Azure DNS** | Name-to-IP resolution |
| **Public IP Address** | Internet-routable address |

---

# 🧪 Hands-On Lab

Complete the companion lab:

**[Lesson 09 Lab — Networking](https://github.com/Lrich7/AZ-900-Azure-Fundamentals-/blob/main/labs/Lesson-09-Lab-09-Networking.md)**

### Lab Focus

- Create or configure a Virtual Network exercise.
- Explore subnets.
- Explore Network Security Groups.
- Explore Public IP Addresses.
- Explore Azure DNS.
- Compare Public and Private Endpoints.
- Practice selecting the correct networking concept for common scenarios.

> [!TIP]
> Azure Portal exploration, resource configuration, and practical exercises are kept in the separate lab.

---

# Quick Check

| Question | Answer |
|---|---|
| Azure's private network | Virtual Network |
| Smaller network inside a VNet | Subnet |
| Filters inbound and outbound network traffic | Network Security Group |
| Publicly reachable network path | Public Endpoint |
| Private IP access to an Azure service | Private Endpoint |
| Resolves names to IP addresses | Azure DNS |
| Internet-routable Azure address | Public IP Address |

---

# Before Moving On

You should be able to:

- Explain the purpose of a Virtual Network.
- Explain the purpose of a subnet.
- Explain why Network Security Groups are used.
- Explain the difference between Public and Private Endpoints.
- Explain the purpose of Azure DNS.
- Explain what a Public IP Address provides.
- Explain how Azure networking helps secure cloud resources.
- Choose the correct networking concept from a basic scenario.

---

# Exam Thinking Summary

| Concept | Remember |
|---|---|
| **VNet** | Azure private network |
| **Subnet** | Network segment inside a VNet |
| **NSG** | Inbound/outbound traffic filtering |
| **Public Endpoint** | Public network access |
| **Private Endpoint** | Private VNet access |
| **Azure DNS** | Name resolution |
| **Public IP** | Internet-routable address |
