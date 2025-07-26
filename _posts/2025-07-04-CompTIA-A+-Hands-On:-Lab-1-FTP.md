---
title: "Comp TIA A+ Hands On: Lab 1 - FTP"
date: 2025-07-04 11:59:00 +0800
categories: [IT]
tags: []
media_subpath: /assets/
---

# Lab Number and Title: 
Lab01 “Remote File Access -- FTP”

##Objective: 
Learn how to save configurations using File Transfer Protocol.
(Back up your router configuration using File Transfer Protocol) 

## Lab Tool: 
Cisco Packet Tracer

## Lab Topology:
![Desktop View](/lab01comptiaA+.png)


## Steps Taken:
1. Connect a router to a server using a crossover cable
2. Assigned an IP address and default gateway to the server
3. Assigned an IP address to the router
4. Pinged the router from the server (successful)
5. Saved the routers configuration using ‘copy run start’ command
6. Configured FTP credentials on the server
7. Added the FTP username and password to the router
8. Copied the router configuration to the FTP server
9. Ensured that the file was on the FTP server

## Issues Encountered:
Problem: Crossover cable had 2 red arrows. Determined to be caused by the cable not being activated or is not working correctly.
Solution: Turned on the router's port labeled “GigabitEthernet0/0”. Connection is now established between the router and server.
Lesson learned: Check configs.

Problem: When attempting to assign an IP address to the router, I receive an error saying “%Invalid interface type and number”
Solution: Checked Interface configs. Interface is named “GigabitEthernet0/0”
Lesson learned: Manually check configs to get interface or device names.

Problem: When attempting to run the ‘copy run start’ command to save the routers configurations, I get the error “Router(config)#copy run start^% Invalid input detected at '^' marker.”
Solution: Run the command in privileged mode instead of global configuration mode. Used ‘exit’ command to exit global config mode and enter privileged mode.
Lesson learned: Make sure you are in the right ‘mode’ when setting up a router using the CLI tool.

## Key Concepts or Commands:
‘copy run start’ - used in Cisco devices to save the current active configuration (running-config) to the non-volatile memory (startup-config), ensuring the changes persist after a reboot

## Takeaways:
I learned how to set up FTP credentials on a file server and save those credentials on a router. I also learned how to use FTP to transfer a back-up copy of the router's configuration file from a router to a server.

## Real-World Application:
I have gained a better understanding of FTP and how to configure it on both a file server and router to enable back-up file transfers over the network.
