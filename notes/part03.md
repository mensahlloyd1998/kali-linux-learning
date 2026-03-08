# Kali Linux -- Part 3

## User Management and Administration

Linux is designed as a **multi-user operating system**, meaning multiple
users can access and use the same system at the same time.\
Because of this, Linux implements a **permission and access control
system** to ensure security and proper system management.

Different users have different **levels of access and permissions**
depending on their role.

------------------------------------------------------------------------

# 1. Multi‑User Systems

A **multi-user system** allows several users to:

-   Access the system
-   Run programs
-   Use system resources

at the same time without interfering with each other.

Each user has their own:

-   username
-   home directory
-   permissions

This structure helps keep the system secure and organized.

------------------------------------------------------------------------

# 2. Types of Users in Linux

There are three main types of users in Linux.

## 1. Regular Users

Regular users are standard accounts created for everyday tasks.

Characteristics:

-   Limited permissions
-   Cannot perform administrative tasks by default
-   Used for normal activities such as editing files, browsing, or
    running applications

This limitation helps protect the system from accidental or malicious
damage.

------------------------------------------------------------------------

## 2. System Users

System users are accounts created automatically by the operating system
or installed applications.

Characteristics:

-   Used to run services and background processes
-   Usually do not log in interactively
-   Help manage system services such as databases, web servers, and
    network services

Example services that may use system users:

-   web servers
-   databases
-   background daemons

------------------------------------------------------------------------

## 3. Root User

The **root user** is the most powerful account in Linux.

Characteristics:

-   Full administrative access
-   Can read, modify, or delete any file
-   Can install or remove software
-   Can create or delete users
-   Can change system configuration

Because of this unrestricted access, the root account is also called the
**superuser**.

Improper use of the root account can damage the system.

------------------------------------------------------------------------

# 3. Command Prompt Symbols

Linux terminals often display different symbols depending on the user.

Regular user prompt:

\$

Root user prompt:

# 

Example:

Regular user:

kali@machine:\~\$

Root user:

root@machine:\~#

------------------------------------------------------------------------

# 4. Performing Administrative Tasks

Administrative tasks require **root privileges**.

There are two ways to run administrative commands:

1.  Log in as the **root user**
2.  Use the **sudo command**

Logging in as the root user can be risky for beginners because commands
run with full system power.

For safety, it is recommended to use **sudo instead of logging in as
root**.

------------------------------------------------------------------------

# 5. The sudo Command

`sudo` stands for:

Super User Do

It allows a regular user to execute commands with **administrative
privileges**.

Syntax:

sudo command

Example:

sudo apt install vlc

Explanation:

-   `apt` is the package manager used in Debian-based systems like Kali
    Linux
-   `install vlc` installs the VLC media player
-   `sudo` grants the command temporary administrative privileges

When using sudo, the system usually asks for the **user's password** to
confirm authorization.

------------------------------------------------------------------------

# 6. Who Can Use sudo?

Not all users can run sudo commands.

By default:

-   The user account created during **OS installation** is granted sudo
    privileges.
-   This user belongs to the **sudo group**.

System administrators can grant or remove sudo privileges for other
users.

------------------------------------------------------------------------

# 7. Checking User Information

The `id` command is used to display information about a user.

It shows:

-   user ID (UID)
-   group ID (GID)
-   groups the user belongs to

Syntax:

id username

Example:

id kali

Example output:

uid=1000(kali) gid=1000(kali) groups=1000(kali),27(sudo)

This means:

-   the user **kali** belongs to the **sudo group**
-   the user can execute administrative commands using sudo

------------------------------------------------------------------------

# Summary

Concepts covered in this section:

| Concept \| Description \|

\|-------\|-------------\| Linux Multi‑User System \| Allows multiple
users to access a system \| \| Regular User \| Standard user with
limited permissions \| \| System User \| Used by services and background
processes \| \| Root User \| Superuser with full administrative access
\| \| sudo \| Allows regular users to run administrative commands \| \|
id command \| Displays user and group information \|

------------------------------------------------------------------------

# Key Takeaway

Understanding **user permissions and privilege management** is essential
in cybersecurity.

Ethical hackers and system administrators must understand:

-   which users have administrative privileges
-   how permissions are assigned
-   how privilege escalation can occur

User management is a fundamental concept in **Linux security and
penetration testing**.
