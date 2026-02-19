This README is for redirection and filters, serves as indication for commands used in tasks.

0- echo "Hello, World"              This command is used to print a text.
1- echo "\"(Ôo)'"                   The \ cancels the character that follows it.
2- cat /etc/passwd                  This one displays the content of a file 
3- cat /etc/passwd /etc/hosts       Displays content of 2 files
4- tail -n 10 /etc/passwd           Displays the last n (-n) LINES of the file
5- head -n 10 /etc/passwd           Displays the first n (-n) LINES of the file

6- head -n 3 iacta | tail -n 1      Displays the 3rd line only 
7- echo "Best School" > \\\*\\\\"'\"Best School\"\\'"\\\\\*\$\\\?\\\*\\\*\\\*\\\*\\\*\:\)           Creates this specific file name, using \ to cancel characters that would run commands

8- ls -la > ls_cwd_content          Writes the result of a command in a file using > (Replaces the file with the new one)
9- tail -n 1 iacta >> iacta         Writes the last line of the file using >> (Duplicates the file if it exists already)
10- find . -type f -name "*.js"     Deletes all the .js that are FILES (-type f) in the cwd

11- find -mindepth 1 -type d | wc -l        Counts the number of DIRECTORIES (-type d) in the tree with a depth of 1 (-mindepth) and counts with wc -l
12- ls -1t | head -n 10                     Displays the newest files with head with only one file per line (-1t)
13- sort | uniq -u                          Takes a list of word as inputs (sort) and uniq filters the repeated line and makes them appear only once where (-u)
14- grep "root" /etc/passwd                 Displays the lines containing "root"
15- grep bin /etc/passwd | wc -l            Displays the number of lines that have "bin" 
16- grep -A 3 root /etc/passwd              Displays lines with "root" and the three lines AFTER (-A)
17- grep -v bin /etc/passwd                 Displays all the lines that DONT HAVE (-v) bin
18- grep "^[A-Za-z]" /etc/ssh/sshd_config   Displays the lines in a file that START (^) with a letter 
19- tr 'AZ' 'ce'                            Replaces with tr the letter A to Z and c to e, in bash ' ' prevent the shell from interpreting special characters inside them
20- tr -d 'cC'                              DELETES (-d) all defined letters
21- rev                                     Reverse the input
22- cut -d: -f1,6 /etc/passwd | sort        Displays all users and their home directories, sorted by users

22 explanation : 
cut extracts fields from each line of a file
-d: DELEMITERS to :
/etc/passwd uses : in the 7 columns that are username:password:UID:GID:info:home:shell
-f1,6 Extracts field 1 and 6 that are username and home