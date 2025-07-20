# Azure-PrivateMesh-Lab

## Objective

This project aims to design and implement a Hub-and-Spoke network architecture in Microsoft Azure, integrating it with an on-premises setup via a Site-to-Site (S2S) VPN connection. The goal is to enable secure, scalable, and efficient communication between on-prem resources and Azure workloads while enforcing centralized security policies.

## Skills Learned

**Azure Networking:** Configured Virtual Networks (VNets), subnets, and VNet peering.

**Hybrid Cloud Integration:** Established Site-to-Site VPN connectivity between Azure and an on-premises Domain Controller.

**Security & Access Control:** Implemented Azure Firewall, User-Defined Routes (UDRs), and Private DNS for enhanced security and controlled traffic flow.

**Remote Access & Management:** Configured Azure Bastion for secure remote access to VMs without exposing RDP/SSH ports.


## Architecture Overview


 ![SS](Screenshots/Hub&spokes-Page.png)



**On-Premises Setup:**

* Domain Controller (DC) (For setup : https://github.com/Sakshi95Si/AD-Domain_Lab )

* Site-to-Site VPN Connection to Azure

**Azure Hub-and-Spoke Design:**

Hub Network:

* Virtual Network Gateway (for S2S VPN)

* Azure Firewall (for centralized security)


Spoke Networks:

* Peered with the Hub for connectivity

* Subnets configured with NSGs and UDRs


**Access & Security:**

* Azure Bastion for secure VM access

* Traffic flow managed via Azure Firewall and UDRs



## Tools & Services Used

**Networking:** Virtual Networks, Subnets, VNet Peering

**Security:** Azure Firewall, NSGs, UDRs

**Hybrid Connectivity:** Site-to-Site VPN, Virtual Network Gateway

**Management & Access:** Azure Bastion, Azure Portal
