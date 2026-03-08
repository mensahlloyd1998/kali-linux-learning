# Kali Linux Part 2 -- Practice Exercises

These exercises reinforce the concepts from **Kali Linux Part 2**:

-   Piping
-   Copying files
-   Deleting files
-   Deleting directories

Work through the exercises directly in the **Linux terminal**.

------------------------------------------------------------------------

# Section 1 -- Practicing Piping

1.  Create a file called:

    users.txt

2.  Add the following lines to the file:

    user Lloyd logged in\
    admin logged in\
    user attempted login\
    guest logged in\
    user created account

3.  Display the file contents.

4.  Use **piping** to search for the word:

    user

5.  Use piping again to search for:

    admin

------------------------------------------------------------------------

# Section 2 -- Listing and Filtering Files

1.  Run a command to list files with detailed information.

2.  Use **piping with grep** to filter the output and display only lines
    containing:

    Desktop

3.  Try filtering another directory or filename.

------------------------------------------------------------------------

# Section 3 -- Copying Files

1.  Create a directory called:

    backup

2.  Copy the file:

    users.txt

    into the backup directory.

3.  Confirm that the file exists inside the directory.

4.  Create another copy of the file called:

    users_backup.txt

------------------------------------------------------------------------

# Section 4 -- Copying Directories

1.  Create a directory called:

    projects

2.  Inside **projects**, create a file named:

    notes.txt

3.  Copy the entire **projects directory** into:

    backup

4.  Verify that the directory and its contents were copied.

------------------------------------------------------------------------

# Section 5 -- Deleting Files

1.  Delete the file:

    users_backup.txt

2.  Confirm that the file no longer exists.

3.  Recreate the file and delete it again using **force deletion**.

------------------------------------------------------------------------

# Section 6 -- Deleting Directories

1.  Create a directory called:

    temp_folder

2.  Delete the directory using:

    rmdir

3.  Create the directory again.

4.  Add a file inside it.

5.  Try deleting it using `rmdir` again and observe what happens.

6.  Delete the directory using:

    rm -r

------------------------------------------------------------------------

# Challenge Exercise

1.  Create a directory called:

    cybersecurity_logs

2.  Inside it create a file named:

    log.txt

3.  Add several lines including the word:

    failed

4.  Use **piping with grep** to display only lines containing:

    failed

5.  Copy the directory into another directory called:

    archive

6.  Delete the original directory.

------------------------------------------------------------------------

# Goal

By the end of these exercises you should be comfortable with:

-   Using pipes to filter command output
-   Copying files and directories
-   Removing files safely
-   Removing directories recursively

Practice these commands until you can run them **without referring to
your notes**.
