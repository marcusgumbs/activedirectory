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

- Create VMs (Domain controller via Windows Server and Client via Windows 10)
- Install Active Directory Domain Services
- Create Organizational Units
- Create accounts via script
- Perform actions within accounts
  

<h2>Deployment and Configuration Steps</h2>

<p>
<img width="349" alt="Screenshot 2024-03-06 200347" src="https://github.com/marcusgumbs/activedirectory/assets/162270050/1363c22d-d892-4924-a665-bde51e170a4e">

</p>
<p>
Created the Domain Controller VM (Windows Server 2022) named “DC-1”
Set the Domain Controller’s NIC Private IP address to be static
Create the Client VM (Windows 10) named “Client-1”. Used the same Resource Group and Vnet that was created for DC1. Ensured that both VMs were in the same Vnet. Logged in to DC-1 and installed Active Directory Domain Services.

</p>
<br />

<p>
<img width="655" alt="Screenshot 2024-03-06 200457" src="https://github.com/marcusgumbs/activedirectory/assets/162270050/381ec6ea-63e2-4797-af72-24629c514581">

</p>
<p>
In Active Directory Users and Computers (ADUC) I created organizational units (employees, clients, and admins). I then ran a script in powershell comprised of self generated accounts that will be used for various tasks.
</p>
<br />

<p>
<img width="349" alt="Screenshot 2024-03-06 200643" src="https://github.com/marcusgumbs/activedirectory/assets/162270050/33ca519e-763c-46b1-927a-c18b00990d7b">

</p>
<p>
I learned to create/reset passwords, disable/enable accounts, add users to different groups, etc.
</p>
<br />
