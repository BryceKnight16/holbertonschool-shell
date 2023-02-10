What each sciprt does
Task 0    a script that prints the absolute path name of the current working directory 
#!/bin/bash
 pwd
Task 1 a script that displays a list whats in the current directory 
#!/bin/bash 
ls
Task 2 a script that changes the working directory to the user’s home directory.
 #!/bin/bash 
cd ~
Task 3  a script that displays current directory contents in a long format 
#!/bin/bash 
ls -l
Task 4  a script that displays current directory contents, including hidden files in long format #!/bin/bash 
ls -l
Task 5  a script that lists all files in long format sorted numerically 
#!/bin/bash 
ls -lan
Task 6  a script that makes a new directory 
#!/bin/bash 
mkdir /tmp/my_first_directory
Task 7  a script that moves a file from one dir to another 
#!/bin/bash 
mv /tmp/betty tmp/my_first_directory/betty
Task 8  a script that removes a file 
#!/bin/bash 
rm /tmp/my_first_directory/betty
Task 9 a script that removes a directory 
#!/bin/bash rmdir /tmp/my_first_directory
Task 10  a script that toggles between last two directories
 #!/bin/bash 
cd -
Task 11  a script that lists all files in the current, parent and boot directories 
#!/bin/bash 
ls -la . .. /boot
Task 12  a script that prints the file type 
#!/bin/bash 
file /tmp/iamafile
Task 13  a script that makes a symbolic link that points to a file 
#!/bin/bash 
ln -s /bin/ls __ls__
Task 14  a script that copies all .html files in the current directory to the parent directory #!/bin/bash 
cp -u *.html ..
Task 15  a script that moves all files starting with a capital letter to another directory 
#!/bin/bash 
mv [[:uppper:]]* /tmp/u
Task 16  a script that removes all emacs files 
#!/bin/bash 
rm *~
Task 17  a script that makes create directories inside directories
#!/bin/bash 
mkdir -p welcome/to/school
