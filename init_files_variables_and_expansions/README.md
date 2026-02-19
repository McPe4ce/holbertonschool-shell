This README presents all the commands used in this project

0- alias ls= rm -f*         Creating this allows to launch a command by entering a pre-set string
1- echo "hello $USER"       Displays a message with a variable defined by $ 
2- export "$PATH:/action"   Adds a directory to a variable, and here it is the last directory the shell looks when looking for it

3- echo $PATH | tr : $'\n' | grep / | wc -l         Counts the number of directories in PATH with $PATH being an absolute path with many dir, tr translates with : to cut and change to new line, \n counts the lines, grep / finds the pattern of directories and wc counts them.

4- printenv | less          Prints all the variables in the environment and less shows one file at a time 
5- set                      Lists all the local variables, environment and functions.
6- 
