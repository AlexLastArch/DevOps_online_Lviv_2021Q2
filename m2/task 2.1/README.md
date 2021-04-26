Module 2 Virtualization and Cloud Basic
# TASK 2.1
## PART 1. HYPERVISORS
##### __1. What are the most popular hypervisors for infrastructure virtualization?__
* VMware vSphere Hypervisor
* Microsoft Hyper-V
* Citrix XenServer
* Oracle VirtualBox
* KVM (Kernel-based Virtual Machine)

##### __2. Briefly describe the main differences of the most popular hypervisors.__
* __Oracle VirtualBox__ has free accsess
* __WMWare__ One of the largest developers of software solutions in the field of virtualization
* __Hyper-V__ are greatly enhanced with the help of Microsoft System Center components.
---
### PART 2. WORK WITH VIRTUALBOX
__1.1__ Downloaded the latest stable version of VirtualBox for Linux Ubuntu and installed it.
1.2 Downloaded the latest stable version Ubuntu Server.
1.3 Created VM1 and set machine name as "Ubuntu"_"Pokhodoshchuk"
1.4 Got acquainted with the possibilities of VM1 control - start, stop, reboot, save state, use Host key and keyboard shortcuts, mouse capture, etc.
1.5 Cloned an existing VM1 by creating a VM2.
1.6 Create a group of two VM: VM1, VM2 and learned the functions related to groups.
1.7 For VM1, changed its state, took several different snapshots, forming a branched tree of snapshots.
![Snapshots](https://user-images.githubusercontent.com/66686269/113589445-04ef6700-963a-11eb-893a-a735a6eaa6a7.png)

1.8 Exported VM1. Saved the *.ova file to disk. Import VM from Ubuntu Server Pokhodoshchuk.ova file .
___

## 2. Configuration of virtual machines


2.1 Explored VM configuration options (general settings, system settings, display, storage, audio, network, etc.).
2.2 Configured the USB to connect the USB ports of the host machine to the VM.
![Vbox](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/issues/2#issue-850429983)
2.3 Configured a shared folder to exchange data between the virtual machine and
the host.
2.4 Configured different network modes for VM1, VM2. Check the connection
between VM1, VM2, Host, Internet for different network modes. Used the ping
command to do this. Made a table of possible connections.


## 3. Work with CLI through VBoxManage.


3.1 Ran the cmd.exe command line.
3.2 Examined the purpose and execute the basic commands of VBoxManage list,
showvminfo, createvm, startvm, modifyvm, clonevm, snapshot, controlvm.

# PART 3. WORK WITH VAGRANT

1. Downloaded the required version of Vagrant for Windows
2. Ran the powershell. Create a folder "oleksandr".
3. Initialized the environment

4. Ran vagrant up and watch for messages during VM boot and startup.
For connection to the VM used the program PuTTY
6. Record the date and time by executing the date command
![Vagrand](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/issues/3#issue-850430340)
7. Stop and delete the created VM.
8. Create my own Vagrant box 
![Vagrand2](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/issues/4#issue-850430623)
