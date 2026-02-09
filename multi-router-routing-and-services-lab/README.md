## Overview
This project demonstrates advanced networking concepts including
multi-router topology design, static routing, route summarization,
DNS configuration, DHCP services, and centralized configuration
management. The lab simulates an ISP-connected enterprise network
with multiple internal routers and services.

---

## Network Architecture
**Routing & Switching**
- Cisco 1941 routers (ISP, R1, R2, R3)
- Cisco 2960 switches (access layer)

**End Devices & Services**
- Client PCs and administrative workstation
- Multiple servers providing:
  - HTTP
  - DNS
  - TFTP
  - DHCP

**Addressing**
- Multiple internal networks including:
  - `10.0.0.0`-based networks
  - `192.168.0.0/24` ranges
  - DHCP pool: `192.168.30.0/24` (NET30)

---

## Implementation Details
- Installed and configured appropriate router modules
- Assigned IP addresses based on a predefined network design
- Configured static routing across all routers
- Implemented default routes using next-hop addressing
- Configured additional interface-based static routes on R2
- Implemented route summarization on the ISP router for efficient routing
- Configured DNS settings on all hosts pointing to a centralized DNS server
- Created a custom domain record (`name.surname.ge`) resolving to a web server
- Verified web access via domain name from an administrative client
- Configured DHCP service on R3 to dynamically assign IP addresses
- Connected new clients to receive addresses automatically
- Backed up router configurations to a TFTP server
- Set system time and date on the ISP router

---

## Security & Networking Perspective
- Demonstrates hierarchical network design with ISP and internal routing layers
- Shows the importance of route summarization for scalability and efficiency
- Highlights centralized services (DNS, DHCP, TFTP) as critical infrastructure
- Models real-world risks of misconfigured default routes and DNS records
- Reinforces configuration management and backup as part of network security
- Demonstrates separation of control, access, and service layers

---

## Validation
- Verified end-to-end connectivity between all networks using ICMP (ping)
- Confirmed successful DNS name resolution to the web server
- Verified HTTP access via custom domain name
- Confirmed DHCP address allocation for newly added clients
- Verified successful router configuration backups to the TFTP server

---

## Career Relevance
This project builds hands-on experience directly applicable to:
- **Network Engineering** – routing design, summarization, and services
- **Cybersecurity & Ethical Hacking** – understanding routing paths,
  service exposure, and infrastructure dependencies
- **System & Network Administration** – DNS, DHCP, backups, and validation
- **Technical Troubleshooting** – diagnosing routing, naming, and service issues
