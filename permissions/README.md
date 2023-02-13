Description of all scripts used in this project

Task 0 My name is Betty
A script that switches the current user to the user betty.
#!/bin/bash
su betty hello

Task 1 Who am I
A script that prints the effective username of the current user.
#!/bin/bash
whoami

Task 2 Groups
A script that prints all the groups the current user is part of.
#!/bin/bash
groups

Task 3 New owner
A script that changes the owner of the file hello to the user betty.
#!/bin/bash
chown betty hello

Task 4 Empty!
A script that creates an empty file called hello.
#!/bin/bash
touch hello

Task 5 Execute
A script that adds execute permission to the owner of the file hello
#!/bin/bash
chmod 744 hello

Task 6 Multiple permissions
A script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.
#!/bin/bash
chmod 754 hello

Task 7 Everybody 
A script that adds execution permission to the owner, the group owner and the other users, to the file hello
#!/bin/bash
chmod a+x hello

Task 8 James Bond
A script that sets the permission to the file hello as follows:
Owner: no permission at all
Group: no permission at all
Other users: all the permissions.
#!/bin/bash
chmod 007 hello

Task 9 John Doe
A script that sets the mode of the file hello to this -rwxr-x-wx
#!/bin/bash
chmod 753 hello

Task 10 Look in the mirror 
A script that sets the mode of the file hello the same as olleh’s mode
#!/bin/bash
chmod --reference=olleh hello

Task 11 Directories
A script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed.
#!/bin/bash
chmod -R 755 ./*/

Task 12 More directories
A script that creates a directory called my_dir with permissions 751 in the working directory
#!/bin/bash
mkdir -m751 my_dir

Task 13 Change group
A script that changes the group owner to school for the file hello
#!/bin/bash
chgrp school hello

Task 14 Owner and group
A script that changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.
#!/bin/bash
sudo chown -R vincent:staff .

Task 15 Symbolic links
A script that changes the owner and the group owner of _hello to vincent and staff respectively
#!/bin/bash
sudo chown -h vincent:staff _hello

Task 16 If only
A script that changes the owner of the file hello to vincent only if it is owned by the user guillaume
#!/bin/bash
chown --from=guillaume vincent hello
