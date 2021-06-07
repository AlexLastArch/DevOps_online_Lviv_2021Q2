## Task2

1) Analyze the structure of the /etc/passwd and /etc/group file, what fields are present in it, what users exist on the system? Specify several pseudo-users, how to define them?
![1](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/df5acc71e7e2456a0b9a47bcdabaf3743892de3d/m5/task5.2/img/1.png)
![2](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/df5acc71e7e2456a0b9a47bcdabaf3743892de3d/m5/task5.2/img/2.png)
__Root, Pseudo-users, Regular users__
__sshd, bin, daemon, nobody. Their UID between 1-999__
2) What are the uid ranges? What is UID? How to define it?
UID numeric designation for individual user. Usualy not more than 65535.

3) What is GID? How to define it?
GUI group unique identifier. 
$ groups

4) How to determine belonging of user to the specific group?
$ groups sk

5) What are the commands for adding a user to the system? What are the basic parameters required to create a user?
sudo useradd test_user
sudo -d /home/test_user test_user
sudo passwd

6) How do I change the name (account name) of an existing user?
sudo usermod -l

7) What is skell_dir? What is its structure?
skell_dir - кcontains files which must be copied to the new users home dir

8) How to remove a user from the system (including his mailbox)?
userdel [-r] username

9) What commands and keys should be used to lock and unlock a user account?
passwd -l username -block and adding prefix! to password
passwd -u username -unblock user and remove prefix !

10) How to remove a user's password and provide him with a password-free login for subsequent password change?
passwd -d username -cancel the password for the user and allows the user to change it

11) Display the extended format of information about the directory, tell about the information columns displayed on the terminal.
ls -al

12) What access rights exist and for whom (i. e., describe the main roles)? Briefly describe the acronym for access rights.
read (r)-4 
write (w)-2
execute (x)-1
root, first 3 rwx 
groupe next 3 rwx
others last 3 rwx

13) What is the sequence of defining the relationship between the file and the user?
owner defines what other users or group can do with file

14) What commands are used to change the owner of a file (directory), as well as the mode of access to the file? Give examples, demonstrate on the terminal.
chown [username] [filename]
![2]()
15) What is an example of octal representation of access rights? Describe the umask command.
Octal notation is a numerical system for modifying the permissions on Linux, Mac and other Unix like file systems. Each octal permission can be represented by 3 or 4 numbers; where each of these numbers is an "octal", meaning they range from 0-7. Each one of the numbers represents permissions that can be set to either a file or directory. 777, 2775, 700, 552
The umask settings are actually something of an inversion of the permissions they will create. A 0 in a netmask might yield a 7 for the resultant permissions, where a 7 in a netmask would yield a 0. Thus, 777 is the most restrictive umask setting, and 000 is the most permissive.
Create a new file when your umask setting is 777 and you won't even be able to look at it yourself — at least not without first changing its permissions.

16) Give definitions of sticky bits and mechanism of identifier substitution. Give an example of files and directories with these attributes.
Sticky bit is a permission bit which is set on a file or folder, thereby permitting only the owner or root user of the file or folder to modify, rename or delete the concerned directory or file. No other user would be permitted to have these privileges on a file which has a sticky bit. In Unix-like systems, without the sticky bit on, any user can modify, rename or delete the directory or file regardless of the owner of the file or folder
rwxrwxrwt - t is a sticky bit

17) What file attributes should be present in the command script
Sudo?
