Shell Variables & Commands Project

In this project, we explored how to:

Display variables

Create local variables

Create global variables

This README serves as a guide explaining what each command does.

Tasks & Explanations
0 - alias ls='rm -f *'

Creates an alias that allows you to launch a command by entering a pre-set string.
Here, typing ls would execute rm -f *.

1 - echo "hello $USER"

Displays a message containing a variable.
$USER is an environment variable defined by $.

2 - export PATH="$PATH:/action"

Adds a directory to an existing variable.
Here, /action is added as the last directory the shell searches when looking for programs.

3 - Count directories in PATH
echo $PATH | tr : '\n' | grep / | wc -l


Explanation:

$PATH contains multiple directories separated by :

tr : '\n' replaces : with a newline

grep / keeps lines that look like directory paths

wc -l counts the number of lines (directories)

4 - printenv | less

printenv prints all environment variables

less displays the output one screen at a time

5 - set

Lists:

Local variables

Environment variables

Functions

6 - BEST="School"

Creates a local variable called BEST with the value "School".

7 - export BEST="School"

Creates a global (environment) variable.

Local variables are accessible only in the current shell or function.

Global (exported) variables are accessible to child processes.

8 - Arithmetic Expansion
echo $((128 + TRUEKNOWLEDGE))


Displays the sum of 128 and the variable TRUEKNOWLEDGE.

$(( )) → arithmetic expansion

$() → command substitution

9 - Division Between Two Variables
echo $((POWER / DIVIDE))


Displays the result of dividing POWER by DIVIDE.

10 - Exponentiation
echo $((BREATH ** LOVE))


Raises BREATH to the power of LOVE.

11 - Binary to Decimal Conversion
echo $((2#BINARY))


Converts a number from base 2 (binary) to base 10 (decimal).

12 - Generate Two-Letter Combinations
echo {a..z}{a..z} | tr ' ' '\n' | grep -v oo


Explanation:

{a..z}{a..z} generates all two-letter combinations from aa to zz

tr ' ' '\n' replaces spaces with newlines

grep -v oo removes lines containing oo

13 - Floating-Point Formatting
printf "%.2f\n" "$NUM"


Displays a formatted floating-point number:

% → insert a value

.2 → two digits after the decimal point

f → floating-point number

\n → new line

14 - Decimal to Hexadecimal Conversion
printf "%x\n" "$DECIMAL"


%x converts a decimal number to hexadecimal

\n prints a new line

Little PS: About printf

printf prints formatted output and works like the C programming printf.

Unlike echo, it:

Understands format specifiers

Controls decimal precision

Controls spacing

Handles newlines properly