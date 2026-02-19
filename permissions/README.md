This README explains the permission project 

0- su betty                 This command changes the user
1- whoami                   Prints the current username 
2- groups                   Prints the groups the user is in
3- chown betty hello        Changes the owner of a file
4- touch hello              Creates an empty file
5- chmod u+x hello          Adds execute (x) permissions to user (u)
6- chmod u+x,g+x,o+r hello  Adds execute permissions to user and group (g) and read (r) to others (o)
7- chmod ugo+x hello        Adds execute permission to all
8- chmod 007 hello          Sets no perms to user and group and gives all to other users
9- chmod 753 hello          Sets perms for a file

10- chmod --reference hello olleh           Mirrors permissions 
11- chmod a+x */                            Gives all permissions to everyone to files not directories
12- mkdir -m 751 my_dir                     Creates a directory with a permission MODE (-m) 
13- chgrp school hello                      Changes group owner of a file
14- chown vincent:staff *                   Changes user to vincent and group to staff for all files
15- chown -h vincent:staff _hello           Changes the permissions for the symbolic link not the original file using (-h)
16- chown --from=guillaume vincent hello    Changes owner of a file only if it is owned by someone specifically  
