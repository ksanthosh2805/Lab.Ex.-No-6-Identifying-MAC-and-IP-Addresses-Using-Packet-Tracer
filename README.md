# Ex. No: 6 Identifying MAC and IP Addresses Using Packet Tracer
## Date: 13-09-2025
## Name: Santhosh K
## RegNo: 212223100050
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
(Insert screenshot of your Packet Tracer setup here)<br>
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
#### •	PDU details for local communication(Pinging from 172.16.31.5 to 172.16.31.2)<br>

##### At 172.16.31.5

<img width="630" height="609" alt="Screenshot 2025-09-13 141429" src="https://github.com/user-attachments/assets/e6c43d50-0f33-4de1-8f60-ae1823624c60" />
<br>

##### At 172.16.31.2

<img width="630" height="625" alt="Screenshot 2025-09-13 141516" src="https://github.com/user-attachments/assets/35fd84ad-f3f8-474c-882e-5181c59f495d" />
<br>

#### •	PDU details for remote communication(Pinging from 172.16.31.5 to 10.10.10.2)<br>

##### At 172.16.31.5
<img width="630" height="608" alt="image" src="https://github.com/user-attachments/assets/da7f7289-ee4f-422d-9efb-988b4dfc0daa" />

<br>

##### At 10.10.10.2
<img width="630" height="608" alt="image" src="https://github.com/user-attachments/assets/0c380fbd-dc53-4185-93b1-073988454bd7" />

#### •	Tables showing MAC/IP changes through each device<br>

##### Local Communication(From 172.16.31.5 to 172.16.31.2)
<img width="622" height="137" alt="image" src="https://github.com/user-attachments/assets/5e4c28b1-085d-459c-8bbc-f28ff7f63d16" />

##### Remote Communication(From 172.16.31.5 to 10.10.10.2)
<img width="616" height="187" alt="image" src="https://github.com/user-attachments/assets/6d59484e-2360-4cb5-bd80-2cb70851bd11" />


________________________________________
# Result
Successfully captured and analyzed MAC and IP addresses for both local and remote communications. Verified that MAC addresses change at each hop while IP addresses remain constant from source to destination.
