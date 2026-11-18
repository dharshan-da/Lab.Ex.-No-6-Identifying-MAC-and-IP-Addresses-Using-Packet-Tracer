# Ex. No: 6 Identifying MAC and IP Addresses Using Packet Tracer
# Date:17:11:2026
________________________________________
# Objective
To use Cisco Packet Tracer simulation mode to capture and analyze MAC and IP address information for both local and remote network communication.
________________________________________
# Apparatus/Tools Required
•	Cisco Packet Tracer<br>
•	Pre-configured network topology (as provided in the activity file)<br>
•	PCs, switches, router, hub, and wireless access point (as per given setup)<br>
________________________________________
# Network Topology Diagram
# Description:
•	The topology contains a local network (172.16.31.0/24) connected to a remote network (10.10.10.0/24) via a router.<br>
•	Devices include PCs, switches, hub, and wireless AP.<br>
<img width="1600" height="897" alt="WhatsApp Image 2026-11-18 at 5 45 37 PM" src="https://github.com/user-attachments/assets/8cee657b-c63b-46df-8374-c1abf895aea1" />
<br>
________________________________________
# IP Addressing Table
(Example – actual values from simulation)<br>
Device	IPv4 Address	Subnet Mask	MAC Address<br>
PC-A	172.16.31.5	255.255.255.0	00D0:D311:C788<br>
PC-B	172.16.31.2	255.255.255.0	000C:85CC:1DA7<br>
Router (G0/0)	172.16.31.1	255.255.255.0	00D0:BA8E:741A<br>
PC-Remote	10.10.10.2	255.255.255.0	00D0:588C:2401<br>
________________________________________
# Procedure
# Part 1: Local Network Communication
1.	Click PC-A (172.16.31.5) and open the Command Prompt.<br>
2.	Enter ping 172.16.31.2.<br>
3.	Switch to Simulation Mode and repeat the ping.<br>
4.	When the PDU appears, click it and record: Destination MAC, Source MAC, Source IP, Destination IP, and the device name.<br>
5.	Use Capture/Forward to follow the PDU through the network until it reaches PC-B.<br>
6.	Record the information in a table.<br>
7.	Repeat the above process for:<br>
o	Ping from 172.16.31.3 to 172.16.31.2<br>
o	Ping from 172.16.31.5 to 172.16.31.4<br>
Part 2: Remote Network Communication<br>
1.	From PC-A (172.16.31.5), enter ping 10.10.10.2.<br>
2.	Switch to Simulation Mode and repeat the ping.<br>
3.	When the PDU appears, note the Destination MAC, Source MAC, Source IP, and Destination IP.<br>
4.	Follow the PDU step-by-step until it reaches the remote PC.<br>
5.	Observe how MAC addresses change at the router while IP addresses remain constant end-to-end.<br>
________________________________________
# Example Data Recording Table
At Device	Dest. MAC	Src MAC	Src IPv4	Dest IPv4<br>
172.16.31.5	000C:85CC:1DA7	00D0:D311:C788	172.16.31.5	172.16.31.2<br>
Switch1	000C:85CC:1DA7	00D0:D311:C788	N/A	N/A<br>
172.16.31.2	00D0:D311:C788	000C:85CC:1DA7	172.16.31.2	172.16.31.5<br>
________________________________________
# Output (Screenshots)
•	PDU details for local communication<br>
<img width="1600" height="900" alt="WhatsApp Image 2026-11-17 at 5 58 24 PM" src="https://github.com/user-attachments/assets/8149c0d3-0090-4168-939d-ca7fb65edce6" />
<img width="1600" height="899" alt="WhatsApp Image 2026-11-17 at 5 58 29 PM" src="https://github.com/user-attachments/assets/4d79e758-007f-414c-9c52-6417c2c548a6" />
<img width="1600" height="899" alt="WhatsApp Image 2026-11-17 at 5 58 38 PM" src="https://github.com/user-attachments/assets/427c0745-0dca-43d2-a009-fda7055b0ae3" />



•	PDU details for remote communication<br>
<img width="1600" height="900" alt="WhatsApp Image 2026-11-17 at 5 59 02 PM" src="https://github.com/user-attachments/assets/04e1c975-5433-4b8e-9abb-b000df0e7275" />

•	Tables showing MAC/IP changes through each device<br>
<img width="972" height="261" alt="WhatsApp Image 2026-11-18 at 5 48 21 PM" src="https://github.com/user-attachments/assets/7db6580b-e2cd-4135-8fa8-364a40a870d7" />

________________________________________
# Result
Successfully captured and analyzed MAC and IP addresses for both local and remote communications. Verified that MAC addresses change at each hop while IP addresses remain constant from source to destination.

