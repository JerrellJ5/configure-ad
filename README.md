<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://www.youtube.com/watch?v=wuIE4p4io7Q)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Setup Domain Controller and Domain controller-2 in Azure 
- Use Remote desktop to simulate a virtual machine using Windows server and Windows 10
- Deploy Active Directory 
  

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/qAeaOtg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Deployed two virtual machines (DC-1 and DC-2) in Azure to establish a robust Active Directory environment. Configured DC-1 as the primary domain controller, installed Active Directory Domain Services, and promoted it to manage the domain. DC-2 was set up as a secondary domain controller to ensure redundancy and load balancing, providing a failover solution for improved reliability and security within the domain.
</p>
<br />

<p>
<img src="https://i.imgur.com/5s9N90n.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Utilized Remote Desktop to simulate virtual environments, connecting to a Windows Server and Windows 10 virtual machine. Configured and managed the Windows Server VM for server-side operations, while the Windows 10 VM was used for client-side simulation. This setup allowed for testing, system management, and network administration in a controlled virtual environment.
</p>
<br />

<p>
<img src="https://i.imgur.com/l2mY0NT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Deployed Active Directory on a Windows Server using PowerShell for streamlined automation. Installed the 'AD DS' (Active Directory Domain Services) role with `Install-WindowsFeature` cmdlet, and used `Install-ADDSForest` to promote the server to a domain controller. This approach simplified the setup process, allowing for quick, efficient domain management and configuration through scripting.
</p>
<br />
