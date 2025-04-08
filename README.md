# splunk-cluster-mini-cybersecurity
This project simulates a basic Splunk cluster on a single laptop using virtual machines (VMs). 
It's designed to demonstrate how log data flows from systems to a centralized platform for 
analysis, detection, and monitoring in a cybersecurity context.

 --------------------------------------------------------------------------------------------
 🎯 **Objective**
 Build a lightweight, virtualized Splunk cluster to:
    * Centralize and analyze system logs
    * Simulate security incidents (e.g. failed logins)
    * Detect and monitor potential threats
    * Showcase cybersecurity and log management skills

--------------------------------------------------------------------------------------------
🛠 **Environment**
    * Host Machine: Laptop with Intel celeron 4205U 1.8GHz - 2 cores, 2 threads
    * Virtualization Software: QEMU/KVM
    * Guest OS: Ubuntu Server (CLI only)
    * Number of VMs: 3
    * Search Head (splunk-searchhead)
    * Indexer (splunk-indexer)
    * Forwarder (splunk-forwarder)

--------------------------------------------------------------------------------------------
🧱 **Architecture**
![Splunk Architecture](https://github.com/user-attachments/assets/c883923a-5b2e-45c3-a74a-8c0c0b01a224)

--------------------------------------------------------------------------------------------
 🔐 Networking
    * All VMs use Host-only Adapter for private communication.
    * IPs are manually assigned for simplicity.

--------------------------------------------------------------------------------------------
📥 **Splunk Components**
    >> $ Indexer
    - Receives logs from the forwarder
    - Indexes and stores the data
    >> $ Search Head
    - Runs user searches
    - Visualizes data with dashboards and alerts
    >> $ Universal Forwarder
    - Sends log data from its VM (simulating a real server)

--------------------------------------------------------------------------------------------
🧠 **Use Cases**
    * Monitor failed SSH login attempts
    * Detect brute-force attacks
    * Visualize system event logs in real-time

--------------------------------------------------------------------------------------------
🧾 **License**
This project is for educational and demonstration purposes only. Not intended for production 
use but for public use. you can take use the documantation to setup our own splunk cluster 
for production.

