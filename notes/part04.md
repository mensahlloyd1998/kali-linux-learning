
---

# Kali Linux – Part 4

## Package Management and Network Scanning

This section introduces two important concepts in Kali Linux:

* **APT package management**
* **Network scanning with Nmap**

These tools are frequently used by cybersecurity professionals, system administrators, and ethical hackers.

---

# 1. APT Package Manager

Kali Linux is based on **Debian Linux**, which uses the **APT (Advanced Package Tool)** package manager.

APT is used to:

* install software
* update software
* remove software
* manage system packages

Most APT commands require **administrative privileges**, so they are usually run with `sudo`.

---

## Update Package Lists

Before installing software, update the package index.

```
sudo apt update
```

This command refreshes the list of available packages from the repositories.

---

## Upgrade Installed Packages

To upgrade all installed packages to their latest versions:

```
sudo apt upgrade
```

This installs the newest versions of the software already installed on the system.

---

## Install a Package

To install software:

```
sudo apt install package_name
```

Example:

```
sudo apt install vlc
```

This installs the **VLC media player**.

---

## Remove a Package

To remove installed software:

```
sudo apt remove package_name
```

Example:

```
sudo apt remove vlc
```

---

## Remove Package and Configuration Files

To completely remove a package including configuration files:

```
sudo apt purge package_name
```

---

# 2. Nmap – Network Mapper

Nmap is a powerful **network scanning and reconnaissance tool** used in cybersecurity.

It is commonly used for:

* discovering hosts on a network
* identifying open ports
* detecting running services
* gathering information about target systems

Nmap is one of the **most important tools in penetration testing**.

---

# 3. Important Legal Warning

Network scanning without permission may be **illegal**.

Only scan:

* systems you own
* systems you have permission to test
* official practice targets

A safe public target provided by the Nmap developers is:

```
scanme.nmap.org
```

---

# 4. Checking if a Host Is Online

Before performing a full scan, you may want to check if the host is **alive**.

This is called a **ping scan**.

```
nmap -sn <target_ip_or_domain>
```

Example:

```
nmap -sn scanme.nmap.org
```

The `-sn` option tells Nmap to:

* discover hosts
* skip port scanning

---

# 5. Scanning a Target

To perform a basic scan:

```
nmap <target_ip_or_domain>
```

Example:

```
nmap scanme.nmap.org
```

By default, Nmap scans the **1000 most common ports**.

The scan will attempt to identify:

* open ports
* closed ports
* filtered ports

---

# 6. Scanning Specific Ports

You can scan specific ports using the `-p` option.

Example:

```
nmap -p 80,443 scanme.nmap.org
```

This scans:

* port 80 (HTTP)
* port 443 (HTTPS)

---

# Summary

Commands introduced in this section:

| Command            | Purpose                    |
| ------------------ | -------------------------- |
| `sudo apt update`  | Update package list        |
| `sudo apt upgrade` | Upgrade installed packages |
| `sudo apt install` | Install software           |
| `sudo apt remove`  | Remove software            |
| `nmap -sn`         | Check if host is online    |
| `nmap target`      | Scan most common ports     |
| `nmap -p`          | Scan specific ports        |

---

# Key Takeaway

Understanding package management and network scanning is essential for cybersecurity.

* **APT** helps manage software in Kali Linux.
* **Nmap** helps gather information about networks and systems.

Information gathering is the **first phase of penetration testing**, often called **reconnaissance**.

---

