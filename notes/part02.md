# Kali Linux -- Part 2

## Piping and File Management

This section continues the Kali Linux basics and focuses on **piping
commands and basic file management**. These concepts are important
because penetration testers and system administrators often combine
commands to process data quickly.

------------------------------------------------------------------------

# 1. Piping

**Piping** allows the output of one command to be used as the input for
another command.

The pipe operator is:

| 

This makes it possible to **chain commands together**, which saves time
and avoids creating temporary files.

General syntax:

command1 \| command2

`command1` produces output, and that output becomes the input for
`command2`.

------------------------------------------------------------------------

## Example 1

cat output.txt \| grep 'user'

Explanation:

-   `cat output.txt` displays the contents of the file
-   `grep 'user'` searches for lines containing the word **user**

Using the pipe sends the output of `cat` directly to `grep`, which then
filters the results.

------------------------------------------------------------------------

## Example 2

ls -l \| grep 'Desktop'

Explanation:

-   `ls -l` lists files with detailed information
-   `grep 'Desktop'` filters the results and only shows lines containing
    **Desktop**

------------------------------------------------------------------------

## Why Piping Is Powerful

Instead of doing this:

1.  Run a command
2.  Save the result to a file
3.  Search that file

You can do everything in **one command** using pipes.

Example:

cat log.txt \| grep 'failed'

This quickly shows **failed login attempts** in a log file.

------------------------------------------------------------------------

# 2. Copying Files

The `cp` command is used to **copy files and directories**.

General syntax:

cp source destination

------------------------------------------------------------------------

## Copy a File to Another Directory

cp filename.txt directoryname/

Example:

cp notes.txt Desktop/

This copies `notes.txt` to the **Desktop directory**.

------------------------------------------------------------------------

## Copy and Rename a File

cp oldname.txt newname.txt

Example:

cp report.txt backup_report.txt

This creates a copy of the file with a **new name**.

------------------------------------------------------------------------

## Copy Directories

To copy a directory and everything inside it, use the **recursive
option**.

cp -r directoryname destination/

Example:

cp -r projects backup/

The `-r` flag means **recursive**, which allows the command to copy:

-   folders
-   subfolders
-   files inside them

------------------------------------------------------------------------

# 3. Deleting Files

The `rm` command is used to **delete files**.

Example:

rm filename.txt

This permanently deletes the file.

Important: Files deleted with `rm` **do not go to a recycle bin**.

------------------------------------------------------------------------

# 4. Deleting Directories

To delete an empty directory:

rmdir directoryname

Example:

rmdir test_folder

------------------------------------------------------------------------

# 5. Deleting Non-Empty Directories

If a directory contains files, use the recursive remove command:

rm -r directoryname

Example:

rm -r old_projects

This deletes:

-   the directory
-   all files inside it
-   all subdirectories

------------------------------------------------------------------------

# 6. Force Deletion

Sometimes Linux will ask for confirmation when deleting files.

To force deletion without confirmation:

rm -f filename.txt

To force delete a directory and everything inside:

rm -rf directoryname

Be extremely careful with this command.

Example:

rm -rf /

This would attempt to delete the entire system.

------------------------------------------------------------------------

# Summary

Commands covered in this section:

  Command   Purpose
  --------- ------------------------------------------
  \|        Pipes output from one command to another
  cp        Copies files
  cp -r     Copies directories recursively
  rm        Deletes files
  rmdir     Deletes empty directories
  rm -r     Deletes directories with contents
  rm -rf    Force deletes directories and files

------------------------------------------------------------------------

# Key Takeaway

Combining commands with **pipes** and managing files efficiently are
core Linux skills.

Ethical hackers frequently use these techniques when:

-   analyzing log files
-   filtering command output
-   moving or backing up files
-   cleaning up testing environments
