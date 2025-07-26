---
title: "Comp TIA A+ Hands On: Lab 2 - SSH"
date: 2025-07-26 11:59:00 +0800
categories: [IT]
tags: []
media_subpath: /assets/
---

Lab Number and Title: Lab02 “SSH”
 Date Completed: 04 July 25
 
 Objective: Learn and understand how to enable SSH (Secure Shell Script) access to a device.
 
 Lab Tool: Cisco Packet Tracer
 
 Lab Topology:
 ![Desktop View](/lab02topology.png)

Steps Taken:
 1. Configured hostname ‘R1’ on Router1. 
 2. Assigned IP addresses to each interface, used ‘ping’ command to ensure connectivity.
 3. Secured Router1 so that it accepts incoming SSH connections. Set a domain name and generated keys. Password attempts restricted to 2 and set a timeout after 120 seconds of inactivity.
 4. Connected to Router1 from PC using SSH.
 5. Attempted to Telnet from the PC to Router1 to ensure the connection was refused.

Key Concepts/Commands:
‘Ping’ - network diagnostic tool used to test connectivity between your device and another device on a network
‘Ip domain-name’ - command in Cisco IOS is used to set the domain name of the device. This is especially important when configuring SSH access or generating cryptographic keys.
‘crypto key generate RSA’ - generates RSA key pairs used for enabling secure communication, primarily SSH (Secure Shell) access to a Cisco device.

