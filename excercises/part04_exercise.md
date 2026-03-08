# Kali Linux Part 4 – Practice Exercises

These exercises help you practice:

- APT package management
- Installing and removing software
- Basic network scanning with Nmap
- Understanding open ports and services

Perform these tasks directly in the **Kali Linux terminal**.

---

# Section 1 – Package Management Basics

1. Open the terminal.

2. Update the system’s package list using APT.

3. Upgrade installed packages on the system.

4. Answer the following questions:

- What does the command `apt update` do?
- What does the command `apt upgrade` do?

---

# Section 2 – Installing Software

1. Install the following package: tree

2. After installation, run the command: tree

3. Observe what the command does.

4. Use APT to verify that the package was installed successfully.

---

# Section 3 – Removing Software

1. Remove the package you installed in the previous exercise.

2. Confirm that the program is no longer available.

3. Reinstall the package again.

4. Remove it completely using the **purge** command.

---

# Section 4 – Nmap Host Discovery

1. Check whether the following host is online: scanme.nmap.org


2. Use the correct **Nmap host discovery command**.

3. Observe the output and answer:

- Did the host respond?
- What information did Nmap return?

---

# Section 5 – Basic Port Scanning

1. Perform a basic scan on:

2. Observe the output.

3. Answer the following:

- How many ports were scanned by default?
- Which ports were open?

---

# Section 6 – Scanning Specific Ports

1. Use Nmap to scan the following ports only:

- 80
- 443

Example format: ```nmap -p <ports> <target>```


2. Record whether the ports are:

- open
- closed
- filtered

---

# Section 7 – Understanding the Output

After running your scans, answer the following questions:

1. What does an **open port** mean?

2. What does a **closed port** mean?

3. Why do hackers scan ports during reconnaissance?

---

# Challenge Exercise

Perform the following tasks:

1. Update the package list using APT.

2. Install a small tool such as: htop


3. Run the program.

4. Scan `scanme.nmap.org` using Nmap.

5. Identify at least **one open port** from the scan results.

6. Research which service usually runs on that port.

---

# Goal

By the end of these exercises you should be comfortable with:

- Installing and removing software using APT
- Updating and upgrading system packages
- Running basic Nmap scans
- Identifying open ports on a system

These skills form the foundation of **reconnaissance and system management in Kali Linux**.



