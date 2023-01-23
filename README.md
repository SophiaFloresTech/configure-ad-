<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Server Manager
- Install Active Directory
- Add Roles and Features

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/y3rSyWx.png"/>

<img src="https://i.imgur.com/AfFKLYE.png"/>

<img src="https://i.imgur.com/rol4WUn.png"/>

Install Active Directory
  -  Install Active Directory Domain Services (Server Manager) 
  -  Promote as a DC: Setup a new forest as mydomain.com  
  -  Restart and then log back into DC-1 as user: mydomain.com\labuser 


<img src="https://i.imgur.com/C7qgYWP.png"/>

 - Create an Admin and Normal User Account in AD
 
 _ In Active Directory Users and Computers (ADUC), create an Organizational Unit (OU) called “_EMPLOYEES” 
 
 _ Create a new OU named “_ADMINS” 
 
 _ Create a new employee named “Jane Doe” (same password) with the username of “jane_admin” 
 
 _ Add jane_admin to the “Domain Admins” Security Group 
 
 _ Log out/close the Remote Desktop connection to DC-1 and log back in as “mydomain.com\jane_admin” 
 
 _ User jane_admin as your admin account from now on


