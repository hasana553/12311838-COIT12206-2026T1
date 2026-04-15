Introduction:
This assignment will help you understand how packet routing works within a computer network by implementing both static (manually created) and dynamic (automatically generated) routing methods. Your first task is to create a small computer network containing four Linux-based hosts and one Linux-based router using a GNS3 emulator to observe the way in which packets are forwarded through the entire network and how routing tables are created for each of the subnets.

Each device in the subnetwork has a static (fixed) IP address assigned, and IP Forwarding must be set on the router to allow packets to pass from one network to another.

Your second task will examine using the open shortest path first (OSPF) dynamic routing protocol to automatically update routing tables whenever there is a change in the way packets can be routed from one network to another. The analysis tools (routing commands and traceroute) will help to verify how packets are routed between different devices on the network and also provide insight into how the routing protocols adapt to link failures.
<img width="940" height="505" alt="image" src="https://github.com/user-attachments/assets/f0c26184-cc00-4ab1-8132-7708559f25bb" />
<img width="778" height="458" alt="image" src="https://github.com/user-attachments/assets/368a37ac-cbeb-4461-9e7a-957d4a593421" />
<img width="940" height="710" alt="image" src="https://github.com/user-attachments/assets/59884cc6-0c7c-4a90-84f7-2d0b7c2d7968" />
<img width="940" height="325" alt="image" src="https://github.com/user-attachments/assets/fdf43dcd-f4e1-4135-ad04-997f5ead3f3d" />
source	Deatination	Next route	Interface
10.10.1.101	10.10.1.0/24	Direct	Eth0
	any	10.10.1.101	Eth0
		<img width="940" height="354" alt="image" src="https://github.com/user-attachments/assets/cb66afd8-7f37-4729-875c-5b2279193dc0" />
	<img width="940" height="732" alt="image" src="https://github.com/user-attachments/assets/4318cf27-4f99-473d-bb5d-399c60e1bda9" />
<img width="940" height="643" alt="image" src="https://github.com/user-attachments/assets/3bfdbc64-676b-4c6e-9799-b4c797851e2c" />
<img width="939" height="889" alt="image" src="https://github.com/user-attachments/assets/20c62992-fd2e-4730-b5b9-f1af0a94baed" />
<img width="939" height="889" alt="image" src="https://github.com/user-attachments/assets/54937d46-3472-4b93-8c0a-08d2c5d16e6e" />
Task 2
Frr1:
<img width="940" height="684" alt="image" src="https://github.com/user-attachments/assets/2e7b768f-f932-4b4c-868b-455235523173" />
<img width="940" height="410" alt="image" src="https://github.com/user-attachments/assets/87281fe7-8ba4-42c3-8bba-db325ca52d11" />

Conclusion
The two tasks from this assessment have demonstrated the basic principles of Routing in a networking context. Task 1 proved the theory behind manually managing routing tables, as well as enabling IP forwarding between two different subnets. It also provided examples of where to configure the IP Address(es) as well as the gateway in this type of scenario.Task 2 highlighted the many advantages of using dynamic routing protocols such as OSPF by demonstrating how routers share information with one another to automatically update each other’s routing tables. Furthermore, when a link is disconnected in a network using OSPF to perform dynamic routing there will be an alternative route that will be found quickly to ensure there is no disruption to the flow of data between two nodes (routers).

Additionally, it is clear from these two assessments why dynamic routing protocols exist and are more efficient and reliable in complex or changing environments in comparison to static routing protocols.

Reflection:
Experiencing the network configuration process and how routing works in practical applications helped to increase my knowledge on network routing and configuration. The first few steps helped provide an overview of the process. The configuration of IP addresses and forwarding required accuracy and attention to detail because a small mistake could result in no communication occurring.

Using OSPF showed me how routers dynamically learn of new routes and update their routing table with this information. In particular, the ability of the network to automatically reconfigure itself when you disconnected a link was a valuable lesson on the importance of fault tolerance in networks.

The project has enhanced my skills in network configuration, troubleshooting issues within the network, and analysing routing behaviours. Additionally, I have developed an understanding of the differences between static and dynamic routing protocols, and why dynamic routing protocols such as OSPF are widely utilised in today’s networks.





