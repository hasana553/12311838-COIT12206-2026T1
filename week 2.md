




Introduction:
The objective of this assessment is to provide an understanding of how to create a static IP address
and verify the ability for devices connected to a network to communicate with one another using the 
ping command in a simulated network environment running on Linux servers using GNS3 as the network simulation application.

There are three different techniques to create a static IP address that were tried: configuring the static IP
using the GNS3 configuration screen, configuring the static IP by editing the /etc/network/interfaces file, and
configuring static IP with the ip address add command. Each method presents varying levels of persistence and flexibility
when creating a static IP address for a given device. Additionally, this assessment includes the use of the ping command to
test whether or not two devices are reachable from one another and measure the amount of time it took for a packet sent from 
one device to arrive at another device in a local area network (LAN).

By completing these tasks, students are able to gain hands-on experience in establishing, configuring, and troubleshooting 
a network within a controlled and simulated network environment.
For host 1:
<img width="940" height="534" alt="image" src="https://github.com/user-attachments/assets/fe875e86-007b-40d4-aeae-67ca46f291fd" />
<img width="940" height="530" alt="image" src="https://github.com/user-attachments/assets/a238d275-a908-47bf-b2d1-f1d2ea612275" />
For host 2:
<img width="940" height="530" alt="image" src="https://github.com/user-attachments/assets/7432806b-d1ba-4d3d-a5df-828c9e5696e3" />
<img width="940" height="527" alt="image" src="https://github.com/user-attachments/assets/62ec415f-4a63-41bc-80a3-eb81d7734c2f" />
For host3:
<img width="940" height="507" alt="image" src="https://github.com/user-attachments/assets/9fe65681-e654-46af-b219-235096775e42" />
<img width="940" height="535" alt="image" src="https://github.com/user-attachments/assets/4e3ad256-f8a0-41e6-b7a3-36a0d8e67220" />
<img width="940" height="535" alt="image" src="https://github.com/user-attachments/assets/0ab95001-50f4-47cb-83dd-607687cb5bca" />
For host 4:
<img width="940" height="526" alt="image" src="https://github.com/user-attachments/assets/51fbb689-b238-4916-acb4-287398669225" />
<img width="940" height="530" alt="image" src="https://github.com/user-attachments/assets/f3f4859f-3e45-4408-b3cf-3e8ceef1fdb6" />

Conclusion:
This assessment created a local area network (LAN) that includes four Linux hosts connected via an Ethernet switch. 
The LAN was built and tested successfully. Each host was given a static IP address using one of three different
methods: via the GNS3 interface, by manually editing the /etc/network/interfaces file of each host, or by dynamically
assigning the host IP address(s) using the ip command.

The results indicated that all three methods of IP address assignment were valid; however, there were major differences 
in persistence and immediacy. The GNS3 interface and the /etc/network/interfaces file provided the static and persistent
configurations needed to maintain the IP address configuration after rebooting. In contrast, the ip command provided immediate
assignments but was not persistent between reboots.

The use of the ping command confirmed that the hosts were able to communicate with each other, in addition to demonstrating
how to use the ping command to determine round-trip-time (RTT) from one device to another and measure the success rate of packet
delivery (lost packets) between devices.

In general, this assessment fulfilled that purpose of demonstrating key concepts associated with networking which include IP 
addressing, configuring interfaces, testing connectivity with ping commands and others.


Reflection:
The experience gained through this assignment allowed me to develop hands-on experience with configuring and managing network
settings in a Linux environment. One major takeaway from this assignment is how to configure persistent versus temporary IP
addresses. The process of editing the /etc/network/interfaces file involved additional steps to restart the interface; 
however, to the best of my ability to perform this configuration correctly, the edit provided a long-term solution.
In contrast, the ip command is a quick and easy way to set an IP address temporarily but does not provide a long-term solution.
This experience working with ping allowed me to better understand how packets communicate over a network, and how packet loss and
delay affect the performance or connectivity of a network. The interpretation of the ping response, specifically the round trip
time and the percentage of packets lost when using ping, enabled me to develop my troubleshooting skills. 

One challenge I encountered while completing this project was ensuring that IP addresses were assigned properly 
(within the same subnet) to allow for communication between the hosts. It was important to understand the value
of proper planning when designing a network. Ultimately, this task has improved my confidence in performing basic 
network configuration and diagnostics, and I look forward to continuing to build on these foundational skills by 
learning about more advanced networking concepts such as DHCP, routing, and firewall configuration.















