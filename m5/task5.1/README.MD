## Task1.Part1

1) Loged in to the system as root. 
2) Used the passwd command to change the password. Examine the basic 
parameters of the command. 
It change file /etc/passwd and /etc/shadow

3) Determine the users registered in the system, as well as what commands they execute. What additional information can be gleaned from the command execution?
__who -shows who is currently logged into the system__
__w - shows who is currently in the system and what he is doing__
__whoami - prints out the users UID__
__id - prints extended user informstion (group, uid, gid)__
![1](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/1.png)
4) Change personal information about yourself.
__chnf__
![2](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/2.png)
5) Become familiar with the Linux help system and the man and info commands. 
__man chnf__
![3](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/3.png)

6) Explore the more and less commands using the help system. View the contents of files .bash* using commands.
![4](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/4.png)
![5](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/5.png)
![6](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/6.png)
![7](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/7.png)


### Task1.Part2
1) Examine the tree command. Master the technique of applying a template, for example, display all files that contain a character c, or files that contain a specific sequence of characters. List subdirectories of the root directory up to and including the second nesting level.
![8](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/8.png)
![9](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/9.png)
![10](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/10.png)
2) What command can be used to determine the type of file (for example, text or 
binary)? Give an example.
3) Master the skills of navigating the file system using relative and absolute paths. 
How can you go back to your home directory from anywhere in the filesystem?
__cd /home__
__cd__
4) Become familiar with the various options for the ls command. Give examples 
of listing directories using different keys. Explain the information displayed on 
the terminal using the -l and -a switches.

ls -R will list all the files in the sub-directories as well
ls -a will show the hidden files
ls -al will list the files and directories with detailed information like the permissions, size, owner, etc.
![11](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/11.png)
5) Perform the following sequence of operations:
- create a subdirectory in the home directory;
- in this subdirectory create a file containing information about directories located in the root directory (using I/O redirection operations);
- view the created file;
- copy the created file to your home directory using relative and absolute 
addressing.
- delete the previously created subdirectory with the file requesting removal;
- delete the file copied to the home directory.
![12](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/12.png)
![13](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/13.png)

 6.Perform the following sequence of operations:
 - create a subdirectory test in the home directory;- copy the .bash_history file to this directory while changing its name to labwork2;
![14](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/14.png)
- create a hard and soft link to the labwork2 file in the test subdirectory;
- how to define soft and hard link, what do these concepts;
If move the executable, it may not work as it needs to access some of the code and it won't find the path to these files from the /usr/bin directory. This is where you can create a link to this executable file in the /usr/bin directory.
- change the data by opening a symbolic link. What changes will happen and 
why
- rename the hard link file to hard_lnk_labwork2;
- rename the soft link file to symb_lnk_labwork2 file;
![15](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/15.png)
- then delete the labwork2. What changes have occurred and why?
Soft link changed color A symbolic or soft link is an actual link to the original file, whereas a hard link is a mirror copy of the original file. If you delete the original file, the soft link has no value, because it points to a non-existent file. But in the case of hard link, it is entirely opposite. Even if you delete the original file, the hard link will still has the data of the original file. Because hard link acts as a mirror copy of the original file.
![16](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/16.png)
7) Using the locate utility, find all files that contain the squid and traceroute sequence.
![17](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/17.png)
8) Determine which partitions are mounted in the system, as well as the types of these partitions.
![18](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/18.png)
9) Count the number of lines containing a given sequence of characters in a given file.
10) Using the find command, find all files in the /etc directory containing the host character sequence.
![19](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/19.png)
11) List all objects in /etc that contain the ss character sequence. 
![20](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/156fdeaf7b324bd3d24e1176aa45efd82b945b12/m5/task5.1/img/20.png)

12) Organize a screen-by-screen print of the contents of the /etc directory. Hint: You must use stream redirection operations.
13) What are the types of devices and how to determine the type of device? Give examples.
14) How to determine the type of file in the system, what types of files are there?
15) * List the first 5 directory files that were recently accessed in the /etc directory
