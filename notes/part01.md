
# Kali Linux – Part 1

### Basic Terminal Commands and File Operations

Kali Linux is a Linux distribution widely used for **ethical hacking, penetration testing, and cybersecurity research**. Most operations in Kali are performed through the **terminal emulator**, which allows users to interact with the operating system using commands.

---

# 1. Terminal Basics

The **terminal emulator** allows users to execute Linux commands to interact with the system.

### Display Current User

```
whoami
```

Shows the **username of the currently logged-in user**.

---

### Display Hostname

```
hostname
```

Shows the **name of the computer (host)** currently in use.

---

### Display Current Date and Time

```
date
```

Displays the **current system date and time**.

---

### Show Current Working Directory

```
pwd
```

`pwd` stands for **Print Working Directory**.
It shows the **full path of the directory you are currently in**.

Example:

```
/home/kali/Desktop
```

---

### Show Command History

```
history
```

Displays a list of **previous commands executed in the terminal**.

---

# 2. Listing Files and Directories

The `ls` command is used to **list files and directories**.

---

### List Files in Current Directory

```
ls
```

---

### List All Files (Including Hidden Files)

```
ls -a
```

Hidden files in Linux start with a **dot (.)**.

Example:

```
.bashrc
.profile
```

---

### List Files with Detailed Information

```
ls -l
```

Displays details such as:

* file permissions
* owner
* group
* file size
* last modified date

---

### Human Readable File Sizes

```
ls -lh
```

Displays file sizes in **KB, MB, or GB** instead of bytes.

---

### List Files in Another Directory

```
ls Desktop
```

Shows the files inside the **Desktop directory** without moving into it.

---

# 3. Changing Directories

The `cd` command means **Change Directory**.

---

### Move into a Directory

```
cd Desktop
```

Moves from the current directory into the **Desktop directory**.

---

### Go to Home Directory

```
cd
```

Moves to the **home directory** of the current user.

Example:

```
/home/kali
```

---

# 4. Creating Directories

The `mkdir` command is used to **create new directories (folders)**.

---

### Create a Directory

```
mkdir foldername
```

Creates a new directory called **foldername** in the current directory.

---

### Create Nested Directories

```
mkdir -p parentname/directoryname
```

The `-p` option allows you to **create parent directories if they do not already exist**.

Example:

```
mkdir -p projects/test
```

This creates:

```
projects/
    test/
```

---

# 5. Nano Text Editor

**Nano** is a simple command-line text editor used to create and edit files.

---

### Create or Open a File

```
nano filename.txt
```

If the file **does not exist**, Nano will create a new one.

---

### Save a File

Press:

```
CTRL + O
```

Then press **Enter** to confirm the filename.

---

### Exit Nano

Press:

```
CTRL + X
```

---

# 6. Grep Command

**GREP** stands for:

**Global Regular Expression Print**

It is used to **search for text patterns inside files**.

---

### View Grep Help

```
grep --help
```

Shows all available options.

---

### Search for a Word in a File

```
grep -n 'user' textfile.txt
```

Options used:

* `-n` → shows the **line number** where the word appears

Example output:

```
5:user Lloyd logged in
```

Meaning the word **user** appears on **line 5**.

---

# 7. WC Command

`wc` stands for **Word Count**.

It is used to count:

* words
* lines
* characters

---

### Count Words in a File

```
wc -w file.txt
```

Returns the **number of words**.

---

### Count Lines in a File

```
wc -l file.txt
```

Returns the **number of lines** in the file.

---

# Summary

Important commands covered in this section:

| Command  | Purpose                            |
| -------- | ---------------------------------- |
| whoami   | Shows current user                 |
| hostname | Shows system hostname              |
| date     | Shows current date and time        |
| pwd      | Shows current directory            |
| history  | Shows previously executed commands |
| ls       | Lists files and directories        |
| cd       | Changes directory                  |
| mkdir    | Creates directories                |
| nano     | Text editor                        |
| grep     | Searches text patterns             |
| wc       | Counts words or lines              |

---

If you want, I can also help you create **Kali Linux Part 2**, where we cover the next **essential commands ethical hackers must know**, like:

* `cp`, `mv`, `rm`
* `touch`
* `chmod`
* `chown`
* `find`
* `cat`, `less`, `head`, `tail`
* piping (`|`)
* redirection (`>`, `>>`)
* package management (`apt`)

Those commands are **used constantly during penetration testing**.
