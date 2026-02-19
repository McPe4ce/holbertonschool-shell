# Holberton School Project: PERMISSIONS

This project explores **file ownership and permission management** in Linux.  
It demonstrates how to:

- Switch users  
- Inspect and manage file permissions  
- Change ownership and groups  
- Apply permissions for users, groups, and others  

This README explains each command used in the **Permissions** project.

---

## 🔹 0 - Switch User

```bash
su betty
```

Changes the current user to `betty`.

---

## 🔹 1 - Print Current Username

```bash
whoami
```

Displays the username of the current user.

---

## 🔹 2 - Print User Groups

```bash
groups
```

Shows all groups the current user belongs to.

---

## 🔹 3 - Change File Owner

```bash
chown betty hello
```

Changes the **owner** of the file `hello` to `betty`.

---

## 🔹 4 - Create an Empty File

```bash
touch hello
```

Creates a new empty file named `hello`.

---

## 🔹 5 - Add Execute Permission for User

```bash
chmod u+x hello
```

Grants **execute** permission to the **user/owner** of the file.

---

## 🔹 6 - Add Execute/Read Permissions

```bash
chmod u+x,g+x,o+r hello
```

Grants:

- Execute to **user** (`u`) and **group** (`g`)  
- Read to **others** (`o`)

---

## 🔹 7 - Add Execute Permission to All

```bash
chmod ugo+x hello
```

Adds **execute** permission to **user, group, and others**.

---

## 🔹 8 - Set Permissions with Octal Mode

```bash
chmod 007 hello
```

- Removes all permissions from **user** and **group**  
- Grants **all permissions** (read/write/execute) to **others**

---

## 🔹 9 - Set Custom Permissions

```bash
chmod 753 hello
```

Sets a specific combination of permissions for **user, group, and others**.

---

## 🔹 10 - Mirror Permissions from Another File

```bash
chmod --reference hello olleh
```

Applies the same permissions from `hello` to the file `olleh`.

---

## 🔹 11 - Add Execute to All Files in Directories

```bash
chmod a+x */
```

Gives **execute permissions** to **all users** for directories (`*/`).

---

## 🔹 12 - Create Directory with Specific Mode

```bash
mkdir -m 751 my_dir
```

Creates `my_dir` with permission mode `751`:

- `7` → user: read/write/execute  
- `5` → group: read/execute  
- `1` → others: execute only

---

## 🔹 13 - Change Group Ownership

```bash
chgrp school hello
```

Changes the **group owner** of `hello` to `school`.

---

## 🔹 14 - Change Owner and Group for All Files

```bash
chown vincent:staff *
```

Changes **user** to `vincent` and **group** to `staff` for **all files** in the directory.

---

## 🔹 15 - Change Symbolic Link Ownership

```bash
chown -h vincent:staff _hello
```

Changes permissions for a **symbolic link** itself, not the file it points to.  
- `-h` ensures the link is modified.

---

## 🔹 16 - Conditional Ownership Change

```bash
chown --from=guillaume vincent hello
```

Changes the owner of `hello` to `vincent` **only if** the current owner is `guillaume`.

---

## Key Concepts Learned

- Switching users (`su`)  
- Checking current user and groups (`whoami`, `groups`)  
- File ownership and group changes (`chown`, `chgrp`)  
- Basic and advanced permissions (`chmod` with symbolic & octal modes)  
- Creating files and directories (`touch`, `mkdir`)  
- Handling symbolic links and conditional ownership changes  

---

## Author

Permissions project from **Holberton School**.
