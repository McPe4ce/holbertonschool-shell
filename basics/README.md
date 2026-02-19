# Holberton School Project: BASICS

This README contains all the commands used in the **BASICS** project at Holberton School.  
It explains each command and what it does in the shell.

---

## 📁 Directory & File Commands

### 0 - Print Working Directory

```bash
pwd
```

Prints the current working directory.

---

### 1 - List Directory Contents

```bash
ls
```

Displays the files and directories in the current working directory.

---

### 2 - Change Directory to Home

```bash
cd
```

Changes the current working directory to the user's home directory.

---

### 3 - Long Format Listing

```bash
ls -l
```

Displays files in **long format**, showing permissions, owner, size, and modification date.

---

### 4 - List All Files (Including Hidden)

```bash
ls -la
```

Displays all files, including hidden ones (files starting with `.`), in long format.

---

### 5 - List All Files with UID & GID

```bash
ls -lan
```

Displays all files with **user ID (UID)** and **group ID (GID)** in long format.

---

### 6 - Create a Directory

```bash
mkdir /tmp/my_first_directory
```

Creates a new directory named `my_first_directory` inside `/tmp`.

---

### 7 - Move a File

```bash
mv betty /tmp/my_first_directory
```

Moves the file `betty` from the current location to `/tmp/my_first_directory`.

---

### 8 - Delete a File

```bash
rm /tmp/my_first_directory/betty
```

Deletes the file `betty`.

---

### 9 - Remove a Directory

```bash
rmdir /tmp/my_first_directory
```

Deletes the directory `my_first_directory` (only if it is empty).

---

### 10 - Change to Previous Directory

```bash
cd ..
```

Moves to the **parent directory** (one level up).

---

### 11 - List Files in Multiple Locations

```bash
ls . .. -la /boot
```

- `.` → current directory  
- `..` → parent directory  
- `/boot` → boot directory  

Lists all files (including hidden ones) in all specified locations in **long format**.

---

### 12 - Check File Type

```bash
file /tmp/iamafile
```

Prints the type of a file (text, binary, executable, etc.).

---

### 13 - Create a Symbolic Link

```bash
ln -s /bin/ls __ls__
```

Creates a **symbolic link** named `__ls__` pointing to `/bin/ls`.

---

### 14 - Move and Update Files

```bash
mv -u *.html ..
```

Moves all `.html` files to the **parent directory** only if they **do not exist there** or are **updated** (`-u`).

---

### 15 - Move Files Starting with Uppercase

```bash
mv [A-Z]* /tmp/u
```

Moves all files starting with an uppercase letter to `/tmp/u`.

---

### 16 - Delete Backup Files Forcefully

```bash
rm -f *~
```

Deletes all files ending with `~` in the current directory.  
- `-f` → force deletion without confirmation

---

### 17 - Create Nested Directories

```bash
mkdir -p welcome/to/school
```

Creates a directory tree:

```
/welcome
/welcome/to
/welcome/to/school
```

- `-p` → create parent directories as needed

---

## ✅ Summary

This README covers basic shell commands including:

- Navigation (`pwd`, `cd`)  
- Listing files (`ls`)  
- File operations (`mv`, `rm`, `mkdir`)  
- Linking (`ln`)  
- File type inspection (`file`)  

These commands form the foundation for daily shell usage in the Holberton School BASICS project.

