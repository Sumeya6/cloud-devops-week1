# Week 1: Linux Hands-on Lab — Project Workspace

A hands-on introduction to Linux command-line operations, file management, process inspection, and Git-based version control using Git Bash.

## Overview

This project demonstrates fundamental Linux commands used to manage files and directories, inspect running processes, and organize a development workspace. It was completed as part of the **Cloud & DevOps Track — Week 1 Hands-on Lab**.

## Learning Objectives

- Create and navigate directories using the Linux command line.
- Create, edit, and inspect text files.
- Organize files using directory operations.
- Search for files using `find`.
- Identify running processes and their Process IDs (PIDs).
- Document technical work and manage project files using Git and GitHub.

## Technology and Tools

| Tool | Purpose |
|---|---|
| Git Bash | Linux-style command-line environment on Windows |
| Bash commands | File, directory, and process operations |
| Git | Local version control |
| GitHub | Remote repository and project submission |

## Project Structure

```text
week1/
├── README.md
├── scripts/
│   └── notes.txt
└── screenshots/
    ├── 01-workspace.png
    ├── 02-notes-file.png
    ├── 03-scripts-directory.png
    ├── 04-moved-file.png
    ├── 05-find-file.png
    └── 06-process-pid.png
```

## Tasks and Implementation

### 1. Create the Project Workspace

Created the required directory structure and navigated to the working directory.

```bash
mkdir -p ~/cloud-devops/week1
cd ~/cloud-devops/week1
pwd
```

**Purpose:** `mkdir -p` creates the directory and any missing parent directories. `cd` changes the current working directory, while `pwd` displays its absolute path.

### 2. Create and Populate a Text File

Created `notes.txt` and added sample text.

```bash
touch notes.txt
echo "Week 1 Cloud and DevOps lab" > notes.txt
echo "I am learning Linux commands using Git Bash." >> notes.txt
echo "This is my first project workspace." >> notes.txt
cat notes.txt
```

**Purpose:** `touch` creates an empty file, `echo` writes text, `>` replaces file contents, `>>` appends text, and `cat` displays the contents.

### 3. Create the Scripts Directory

Created a directory named `scripts` to organize the project files.

```bash
mkdir scripts
ls
```

**Purpose:** `mkdir` creates a directory, while `ls` lists its contents.

### 4. Move the Text File

Moved `notes.txt` into the `scripts/` directory.

```bash
mv notes.txt scripts/
ls scripts/
```

**Purpose:** `mv` moves or renames files and directories. The listing verifies that the file is in its intended location.

### 5. Search for the File

Searched the workspace for `notes.txt`.

```bash
find ~/cloud-devops/week1 -name "notes.txt"
```

**Expected result:** The search returns the path to the file:

```text
~/cloud-devops/week1/scripts/notes.txt
```

The displayed path may begin with `/` and show the full filesystem location.

**Purpose:** `find` searches a directory hierarchy for files or directories matching specified criteria.

### 6. Inspect Running Processes

Used the `ps` command to display running processes and identify a Process ID (PID).

```bash
ps
```

**Purpose:** `ps` displays processes visible in the current Git Bash environment. The PID identifies a process, and the command or process-name column indicates what is running.

**Process observed:**

- Process name: `REPLACE_WITH_ACTUAL_PROCESS_NAME`
- PID: `REPLACE_WITH_ACTUAL_PID`

*Replace these placeholders with the actual process name and PID from your terminal output.*

## Evidence and Screenshots

The `screenshots/` directory contains terminal screenshots documenting the completion of the lab tasks.

| Screenshot | Evidence |
|---|---|
| `01-workspace.png` | Workspace creation and directory path |
| `02-notes-file.png` | File creation and text contents |
| `03-scripts-directory.png` | Creation of the `scripts/` directory |
| `04-moved-file.png` | File moved into `scripts/` |
| `05-find-file.png` | Successful file search |
| `06-process-pid.png` | Running process and PID |

## Key Learnings

Through this lab, I practiced:

- Navigating and organizing a project workspace through the command line.
- Creating and managing files and directories.
- Understanding file redirection and appending text.
- Searching for files in a directory hierarchy.
- Inspecting running processes and identifying PIDs.
- Documenting commands and results for reproducibility.

## Conclusion

This lab established a foundation in Linux command-line operations and project organization. These skills are useful for subsequent Cloud & DevOps activities involving shell scripting, system administration, Git workflows, and automation.

## Author

**Cloud & DevOps Track — Week 1**