# Networking with Linux
1. Created virtual machines connection according to figure 1:
VM1 VM2
HOST
INTERNET
2. VM2 has one interface (internal), VM1 has 2 interfaces (NAT and internal). Configure all network
interfaces in order to make VM2 has an access to the Internet (iptables, forward, masquerade).
![6](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/351bf255f6e987436fc246cfa8783a2c7da1559d/m6/task%206.1/img/6.png)
![6.1](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/351bf255f6e987436fc246cfa8783a2c7da1559d/m6/task%206.1/img/6.1.png)
![6.2](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/351bf255f6e987436fc246cfa8783a2c7da1559d/m6/task%206.1/img/6.2.png)
![MASQ](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/351bf255f6e987436fc246cfa8783a2c7da1559d/m6/task%206.1/img/MASQ.png)
3. Check the access to the Internet, (just ping, for example, 8.8.8.8).
![MASQ](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/351bf255f6e987436fc246cfa8783a2c7da1559d/m6/task%206.1/img/MASQ.png)
4. Determine, which resource has an IP address 8.8.8.8.
![google](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/351bf255f6e987436fc246cfa8783a2c7da1559d/m6/task%206.1/img/google.png)
5. Determine, which IP address belongs to resource epam.com.
![epam](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/351bf255f6e987436fc246cfa8783a2c7da1559d/m6/task%206.1/img/epam.png)
6. Determine the default gateway for your HOST and display routing table.
![routing](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/351bf255f6e987436fc246cfa8783a2c7da1559d/m6/task%206.1/img/routing.png)
7. Trace the route to google.com
![trace](https://github.com/AlexLastArch/DevOps_online_Lviv_2021Q2/blob/351bf255f6e987436fc246cfa8783a2c7da1559d/m6/task%206.1/img/trace.png)
