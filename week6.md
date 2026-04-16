Introduction:

This project contains two important networking elements: 1) mapping an IP address to a hardware-based MAC-address with ARP in local area networks (LAN); and 2) using gateways to route packets across networks.

In order for hosts in the same subnet to communicate with one another, the need arises to construct (and continually update) a dynamic mapping of IP to MAC addresses, by observing the respective ARP tables before and after communication between hosts.

The second half of this project provides insight into routing between subnets by establishing default gateways and configuring them so packets can be routed outside their local subnet through the establishment of routing tables on routers. The routing tables are created based on routing information (the destination IP address) and it can be inferred that the establishment of default gateways and the associated routing tables will enable movement of data packets out-side their local subnets.

Together, these two activities illustrate how devices communicate with one another, within and outside a local network.

Task 1:
<img width="940" height="719" alt="image" src="https://github.com/user-attachments/assets/4374dbe2-1686-4698-aa4e-a80ee6e02444" />
Screenshot of ARP table of host 1:
<img width="940" height="698" alt="image" src="https://github.com/user-attachments/assets/e01562d6-3228-40c6-a3b5-a8f3eaf6b4cb" />
Pinging from host 1 to host 2:
<img width="940" height="491" alt="image" src="https://github.com/user-attachments/assets/22b0d872-b143-4dcc-827f-71255aadaa1f" />
pinging from host 3 to 1:
<img width="940" height="444" alt="image" src="https://github.com/user-attachments/assets/9188d72a-e6c2-4f97-af8c-a9c0763d40a0" />
<img width="940" height="630" alt="image" src="https://github.com/user-attachments/assets/3013211f-3fcc-492b-9504-61fb138a7b38" />

Task 2:
<img width="940" height="794" alt="image" src="https://github.com/user-attachments/assets/cd403e44-3358-4684-8d1e-7cdbc75124a4" />
Configure of host 2:
<img width="940" height="675" alt="image" src="https://github.com/user-attachments/assets/ed2df6a6-93ab-4cde-acaf-50f30cfc75b3" />

Configure of router 1 eth0:
<img width="940" height="685" alt="image" src="https://github.com/user-attachments/assets/094b90a4-2d90-438f-99a6-986ba728ba88" />

Configure of router1 eth1:
<img width="940" height="704" alt="image" src="https://github.com/user-attachments/assets/d7195003-fd79-40f9-9958-78ebe16fe610" />

	Configure of router2 eth0:
<img width="940" height="696" alt="image" src="https://github.com/user-attachments/assets/ddce381b-87f5-49f9-836d-20364484a762" />

Configure of router2 eth1:
<img width="940" height="683" alt="image" src="https://github.com/user-attachments/assets/37f7a352-b542-4a7c-8e99-fa0278a77af6" />

Configure of host 3:
<img width="940" height="733" alt="image" src="https://github.com/user-attachments/assets/f6b77e4a-7d5f-48ff-a838-dc6733db3195" />

Configure of host 4: 
<img width="940" height="687" alt="image" src="https://github.com/user-attachments/assets/0ef1bdb5-049b-405c-b788-3f4e90255792" />

Pinging host 3 from host 1:
<img width="940" height="632" alt="image" src="https://github.com/user-attachments/assets/c703d19d-537d-448c-a35c-d545710e4f25" />

Route show for host 1:
<img width="730" height="169" alt="image" src="https://github.com/user-attachments/assets/c03287c9-77f0-425b-b173-c2150ba1519e" />

Route show for host 2:
<img width="736" height="127" alt="image" src="https://github.com/user-attachments/assets/ef9d1c25-496d-4203-ba52-d324ddfbdfd8" />

Route show for router 1:
<img width="709" height="142" alt="image" src="https://github.com/user-attachments/assets/0b3ae176-62c2-47ea-95cf-b20cc57bf907" />

Route show for router2:
<img width="697" height="139" alt="image" src="https://github.com/user-attachments/assets/d2d50059-d56b-4412-96eb-20dd15eff38e" />

Route show for host 3:
<img width="709" height="131" alt="image" src="https://github.com/user-attachments/assets/3b28c4ee-e0f6-4f69-848b-afd683f6fb35" />

Route show for host 4:
<img width="789" height="145" alt="image" src="https://github.com/user-attachments/assets/eb014569-d5a0-47d4-aead-2108343a7dba" />

Conclusion:
To sum up, the ARP functions to register IP addresses on the MAC address and a default gateway is required for communicating with networks outside • the current subnetwork. When the hosts were communicating using ARP, some hosts would either have empty or an incomplete ARP table but as they communicated with one another, these ARP tables would build up what was called the ARP mapping between IP and MAC addresses. As well, as the ARP table would change to different levels, ARP just kept track of how much the devices in their subnet would change.

The default gateway would also work in a similar manner by configuring the devices' IP addresses, enabling the routers' forwarding of the packets and assigning the correct gateway for each of the hosts; these settings allowed them to communicate across the different subnets that were created. After testing the pings with 100% success the routes worked as intended + the routing table provided a way to see how the devices/hosts travelled through the network. Overall, the two examples of verifying the ARP process and that the routing process worked correctly showed how critical it was for the ARP to work for inter-communication.


Reflection:
This project was an excellent opportunity for me to work with the fundamental principles of networking in a hands-on manner. One of my key takeaways from this project was learning about how ARP works. I learned ARP works "behind-the-scenes" and cannot be seen just by looking at ARP tables until actual ARP requests have been made and ARP tables actually contain information (as an example, I could see how a new entry gets created in the ARP table after executing ping commands). This was helpful in explaining how devices discover each other on a network.
 I also learned about the function or purpose of default gateways and their role in facilitating communication between devices on different subnets. When I was configuring the routers and ensuring that IP forwarding was enabled, it was helpful to see how the devices or hosts behave differently than routers. When I was first setting up the appropriate IP address and gateway configurations for the devices, I paid close attention to the configuration to make sure that I did not put an error because any errors that I made in these areas would have prevented me from being able to communicate with a device. I also learned a lot about the logic of routing and how to design networks through troubleshooting when an error was present in configuration.
In conclusion, this project helped to solidify my practical networking skills and helped me gain more insight into how data flows throughout and in-between networks. Another of my key takeaways was that I need to have a systematic way of testing and verifying the configuration of a network, such as pinging and checking routing tables.
















