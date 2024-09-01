# osticket-prereqs
OS Tickets Repository
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Installation and Prerequisites</h1>
 Walkthrough: Setting Up osTicket on Windows 10 with a Web Server Environment

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- >Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

 - Web Server- You need a web server such as IIS.

 - PHP- osTicket requires PHP to run.

 - Database- MySQL is commonly used for the database.

 - osTicket- Download the latest version from the osTicket website

- <h2>Create a Windows 10 Virtual Machine in Azure

- Create a Resource Group
- a)Resource groups are logical containers for Azure resources. Name it appropriately for easy identification.
- Create a Windows 10 Virtual Machine (VM) with 2-4 Virtual CPUs
- a)Set a Username for VMs and Password.(Note:username and Password must be easy to identify)

  <h2>Installation Steps</h2>
  <h2>Install IIS with CGI and Common HTTP Features:
- Navigate to Windows Features and select Internet Information Services (IIS).
- Expand World Wide Web Services.
- Go to Application Development Features and enable:
- Check [X] CGI
- Ensure Common HTTP Features are selected.
  <h2>Enable IIS Management Console:
- Under Internet Information Services, expand Web Management Tools.
- Check [X] IIS Management Console

  <h2> Download and Install PHP Manager for IIS:
- Locate the installation file PHPManagerForIIS_V1.5.0.msi
- Run the installer to install PHP Manager for IIS.

  <h2>Download and Install the Rewrite Module:
- Locate the installation file rewrite_amd64_en-US.msi.
- Run the installer to install the Rewrite Module for IIS.





<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>


<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
