# Holberton School Project: REDIRECTION & FILTERS

This project covers **redirection and filtering commands** in the shell.  
It demonstrates how to:

- Print and manipulate text  
- Redirect output to files  
- Use filters to process file content  
- Search and extract information  

This README explains each command used in the project.

---

## 🔹 0 - Print Text

```bash
echo "Hello, World"
```

Prints the text `"Hello, World"` to the terminal.

---

## 🔹 1 - Escape Characters

```bash
echo "\"(Ôo)'"
```

- The `\` cancels the special meaning of the character that follows it.

---

## 🔹 2 - View File Content

```bash
cat /etc/passwd
```

Displays the content of a file.

---

## 🔹 3 - View Multiple Files

```bash
cat /etc/passwd /etc/hosts
```

Displays the content of **two files** sequentially.

---

## 🔹 4 - Tail (Last Lines)

```bash
tail -n 10 /etc/passwd
```

Displays the **last 10 lines** of a file.  
- `-n` specifies the number of lines.

---

## 🔹 5 - Head (First Lines)

```bash
head -n 10 /etc/passwd
```

Displays the **first 10 lines** of a file.

---

## 🔹 6 - Extract a Specific Line

```bash
head -n 3 iacta | tail -n 1
```

Displays the **3rd line** only.

---

## 🔹 7 - Create File with Special Name

```bash
echo "Best School" > \\\*\\\\"'\"Best School\"\\'"\\\\\*\$\\\?\\\*\\\*\\\*\\\*\\*\:\)
```

- Uses `\` to escape characters that would otherwise execute commands.  
- Creates a file with a complex, specific name.

---

## 🔹 8 - Redirect Output to File

```bash
ls -la > ls_cwd_content
```

- `>` writes the **output of a command** to a file, replacing its content.

---

## 🔹 9 - Append Output to File

```bash
tail -n 1 iacta >> iacta
```

- `>>` appends the output to the file if it already exists.

---

## 🔹 10 - Find Files

```bash
find . -type f -name "*.js"
```

- Finds all `.js` files (`-name "*.js"`) that are **files** (`-type f`) in the current directory (`.`).

---

## 🔹 11 - Count Directories

```bash
find -mindepth 1 -type d | wc -l
```

- Counts the number of directories (`-type d`) at **depth 1** (`-mindepth 1`)  
- `wc -l` counts lines

---

## 🔹 12 - Newest Files

```bash
ls -1t | head -n 10
```

- `-1t` → list **one file per line**, sorted by modification time  
- `head -n 10` → display the 10 newest files

---

## 🔹 13 - Unique Lines

```bash
sort | uniq -u
```

- `sort` → sorts input  
- `uniq -u` → filters **lines that appear only once**

---

## 🔹 14 - Search for a String

```bash
grep "root" /etc/passwd
```

Displays lines containing `"root"`.

---

## 🔹 15 - Count Lines Matching Pattern

```bash
grep bin /etc/passwd | wc -l
```

- Counts lines that contain `"bin"`

---

## 🔹 16 - Lines After a Match

```bash
grep -A 3 root /etc/passwd
```

- Displays lines containing `"root"` **and the 3 lines after** (`-A 3`)

---

## 🔹 17 - Exclude Lines Matching Pattern

```bash
grep -v bin /etc/passwd
```

- Shows lines **that do NOT contain** `"bin"` (`-v`)

---

## 🔹 18 - Lines Starting with a Letter

```bash
grep "^[A-Za-z]" /etc/ssh/sshd_config
```

- `^` → matches the **start of the line**  
- `[A-Za-z]` → any letter

---

## 🔹 19 - Translate Characters

```bash
tr 'AZ' 'ce'
```

- `tr` replaces characters  
- `' '` prevents shell from interpreting special characters

---

## 🔹 20 - Delete Characters

```bash
tr -d 'cC'
```

Deletes all occurrences of `c` and `C`.

---

## 🔹 21 - Reverse Input

```bash
rev
```

Reverses the input line by line.

---

## 🔹 22 - Cut & Sort Users

```bash
cut -d: -f1,6 /etc/passwd | sort
```

- `cut -d:` → splits fields using `:` as delimiter  
- `-f1,6` → extracts **field 1 (username)** and **field 6 (home directory)**  
- `sort` → sorts output by username

---

### 22 Explanation

- `/etc/passwd` fields: `username:password:UID:GID:info:home:shell`  
- `cut -d: -f1,6` → extracts **username** and **home directory**  
- `sort` → sorts users alphabetically

---

## Key Concepts Learned

- Printing and escaping text (`echo`)  
- Viewing file content (`cat`, `head`, `tail`)  
- Redirection (`>`, `>>`)  
- Filtering and searching (`grep`, `sort`, `uniq`, `wc`)  
- Text transformations (`tr`, `rev`)  
- Field extraction (`cut`)  
- File and directory operations (`find`)  

---

## Author

Redirection & Filters project from **Holberton School**.
