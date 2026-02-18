In this README file, there are all the commands that can be used by the shell, in the Holberton School project: BASICS. 

0- pwd              Prints the current working directory
1- ls               Displays the content of the current working directory
2- cd               Changes the working directory to the home of the user
3- ls -l            Displays the files of the current working directory in long format
4- ls -la           Displays all the files, including the hidden files
5- ls -lan          Displays all the files, with users and groups ID in long format

mkdir /tmp/my_first_directory               Creates a new directory in the /tmp directory
mv betty /tmp/my_first_directory            Moves the file betty from /tmp/ to /tmp/my_first_directory
rm /tmp/my_first_directory/betty            Deletes the betty file
rmdir /tmp/my_first_directory               Deletes the directory my_first_directory
cd..                                        Changes the working directory to the previous one
ls . .. -la /boot                           Lists all files (ls), even hidden ones (-la) in the current directory (.) and the parent directory (..) as well as in /boot directory

file /tmp/iamafile                          Prints the type of a file
ln -s /bin/ls __ls__                        Creates a link (ln) that is SYMBOLIC (-s) in the current working directory
mv -u *.html ..                             Moves files (mv) in HTML (*.html) that did not exist and UPDATE (-u) in the parent directory (..)
mv [A-Z]* /tmp/u                            Moves files that start with an uppercase ([A-Z]*) in another directory
rm -f *~                                    Deletes all files FORCEFULLY (-f) that end with ~ in the current directory
mkdir -p welcome/to/school                  Creates a directory (mkdir) even a parent one (-p) that are /welcome /welcome/to welcome/to/school
