# ICMP Flood DoS Simulation and ACL-Based Defense

## Overview

This project is a practical cybersecurity and networking lab built using Cisco Packet Tracer to explore the concept of **Denial of Service (DoS)** attacks and basic network defense mechanisms.

The motivation behind this lab was to take the **CIA Triad**, specifically the concept of **Availability**, and demonstrate how network resources can be affected by excessive traffic and how administrators can implement controls to reduce risk.

The lab explores both perspectives:

- **Attacker perspective:** Understanding how excessive ICMP traffic can affect service availability.
- **Defender perspective:** Implementing Access Control Lists (ACLs) to control and filter network traffic.

---

# Objectives

By completing this lab, I aimed to understand:

- How Denial of Service (DoS) attacks affect network availability.
- The role of ICMP in network troubleshooting.
- The difference between normal network communication and traffic abuse.
- How routers can be configured to enforce security policies.
- How ACLs can be used as a basic network defense mechanism.

---

# Lab Scenario

A small organization has:

- An internal web server hosting a service.
- Internal users accessing the service.
- An external user representing a potential attacker.

The goal was to simulate how an attacker could attempt to disrupt availability by generating continuous ICMP traffic toward the server.

After exploring the attack scenario, a defensive control was implemented to restrict unwanted ICMP traffic.

---

# Network Topology

The topology consists of:

## External Network

Representing an external user/attacker.


---

## Internal Network

Representing the organization's internal environment.


---

# Technologies and Concepts Practiced

## Networking Concepts

- IPv4 addressing
- Subnetting
- Default gateways
- Routing between networks
- MAC addresses and ARP
- ICMP communication

---

## Cybersecurity Concepts

### CIA Triad - Availability

The lab demonstrates how attackers can target availability by overwhelming system resources.

The objective of a DoS attack is not always to steal information or gain unauthorized access. Sometimes the goal is simply to prevent legitimate users from accessing a service.

---

### Denial of Service (DoS)

The lab simulated an ICMP-based traffic flood.

Normal communication:


---

### Historical Ping of Death vs Modern DoS

The lab also explored the difference between:

**Historical Ping of Death**

- Exploited software vulnerabilities.
- Used malformed oversized packets.
- Could crash vulnerable systems.

**Modern DoS attacks**

- Usually focus on resource exhaustion.
- Consume bandwidth, CPU, memory, or connection capacity.
- Aim to make services unavailable.

---

# Defensive Implementation

After understanding the attack perspective, an ACL was configured on the router to restrict external ICMP traffic toward the internal server.


The purpose of the ACL was:

- Block unwanted ICMP traffic from the external network.
- Allow other legitimate traffic.
- Demonstrate how security policies can be enforced at the network layer.

---

# Testing

## Before ACL Configuration

The external attacker could communicate with the server.


---

## After ACL Configuration

ICMP traffic from the external network was blocked.

However:

- The server remained online.
- Legitimate users could still access services.
- Other permitted traffic continued functioning.

This demonstrated the difference between:

"Blocking a specific threat"

and

"Blocking the entire network."

---

# Key Lessons Learned

This lab reinforced that cybersecurity begins with understanding normal network behavior.

Key takeaways:

- Availability is a critical part of cybersecurity.
- Not every attack involves stealing information.
- Legitimate protocols can be abused.
- Network defenders must understand attacker techniques.
- Security controls should reduce risk while maintaining usability.
- ACLs provide basic traffic filtering capabilities.

---

# Tools Used

- Cisco Packet Tracer
- Cisco IOS CLI
- IPv4 addressing
- Extended ACLs

---

# Files Included

ICMP_DoS_ACL_Defense.pkt
acl_configuration.png
README.md


---

# Future Improvements

Possible future extensions of this lab:

- Implement firewall-based filtering.
- Explore rate limiting.
- Add IDS/IPS concepts.
- Simulate DDoS scenarios.
- Analyze traffic using Wireshark.
- Explore enterprise-level DDoS mitigation techniques.

---

## Author

Gerrad Chibuye

Networking and Cybersecurity Learning Projects
