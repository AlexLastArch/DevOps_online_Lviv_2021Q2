## TASK5.3
##### Part1

1. How many states could has a process in Linux?
6 states: Running, Sleeping, Uninterruptable, Sleep, Stopped, Zombie

2. Examine the pstree command. Make output (highlight) the chain (ancestors) of the current 
process.
![1]()
3. What is a proc file system?
The proc file system contains a hierarchy of special files that represent the current state of the kernel. It is named after its original purpose, which is an interface to the structures within running processes to support debugging tools.

4. Print information about the processor (its type, supported technologies, etc.).
![2]()

5. Use the ps command to get information about the process. The information should be as 
follows: the owner of the process, the arguments with which the process was launched for 
execution, the group owner of this process, etc.
ps -u 
ps -aux

6. How to define kernel processes and user processes?
UID 

7. Print the list of processes to the terminal. Briefly describe the statuses of the processes. 
What condition are they in, or can they be arriving in?
ps -x

8. Display only the processes of a specific user.
ps -u [username]

9. What utilities can be used to analyze existing running tasks (by analyzing the help for the ps 
command)?
htop
top
10. What information does top command display?
The Linux top command is an interactive utility that displays a character-based screen of all processes running on the current system. The screen updates itself every few seconds, and you can sort the screen contents by characteristics like CPU Usage or Memory Use.

12. Display the processes of the specific user using the top command.
Shift+n - sort by PID

12. What interactive commands can be used to control the top command? Give a couple of 
examples.
<Space> or <Enter> refresh
<?> or <help> help
<A> Alternative mode
<B> Bold
<k> kill task
<z> change color

13. Sort the contents of the processes window using various parameters (for example, the 
amount of processor time taken up, etc.)
Shift + P

14. Concept of priority, what commands are used to set priority?
Nice and renice

15. Can I change the priority of a process using the top command? If so, how?
r - renice

16. Examine the kill command. How to send with the kill command process control signal? Give an example of commonly used signals.
kill -9

17. Commands jobs, fg, bg, nohup. What are they for? Use the sleep, yes command to 
demonstrate the process control mechanism with fg, bg.
jobs -show stoped proces
fg -move a background job into the foreground
bg -resume the sleep job

#### Part2

1. Check the implementability of the most frequently used OPENSSH commands in the MS 
Windows operating system. (Description of the expected result of the commands + 
screenshots: command – result should be presented)
ssh
ssh -V
ssh -keygen
![3]()

2. Implement basic SSH settings to increase the security of the client-server connection (at least 
ssh -i -private access
-p – Use this if your SSH server is listening on a different port (other than 22). Example: ssh -p 4444 root@203.0.113.1
-C – Compress traffic between client and server. Only useful on very slow connections
-v – Verbose mode, outputs a lot more about what is going on. Can help you debug connection issues.

3. List the options for choosing keys for encryption in SSH. Implement 3 of them.
ssh-keygen -t rsa -b 4096
ssh-keygen -t ed25519  -o -a 250 -C “Andrew to WebServer Edwards Twisted Curve”
ssh-keygen -t rsa -b 4096 -o -a 250

4. Implement port forwarding for the SSH client from the host machine to the guest Linux 
virtual machine behind NAT.
![4]()
![5]()
![6]()
![7]()
![8]()
![9]()
5*. Intercept (capture) traffic (tcpdump, wireshark) while authorizing the remote client on the 
server using ssh, telnet, rlogin. Analyze the result
![10]()
tcpdump is a command-line utility that you can use to capture and inspect network traffic going to and from your system. It is the most commonly used tool among network administrators for troubleshooting network issues and security testing.

