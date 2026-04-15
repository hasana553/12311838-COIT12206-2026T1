Week 3:
Introduction:
This assignment is designed to develop key foundational skills in networking through the use of GNS3 and will have a
significant emphasis on the testing of communication and performing packet analysis. The first part of this task will
utilize Netcat (nc) in a TCP or UDP communication simulation to test basic client-server communication between two hosts.
By doing so, this will aid in understanding how application-layer communication works on a network using both protocol families.
The second part of this task will focus on capturing packets using the same protocol families to give real-world examples of
packet transfer through TCP or UDP protocols and to facilitate basic understanding of how a network operates and how to collect
data for analysis with tools like Wireshark.
<img width="940" height="577" alt="image" src="https://github.com/user-attachments/assets/39d54351-aa7e-4f3c-a424-f1c5db746396" />
Configure of host 1
<img width="940" height="696" alt="image" src="https://github.com/user-attachments/assets/6d258795-0751-4e69-8edf-78a68f6586d0" />
Screenshot of host 4: 
<img width="940" height="388" alt="image" src="https://github.com/user-attachments/assets/cd024e17-4129-438e-8f39-100ad98bed60" />
Task 2:

Pinging from host 1 to host 3:
<img width="940" height="630" alt="image" src="https://github.com/user-attachments/assets/683dda64-7a8c-431b-a657-abf9fafbeadc" />
Attempting to ping non existing ip address from host 1:
<img width="940" height="524" alt="image" src="https://github.com/user-attachments/assets/c2d8c994-6248-449a-a775-403989b052e8" />
<img width="940" height="566" alt="image" src="https://github.com/user-attachments/assets/a9626bf5-884f-44a2-8693-84af0162d22a" />

Overall, the goal of this task has been to accurately demonstrate how to use Netcat to test and generate an analysis of 
connectivity between devices in GNS3 through packet capture methods. Also shown is how installing a Netcat Server and Client 
to simulate a real-time connection between two computers allows for confirmation of their ability to communicate at an application
level, thereby improving your understanding of the many different ways in which devices can send data to each other beyond simply
confirming they can communicate using basic Connection Tests (like Ping).

In addition, capturing the packets that were being transmitted during the data transfer process provided the ability to verify
that all of the required data (i.e., text, messages, documents), were indeed being transmitted between the two devices. Exporting 
or saving the data that was included in these packet captures highlights the need to preserve this type of network information, 
so that it can be used to assist in future network problem resolution and analysis as it relates to connectivity and performance 
issues.

Collectively these exercises will develop your hands-on experience with Networking Tools/Methods while establishing solid practices for all future exercises related to Network Security, Monitoring and analysis. The skills learned from this project are also very valuable in determining whether or not there are problems with communication between devices and in understanding how networks work in real applications.

Reflection:
All the host were successful and there were no issue while pinging from one host to another host.
This lab was very beneficial for us. The activities done in this lab taught me to create a new gns project. Firstly 
I added four linux hosts nodes and 1 ethernet switch after that I connect all the hosts using different ip addresses.
After that I pinged host 3 from host 1 and also ping non existence ip address from host 1.
Overall the lab activities helped me to assigned the ip addresses on multiple hosts and pinging from one host to another.

