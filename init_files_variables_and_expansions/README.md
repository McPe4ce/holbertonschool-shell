# Shell Variables & Commands Project

In this project, we explored how to:

- Display variables  
- Create local variables  
- Create global variables  

This README serves as a guide explaining what each command does.

---

## 0 - Alias

```bash
alias ls='rm -f *'
```

Creates an alias that allows you to launch a command by entering a pre-set string.  
Here, typing `ls` would execute `rm -f *`.

---

## 1 - Display a Variable

```bash
echo "hello $USER"
```

Displays a message containing a variable.  
`$USER` is an environment variable defined using `$`.

---

## 2 - Add Directory to PATH

```bash
export PATH="$PATH:/action"
```

Adds `/action` as the last directory the shell searches when looking for programs.

---

## 3 - Count Directories in PATH

```bash
echo $PATH | tr ':' '\n' | grep / | wc -l
```

Explanation:

- `$PATH` contains multiple directories separated by `:`
- `tr ':' '\n'` replaces `:` with a new line
- `grep /` keeps directory-like entries
- `wc -l` counts the number of lines (directories)

---

## 4 - View Environment Variables

```bash
printenv | less
```

- `printenv` prints all environment variables  
- `less` shows the output one screen at a time  

---

## 5 - List Variables and Functions

```bash
set
```

Lists:

- Local variables  
- Environment variables  
- Functions  

---

## 6 - Create a Local Variable

```bash
BEST="School"
```

Creates a local variable called `BEST` with the value `"School"`.

---

## 7 - Create a Global Variable

```bash
export BEST="School"
```

Creates a global (environment) variable.

- Local variables exist only in the current shell.
- Global variables are accessible to child processes.

---

## 8 - Arithmetic Expansion

```bash
echo $((128 + TRUEKNOWLEDGE))
```

Displays the sum of `128` and the variable `TRUEKNOWLEDGE`.

- `$(( ))` → arithmetic expansion  
- `$()` → command substitution  

---

## 9 - Division Between Two Variables

```bash
echo $((POWER / DIVIDE))
```

Displays the result of dividing `POWER` by `DIVIDE`.

---

## 10 - Exponentiation

```bash
echo $((BREATH ** LOVE))
```

Raises `BREATH` to the power of `LOVE`.

---

## 11 - Binary to Decimal Conversion

```bash
echo $((2#BINARY))
```

Converts a number from base 2 (binary) to base 10 (decimal).

---

## 12 - Generate Two-Letter Combinations

```bash
echo {a..z}{a..z} | tr ' ' '\n' | grep -v oo
```

Explanation:

- `{a..z}{a..z}` generates all two-letter combinations from `aa` to `zz`
- `tr ' ' '\n'` replaces spaces with new lines
- `grep -v oo` removes lines containing `oo`

---

## 13 - Floating-Point Formatting

```bash
printf "%.2f\n" "$NUM"
```

Displays a formatted floating-point number:

- `%` → insert a value  
- `.2` → two digits after the decimal point  
- `f` → floating-point number  
- `\n` → new line  

---

## 14 - Decimal to Hexadecimal Conversion

```bash
printf "%x\n" "$DECIMAL"
```

- `%x` converts a decimal number to hexadecimal  
- `\n` prints a new line  

---

## About `printf`

`printf` prints formatted output and works like the C programming `printf`.

Unlike `echo`, it:

- Understands format specifiers  
- Controls decimal precision  
- Controls spacing  
- Handles newlines properly  
