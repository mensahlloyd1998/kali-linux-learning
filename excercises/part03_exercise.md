
```
exercises/kali-part-3-exercises.md
```

---

```markdown
# Kali Linux Part 3 – Practice Exercises

These exercises help you practice **Linux user management and administrative privileges**.

Topics covered:

- User types
- Root vs regular user
- sudo command
- Checking user permissions
- Understanding user IDs and groups

Try to complete the exercises directly in the **Kali Linux terminal**.

---

# Section 1 – Understanding Users

Answer the following questions:

1. What does it mean that Linux is a **multi-user operating system**?

2. List the **three types of users in Linux**.

3. Which user has **full administrative privileges**?

4. Why is it dangerous to work directly as the **root user**?

5. What symbol usually represents:

- a regular user prompt?
- a root user prompt?

---

# Section 2 – Checking Your Current User

1. Open the terminal.

2. Run the command that displays your **current username**.

3. Verify whether you are logged in as a **regular user or root user**.

4. Run the following command to display user information:

```

id

```

5. Write down:

- your **UID**
- your **GID**
- the **groups** you belong to

---

# Section 3 – Checking Another User

1. Use the following command to check information about another user:

```

id username

```

Example:

```

id root

```

2. Observe the output and answer:

- What is the UID of the root user?
- Which group does the root user belong to?

---

# Section 4 – Practicing sudo

1. Run the following command to update the system package list:

```

sudo apt update

```

2. Observe what happens.

3. Answer the following:

- Does the system ask for a password?
- Which password is required?

4. Install a simple package using sudo.

Example:

```

sudo apt install tree

```

5. Run the program after installation.

---

# Section 5 – Root vs Regular User

1. Run the following command:

```

whoami

```

2. Switch to the root user (if permitted):

```

sudo su

```

3. Run the command again:

```

whoami

```

4. Observe the terminal prompt.

Questions:

- What symbol appears in the terminal when you are root?
- What command returns you to the regular user?

Hint:

```

exit

```

---

# Challenge Exercise

Perform the following tasks:

1. Check your user information using the **id command**.

2. Verify whether your user belongs to the **sudo group**.

3. Install a package using **sudo**.

4. Confirm that the package installed successfully.

5. Return to your normal user environment if you switched to root.

---

# Goal

By the end of these exercises you should understand:

- The difference between **regular users, system users, and root**
- How **administrative privileges** work in Linux
- How to safely run commands using **sudo**
- How to check **user and group information**

User permissions are a **critical concept in Linux security and penetration testing**.
```

