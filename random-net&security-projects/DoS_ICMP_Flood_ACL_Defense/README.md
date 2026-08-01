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
