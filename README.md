<p align="center">
    <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>
Microsoft Azure (Virtual Machines/Compute)
Remote Desktop (RDP)
Internet Information Services (IIS)
MySQL Database
PHP

<h2>Operating Systems Used</h2>

- Windows 10 (21H2)

<h2>List of Prerequisites</h2>
Windows VM on Microsoft Azure
Remote Desktop (mstsc.exe)
IIS with PHP Manager
MySQL Database
Visual C++ Redistributable
osTicket Installer

<h2>Installation Steps</h2>
Below are the steps to install and configure osTicket:

<h3>Step 1: Set up a Virtual Machine in Microsoft Azure</h3>
- Provision a new Windows 10 VM in Microsoft Azure.
- Assign appropriate resources like CPU and RAM depending on your workload.
<p>
    <img src="https://i.imgur.com/yourazureimage.png" height="80%" width="80%" alt="Azure VM Setup"/>
</p>

<h3>Step 2: Connect to the VM via Remote Desktop</h3>
- Open Remote Desktop (mstsc.exe) and enter the public IP address of your Azure VM.
- Log in with the credentials set up in Azure.
<p>
    <img src="https://i.imgur.com/yourremoteimage.png" height="80%" width="80%" alt="Remote Desktop Connection"/>
</p>

<h3>Step 3: Install IIS (Internet Information Services)</h3>
- Use the Windows Features tool to install IIS.
- Ensure that PHP Manager is also installed and enabled for IIS.
<p>
    <img src="https://i.imgur.com/youriisimage.png" height="80%" width="80%" alt="IIS Setup"/>
</p>

<h3>Step 4: Install PHP and MySQL</h3>
- Install PHP using PHP Manager for IIS.
- Set up MySQL to store osTicket’s ticketing data.
<p>
    <img src="https://i.imgur.com/yourphpmysqlimage.png" height="80%" width="80%" alt="PHP and MySQL Setup"/>
</p>

<h3>Step 5: Download and Configure osTicket</h3>
- Download the latest version of osTicket from the [official website](https://osticket.com/download).
- Extract the installation files and place them in the IIS web directory (usually `C:\inetpub\wwwroot`).
<p>
    <img src="https://i.imgur.com/yourosticketimage.png" height="80%" width="80%" alt="osTicket Setup"/>
</p>

<h3>Step 6: Complete the Installation Wizard</h3>
- Open a web browser and navigate to `http://<your-vm-ip>/osTicket/`.
- Follow the on-screen instructions to complete the installation.
- Configure osTicket with the MySQL database and other required settings.
<p>
    <img src="https://i.imgur.com/yourinstallwizardimage.png" height="80%" width="80%" alt="osTicket Installation Wizard"/>
</p>

<h2>Conclusion</h2>
You have successfully installed osTicket on your Azure Virtual Machine using IIS, PHP, and MySQL. You can now begin using osTicket for managing helpdesk tickets.
