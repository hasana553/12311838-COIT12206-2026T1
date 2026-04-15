Week 5:
This lab focuses on configuring VLANs (virtual local area networks) with a managed switch in a lab environment. VLAN's are one of the main concepts in computer networking, allowing network administrators to separate a physical network into multiple smaller networks logically. This has numerous benefits, including increasing security, reducing broadcast traffic, and improving overall network performance.

Using GNS3 to create the network topology out of linux hosts with an open vSwitch, we will begin by configuring a default subnet with each host creating basic connectivity. Next we will configure VLAN's to separate hosts from each other onto separate broadcast domains. Finally, we will introduce a router to allow use of a trunk and sub-interfaces for inter-VLAN routing.
<img width="940" height="592" alt="image" src="https://github.com/user-attachments/assets/e9eab618-8a8d-4ddb-8612-eb1bf6321b37" />
Host 1:
<img width="940" height="706" alt="image" src="https://github.com/user-attachments/assets/05071aeb-7589-44bf-906f-0838d5225bd4" />
<img width="940" height="705" alt="image" src="https://github.com/user-attachments/assets/bb3b7f96-133a-41b1-bce7-bfe133443c63" />
<img width="940" height="689" alt="image" src="https://github.com/user-attachments/assets/cfd044fa-ca13-4387-a904-087d013508e9" />
Pinging host2 from host 1:
<img width="940" height="620" alt="image" src="https://github.com/user-attachments/assets/12e9fb5e-407b-48af-971f-f17cb9ea2c42" />

Pinging host3 from host1:
<img width="940" height="746" alt="image" src="https://github.com/user-attachments/assets/8b196132-9161-4791-82b6-ba4fdb176803" />
<img width="940" height="666" alt="image" src="https://github.com/user-attachments/assets/b71c4d1a-1947-4648-aeaf-aa1ea0103290" />
Task 2:
<img width="940" height="754" alt="image" src="https://github.com/user-attachments/assets/881d5cfa-e212-4fb4-92d3-a081eb51f90f" />
<img width="940" height="624" alt="image" src="https://github.com/user-attachments/assets/71a21e5b-86d6-45da-a713-f917498566e2" />

Ovs-vsctl set port eth0 trunks=[]
<img width="716" height="216" alt="image" src="https://github.com/user-attachments/assets/df63fc90-5204-4959-8c59-de9a28eb0213" />

Conclusion:
.This experiment verified that it is possible to configure and manage virtual networks "creating" VLANs by assigning switch ports to different VLAN IDs and creating two separate logical groups of hosts on the same physical network segment, as the hosts would not be able to communicate with each other across the two VLANs using VLANs to isolate traffic from each other effectively.

In addition, by configuring a router to create VLAN sub-interfaces and configuring the switch port used for the trunk link between the router and switch, the hosts in the two VLANs could communicate with each other; therefore, showing that routing is essential to connect segmented networks. The project demonstrated how to configure a VLAN, create a trunk link, and route between VLANs


Reflection:
	I gained practical experience in creating VLANs and seeing how the network is divided into smaller parts.  One of the things I learned the most about was the importance of configuring VLANs correctly to your switch ports as well as verifying that you've configured everything correctly (i.e., using commands such as ovs-vsctl show).  The other concept I also had a difficult time grasping at first was the difference between access ports and trunk ports but by configuring the access and trunk ports step-by-step, it became easier for me to understand the concept behind each.

Another critical concept is the requirement for routing in order to allow computers on separate VLANs to communicate with one another.  Configuring sub-interfaces on the router shows how you can have multiple VLANs on one physical port of the physical router.  I have also developed problem-solving skills during the lab to troubleshoot connectivity issues when verifying IP address schemes, VLAN assignments, and ARP tables.

This lab has provided me with a much better understanding of purpose of VLANs in real-world networking and provided me with a higher amount of confidence in my abilities to use network simulation applications and command-line type configuration, which will be beneficial to my future pursuits within the Networks field as well as in the IT area



