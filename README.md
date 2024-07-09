# Active Directory & Group Policy Management Home Lab
## Introduction
In this home lab I walked through how to create an Active Directory Environment using VMware Workstation Pro. Configuring and running this lab helped develop my understanding of how active directory and windows networking works.
## Utilities used
- [VMware Workstation Pro](https://www.vmware.com/products/workstation-pro/html.html)
- Windows Powershell
## Environment used (Both virtualized)
- Windows Server 2022
- Windows Enterprise LTSC 21H2
## Lab Setup Overview
- ### Setting up the Windows Server (AD Server) Virtual Environment: 
The initial step involves setting up the virtual environment using VMware Workstation Pro. This process includes creating a new virtual machine, allocating necessary resources such as memory and storage (In my case I am allocating 2 Cores, 6GB Memory, 100GB Storage to both of these VMs), and installing Windows Server 2022 as the operating system.

![Screenshot 2024-07-09 174239](https://github.com/Ironfist69/AD-Management-Home-Lab/assets/70436487/5add46bb-1563-4f15-a499-1d517ad09620)

- ### Deploying Active Directory Environment:
Once the operating system is installed, the next phase is to configure Windows Server 2022 to function as an Active Directory server. This configuration involves setting up the server roles and features, configuring networking settings, and setting up the Active Directory Domain Services role.

![Screenshot 2024-07-09 174946](https://github.com/Ironfist69/AD-Management-Home-Lab/assets/70436487/a569ae63-3fa2-41ce-a2a9-3cd6396cdf40)


![Screenshot 2024-07-09 180713](https://github.com/Ironfist69/AD-Management-Home-Lab/assets/70436487/84147277-a9a9-47f5-a836-de89765b4395)

Assigning static IP to our AD server

![AD Project (4)](https://github.com/Ironfist69/AD-Management-Home-Lab/assets/70436487/9903abf7-7190-424e-a72f-3bdc00d3b734)

- ### Managing Active Directory:
Created 4 Organizational unit in the domain and created a user with my name and added him into IT Group

![Screenshot 2024-07-09 212811](https://github.com/Ironfist69/AD-Management-Home-Lab/assets/70436487/918bc782-a840-4494-9502-59f11bc2d0cf)



Now we'll move on to the next step for creating client machine

## Setting up the Windows Enterprise LTSC (Client) Virtual Environment: 

![Screenshot 2024-07-09 213737](https://github.com/Ironfist69/AD-Management-Home-Lab/assets/70436487/9f49c695-aa39-4aff-a7c7-a3cbcefb98f8)

- ### Connected client to Server:
Successfully established connection betweent the Server and Client using the Server's IP Adrress as DNS server on Client side

![AD Project (2)](https://github.com/Ironfist69/AD-Management-Home-Lab/assets/70436487/78b52353-0a86-4a25-853b-82949ac3e3bd)
