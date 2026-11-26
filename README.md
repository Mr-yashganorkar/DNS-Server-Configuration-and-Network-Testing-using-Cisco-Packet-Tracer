<img width="1672" height="941" alt="Welcome Yash in Packet Tracer" src="https://github.com/user-attachments/assets/616385d1-29e7-42a4-bb1a-2cfcee2c5823" />

# DNS Configuration Using Cisco Packet Tracer

---


## Objective

- To configure DNS (Domain Name System) in Cisco Packet Tracer.
- To translate domain names into IP addresses within a local network.
- To allow client PCs to access network services using domain names instead of IP addresses.
- To configure IP addresses on the DNS server and client computers.
- To verify that DNS name resolution works correctly from all client devices.



## Requirements


- Cisco Packet Tracer software
- 1 Switch
- 1 Server (configured as DNS Server)
- 2 PCs (PC0 and PC1)
- Copper Straight-Through Ethernet cables
- Configured IP network (network address and subnet mask)
- DNS service enabled on the server
- DNS records configured on the DNS server
- DNS server IP address configured on all client PCs

  
## Step 1: Connect the Devices
Open Cisco Packet Tracer.

Drag and place the following devices into the workspace:

- 1 Switch
- 1 Server (DNS Server)
- 2 PCs (PC0 and PC1)
  
Connect all devices using Copper Straight-Through cables:

- Server0 to Switch
- PC0 to Switch
- PC1 to Switch

  
Wait until all device connections turn green, indicating that the network links are active.

This creates the basic network topology required for DNS configuration and communication between the server and client computers.

## Screenshot: Network Topology

<img width="940" height="499" alt="image" src="https://github.com/user-attachments/assets/12e2e55d-1f0e-420a-9dca-a73f1f936a3e" />



## Step 2: Configure DNS Service

After connecting all devices, the next step is to configure the DNS service on the server.


- Click on Server0 to open the server configuration window.
- Select the Services tab.
- From the list of available services on the left panel, click DNS.
- Make sure that the DNS Service is set to ON.
  
Enabling the DNS service allows the server to translate domain names into their corresponding IP addresses.

## Screenshot: DNS Service

<img width="1672" height="941" alt="Cisco Packet Tracer DNS Configuration" src="https://github.com/user-attachments/assets/0c7b906a-eacb-433c-8d93-fa2c4bd333dd" />



## Step 3: Configure DNS Records

After enabling the DNS service, configure the DNS records on the server.

- Open the Server configuration window.
- Select the Services tab.
- Click DNS from the left panel.
- Enter the required domain name in the Name field.
- Enter the corresponding server IP address in the Address field.
- Click Add to save the DNS record.
  
A DNS record maps a domain name to its corresponding IP address. This allows client computers to access network resources using domain names instead of IP addresses.

## Screenshot: DNS Service Configuration


<img width="1672" height="941" alt="Cisco Packet Tracer HTML Welcome Page" src="https://github.com/user-attachments/assets/abe12045-a1b3-487d-bb97-9c99689dde1e" />


## Step 4: Configure IP Address on PC0

After configuring the DNS service, assign an IP address to PC0.

- Click on PC0.
- Open the Desktop tab.
- Select IP Configuration.
- Select Static configuration.
- Enter the following IP settings:
  | Setting | Value |
|---|---|
| IP Address | `192.168.1.4` |
| Subnet Mask | `255.255.255.0` |
| Default Gateway | `0.0.0.0` |
| DNS Server | `192.168.1.4` |
  
This configuration assigns a static IP address to PC0 and sets the DNS server address to 192.168.1.4.

It allows PC0 to communicate with the DNS server and perform domain name resolution.

## Screenshot: PC0 IP Configuration


<img width="1672" height="941" alt="Cisco Packet Tracer PC0 IP Configuration" src="https://github.com/user-attachments/assets/090d01df-2eab-487b-8cdf-74db9210041d" />



## Step 5: Configure IP Address on PC1

After configuring PC0, the next step is to assign an IP address to PC1.

- Click on PC1.
- Open the Desktop tab.
- Select IP Configuration.
- Select Static configuration.
- Enter the following IP settings:
| Setting | Value |
|---|---|
| IP Address | `192.168.1.4` |
| Subnet Mask | `255.255.255.0` |
| Default Gateway | `0.0.0.0` |
| DNS Server | `192.168.1.10` |
This configuration assigns a static IP address to PC1 and sets 192.168.1.10 as the DNS server.

It allows PC1 to communicate with the DNS server and resolve domain names.

## Screenshot: PC1 IP Configuration


<img width="1671" height="941" alt="Cisco PC1 IP Configuration Window" src="https://github.com/user-attachments/assets/cc4c8be1-a686-4b6c-b21a-aad8c12eb1b7" />




## Step 6: Configure IP Address on the Server

After configuring the client PCs, assign a static IP address to the DNS server.

- Click on Server0.
- Open the Desktop tab.
- Select IP Configuration.
- Select Static configuration.
- Enter the following IP settings:
| Setting | Value |
|---|---|
| IP Address | `192.168.1.4` |
| Subnet Mask | `255.255.255.0` |
| Default Gateway | `0.0.0.0` |
| DNS Server | `192.168.1.4` |
This configuration assigns the IP address 192.168.1.10 to the DNS server.

The server uses its own IP address as the DNS server address to provide DNS services to client computers.

## Screenshot: Server IP Configuration



<img width="1671" height="941" alt="Cisco Server0 DNS Configuration Update" src="https://github.com/user-attachments/assets/e1633a34-9133-42d5-ab4a-a57eedbcd968" />



## Step 7: Verify DNS Configuration on PC0


After configuring the IP addresses and DNS settings, verify that DNS name resolution is working correctly on PC0.

- Click on PC0.
- Open the Desktop tab.
- Select the DNS testing option used in the configuration.
- Perform DNS testing using the configured domain name.
- Check the result to verify DNS name resolution.
  
This step verifies whether PC0 can successfully communicate with the DNS server and resolve the configured domain name.

## Screenshot: PC0 DNS Testing


<img width="1672" height="941" alt="Cisco Packet Tracer Web Browser Welcome Screen" src="https://github.com/user-attachments/assets/a3863d71-6031-4c67-bde5-e11ee3f14feb" />





## Step 8: Verify DNS Configuration on PC1


After successfully testing DNS on PC0, perform DNS testing on PC1.

- Click on PC1.
- Open the Desktop tab.
- Select the DNS testing option used in the configuration.
- Perform DNS testing using the configured domain name.
- Check the result to verify DNS name resolution.
  
This confirms that PC1 can also communicate with the DNS server and resolve the configured domain name.

## Screenshot: PC1 DNS Testing


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ec224117-9e1a-4347-b8b1-a9a41fcde912" />






## Result
The DNS configuration was implemented using Cisco Packet Tracer.

The network topology was created, DNS service was enabled, and IP addresses were assigned to the server and client computers.

The DNS server was configured with IP address 192.168.1.10.

Both client computers were configured with the following IP settings:

- PC0: 192.168.1.11
- PC1: 192.168.1.12
- DNS Server: 192.168.1.10
- Subnet Mask: 255.255.255.0
- 
DNS testing was performed from both PC0 and PC1 to verify the DNS configuration.

## Conclusion

The DNS Configuration project was completed using Cisco Packet Tracer.

This project demonstrated how DNS translates domain names into IP addresses and helps client computers communicate with servers using domain names.

Through this practical implementation, I gained knowledge of DNS service configuration, IP addressing, DNS records, network topology creation, and client-server communication.

## Author
Yash Ganorkar

Cyber Security Student















