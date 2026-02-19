# Holberton Shell

Welcome to the **Holberton Shell** repository!  

This repository contains my work on the Holberton School **Shell projects**, designed to teach the fundamentals of the Linux shell, file management, permissions, redirection, and text processing.  

The projects are organized to build a strong foundation in both **practical command usage** and **conceptual understanding** of the shell environment.

---

## Introduction to the Shell

The shell is a **command-line interface** that allows users to interact with the operating system. Key concepts include:

- **RTFM** → “Read The Fine Manual” – a reminder to consult documentation.  
- **Shebang (`#!`)** → Indicates the interpreter for a script.  
- **Shell vs Terminal** → The shell interprets commands; the terminal displays the interface.  
- **Shell prompt** → The line where the shell waits for input.  
- **History** → Access previously executed commands using the `history` command or arrow keys.

---

## Navigation

Understanding filesystem navigation is essential:

- `cd`, `pwd`, `ls` → core commands to move around and list directories.  
- **Working directory** → The current location in the filesystem.  
- `.` → current directory, `..` → parent directory.  
- **Root directory (`/`)** → top of the filesystem hierarchy.  
- **Home directory** → the personal workspace of a user.  
- Hidden files → start with `.`; listed with `ls -a`.  
- `cd -` → switch to the previous working directory.

---

## Looking Around

Commands to explore the filesystem and files:

- `ls`, `less`, `file` → listing and inspecting files.  
- Options and arguments modify command behavior.  
- **Long listing format (`ls -l`)** provides detailed information about files.

---

## A Guided Tour

Understanding links and directories:

- `ln` → creates links between files.  
- **Symbolic link** → a pointer to another file.  
- **Hard link** → another directory entry pointing to the same inode.  
- Difference: symbolic links can cross filesystems, hard links cannot.

---

## Manipulating Files

Basic file operations:

- `cp` → copy files  
- `mv` → move or rename files  
- `rm` → remove files  
- `mkdir` → create directories  
- **Wildcards (`*`, `?`, `[A-Z]`)** → match multiple files efficiently.

---

## Working with Commands

Learn how to inspect and manage commands:

- `type`, `which` → identify command type and path.  
- `help`, `man` → access documentation.  
- **Aliases** → create shortcuts for frequently used commands.  
- Use `help` for shell built-ins; `man` for system-wide documentation.

---

## Reading Man Pages

Man pages explain commands in detail:

- Sections include:  
  1. User commands  
  2. System calls  
  3. Library functions  
- Reading man pages requires understanding sections and syntax.

---

## Keyboard Shortcuts for Bash

Common shortcuts:

- `Ctrl + A` → move to beginning of line  
- `Ctrl + E` → move to end of line  
- `Ctrl + R` → reverse search through history  
- `Ctrl + L` → clear screen  

---

## Long-Term Support (LTS)

- LTS ensures stable and supported versions of software.  
- Recommended for production and learning environments.

---

## Projects

This repository contains **four main Holberton Shell projects**, each building essential skills:

### 1. BASICS
Covers **fundamental commands**: navigation, listing files, creating and moving directories, and exploring file types.

### 2. VARIABLES & PRINTF
Focuses on **shell variables**, environment variables, arithmetic operations, and formatted output using `printf`.

### 3. PERMISSIONS
Covers **file ownership and permission management**, including symbolic and hard links, `chmod`, `chown`, and group management.

### 4. REDIRECTION & FILTERS
Introduces **redirecting command output**, **piping**, and using filters to process data (`grep`, `sort`, `uniq`, `cut`, `tr`, `rev`).

---

## Author

Holberton Shell projects by **[Your Name]** – Holberton School.
