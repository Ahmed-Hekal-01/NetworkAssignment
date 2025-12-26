# OSPF Dynamic Routing Lab (GNS3)

**Student:** Omar Ahmed Elwekeil
**ID:** 320230172
**Subject:** Computer Networks
**Date:** December 26, 2025

---

## 1. Justification for Using GNS3

I have chosen to implement this lab using **GNS3 (Graphical Network Simulator-3)** instead of **Cisco Packet Tracer** for this reasons:

* My development environment is **Arch Linux**. Cisco Packet Tracer is proprietary software primarily **built for Windows and older Ubuntu distributions**, making it unstable and difficult to run natively on Arch Linux. GNS3, conversely, offers superior native support and performance on Arch, ensuring a stable testing environment. :)
---

## 2. Project Topology Overview

* **Routers:** 3x Cisco 7200 (IOS c7200-jk9s-mz.124-13b)
* **Routing Protocol:** OSPF (Area 0)
* **End Devices:** 2x VPCS (Virtual PCs)
* **Connectivity:** Serial links for WAN (Routers) and FastEthernet for LAN segments.

---

## 3. Instructions for Testing the Project

To verify the topology and connectivity, please follow these steps:

1.  **Open the Project:**
    * Launch GNS3. (you should open the GNS3 first then open the project from it)
    * Go to **File > Open Project** and select the `.gns3` file located in the project directory.

2.  **Start the Network:**
    * Click the **Green "Play" button** in the top toolbar to power on all routers, switches, and PCs.
    * *Note: Please wait approximately 30 seconds for the routers to boot and for OSPF neighbors to reach the "FULL" state.*

3.  **Verify Connectivity:**
    * Right-click on **PC1** and select **Console**.
    * In the terminal window, run the ping command to reach PC2:
        ```bash
        ping 192.168.2.2
        ```
