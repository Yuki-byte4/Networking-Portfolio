## Overview
This project demonstrates core networking fundamentals, including IPv4
addressing, end-to-end connectivity testing, and basic client–server
communication. The lab simulates a small real-world network where multiple
subnets interact with a centralized web service.

---

## Network Components
**Endpoints**
- Multiple desktop clients (PCs)
- One mobile client (Laptop)

**Services**
- Centralized server providing HTTP web services

**Infrastructure**
- Cisco 2960 switch for Layer 2 switching
- Generic hub to model legacy broadcast-based connectivity

**Addressing**
- Static IPv4 addressing across two logical networks:
  - `192.168.20.0/24`
  - `172.16.0.0/24`

---

## Implementation Details
- Configured multiple subnets with correct IP addressing and gateway logic
- Assigned device hostnames following documentation standards
- Verified full connectivity using ICMP (ping) between all endpoints
- Accessed the server-hosted web page from a client using a virtual browser

---

## Security & Networking Perspective
- Demonstrates how data flows from lower network layers to the application
  layer during HTTP communication
- Highlights the importance of correct IP configuration for service
  availability across subnets
- Models unicast and broadcast traffic behavior in mixed environments
- Shows how using a hub instead of a switch increases the collision domain,
  expanding the attack surface for traffic interception

---

## Validation
- Successful ICMP communication between all clients and the server
- Verified HTTP access from the laptop to the server
- Confirmed correct hostname configuration across infrastructure devices

---

## Career Relevance
This lab strengthens foundational networking knowledge required for:
- **Cybersecurity & Ethical Hacking** – understanding network paths and attack
  surfaces before exploitation or defense
- **Network Engineering** – designing and validating structured IP networks
- **Technical Support & Troubleshooting** – diagnosing connectivity and service
  issues using standard tools
