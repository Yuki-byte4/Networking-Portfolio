## Overview
This project represents a capstone-level enterprise networking lab,
combining WAN connectivity, advanced subnetting, static and default
routing, and centralized network services. The topology models a
multi-site organization with a headquarters, branch offices, and an
ISP-connected public service network.

---

## Network Architecture
**Core & WAN Routing**
- Cisco 1941 routers (HQ, Branch 1, Branch 2, ISP)
- Serial WAN links using subnetted address space

**Access Layer**
- Cisco 2960 switches connecting end devices

**End Devices & Services**
- Client workstations across multiple internal networks
- Public-facing web server
- DHCP, DNS, and TFTP services

---

## Addressing & Subnetting
- Implemented structured IPv4 addressing across multiple LANs
- Subnetted `172.17.1.0/24` into four `/26` networks for WAN links
- Assigned first usable IPs to HQ interfaces and last usable IPs to
  branch router interfaces
- Configured public IP addressing for ISP-facing services

---

## Implementation Details
- Installed and configured serial interfaces on routers
- Assigned static IP addresses and verified interface states
- Configured encrypted and unencrypted router access passwords
- Implemented DHCP services for dynamic client addressing
- Configured DNS resolution pointing to centralized services
- Implemented static routing on all routers
- Configured default routes using both next-hop and exit-interface methods
- Backed up router configurations to a TFTP server
- Verified end-to-end connectivity and service accessibility

---

## Security & Networking Perspective
- Demonstrates enterprise WAN design with trust boundaries
- Highlights risks of misconfigured default and static routes
- Shows how DHCP, DNS, and HTTP services become critical attack targets
- Reinforces the importance of configuration backups and time settings
- Models realistic attack surfaces across LAN, WAN, and ISP layers

---

## Validation
- Verified ICMP connectivity between all internal networks and servers
- Confirmed successful DHCP address allocation
- Verified DNS name resolution and HTTP service availability
- Confirmed successful configuration uploads to TFTP server

---

## Career Relevance
This project demonstrates job-ready foundational skills for:
- **Network Engineering** – enterprise routing and WAN design
- **Cybersecurity & Ethical Hacking** – understanding routing paths,
  service exposure, and infrastructure dependencies
- **System & Network Administration** – DHCP, DNS, backups, and validation
- **Incident Response & Troubleshooting** – isolating routing and service
  failures in complex environments
