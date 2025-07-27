---
title: "Comp TIA A+ Hands On: Lab 5 - DNS"
date: 2025-07-27 11:59:00 +0800
categories: [IT]
tags: []
media_subpath: /assets/
---

# Lab Number and Title: 
Lab05 - DNS
## Objective: 
Learn how the Domain Name System works.
## Lab Tool: 
Wireshark
## Lab Topology:
![Desktop View](/lab05topology.drawio.png)

## Steps Taken:
 1. Captured internet activity over a two minute time period using wireshark. Searched for ‘www.101labs.net’ using my internet browser during the capture.
 2. Filtered the packets with the display filter ‘dns’ to see all the DNS queries and responses made during the packet capture.
 3. Analyzed the first DNS query; used the default DNS port 53 and was transmitted over UDP since the response did not require more than 512 bytes.
 4. Analyzed the first DNS response; an IP address was directly returned for ‘www.101labs.net’

## Key Concepts: 
When you search for a website, your computer sends a DNS query to a DNS server that either responds with the IP address if it has it or forwards the request to another DNS server. Eventually, a DNS response is sent back with the correct IP address for the requested domain.

