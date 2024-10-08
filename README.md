# osticket-prereqs
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Installation and Prerequisites</h1>
osTicket is an open-source, web-based customer support ticket system that manages customer support by organizing and tracking requests through tickets, ensuring efficient and effective handling of customer issues.

# Walkthrough: Setting Up osTicket on Windows 10 with a Web Server Environment

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- >Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>
 
- Microsoft Azure
- Virtual Machine
- osTicket Installation Files

- <h2>Create a Windows 10 Virtual Machine in Azure

- Create a Resource Group > a)Resource groups are logical containers for Azure resources. Name it appropriately for easy identification.
- ![RG](https://github.com/user-attachments/assets/92a84fa3-e6af-4d80-a950-0d95a68a4a63)
- Create a Windows 10 Virtual Machine (VM) with 2-4 Virtual CPUs> a)Set a Username for VMs and Password.(Note:username and Password must be easy to identify)
  ![vmd](https://github.com/user-attachments/assets/a5605635-959b-4add-8ac8-d5b3804b6c60)

  <h2>Installation Steps</h2>
  <h2>Install IIS with CGI and Common HTTP Features:
- Navigate to Windows Features and select Internet Information Services (IIS).
- Expand World Wide Web Services.
- Go to Application Development Features and enable:
- ![ppp](https://github.com/user-attachments/assets/dfe0c5db-2683-43ca-aefd-f477840bfdb9)
- Check [X] CGI
- Ensure Common HTTP Features are selected.
  <h2>Enable IIS Management Console:
- Under Internet Information Services, expand Web Management Tools.
- Check [X] IIS Management Console

  <h2> Download and Install PHP Manager for IIS:
- Locate the installation file PHPManagerForIIS_V1.5.0.msi
- Run the installer to install PHP Manager for IIS.
  ![php](https://github.com/user-attachments/assets/13c0b84d-aec1-416b-b865-8a9758ee11cf)

  <h2>Download and Install the Rewrite Module:
- Locate the installation file rewrite_amd64_en-US.msi.
- Run the installer to install the Rewrite Module for IIS.
  ![VC RE](https://github.com/user-attachments/assets/4ef04cbc-5168-4a39-bdc1-9889637bdd78)

  <h2>Download and Install MySQL 5.5.62 
 - Typical Setup >- Launch Configuration Wizard (after install)>- Standard Configuratio> Password
 - Open IIS as an Admin-> Register PHP from within IIS ->Reload IIS (Open IIS, Stop and Start the server)

  <h2>Install osTicket v1.15.8
- Download osTicket > Extract and copy “upload” folder to c:\inetpub\wwwroot>Within c:\inetpub\wwwroot, Rename “upload” to “osTicket

- Reload IIS (Open IIS, Stop and Start the server)>Go to sites -> Default -> osTicket>On the right, click “Browse *:80”

- Note that some extensions are not enabled  >Go back to IIS, sites -> Default -> osTicket > Double-click PHP Manager > Click “Enable or disable an extension”
 Enable: php_imap.dll > Enable: php_intl.dll > Enable: php_opcache.dll > Refresh the osTicket site in your browse, observe the changes

- Rename: ost-config.php > From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php > To: C:\inetpub\wwwroot\osTicket\include\ost-config.php
-  Assign Permissions: ost-config.php > Disable inheritance -> Remove All > New Permissions -> Everyone -> All
- Continue Setting up osTicket in the browser (click Continue) > Name Helpdesk > Default email (receives email from customers)


- Download and install HeidiSQL. > Open Heidi SQL > Create a new session, root/Password1 > Connect to the session > Create a database called “osTicket”

- Continue Setting up osticket in the browser
  MySQL Database: osTicket
  MySQL Username: root
  MySQL Password: Password1
  Click “Install Now!”

- This walkthrough provided a step-by-step guide to installing and configuring osTicket, ensuring that all necessary prerequisites and settings are in place. By following these instructions, you should now have full functional osticket.













