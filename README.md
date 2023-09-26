# osticket-prereqs

<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>
- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>
-Create a Virtual Machine in Azure 
  -Create a Resource Group
-Installing PHP Manager System for IIS
-Download and Install the Rewrite Module
-Download of Zip file PHP under C Drive
-Download and Install Microsoft Visual C+ Redistrubutal 
-Download and Install My SQL Server with Typical Setup and Standard Configuration

Welcome to OS Ticket Lab. Listed above are the prerequisites needed for the lab. Below are the steps taken to install OS Ticket:

1) Create a resource Group in Azure.
2) Create a VM using Windows 10 with 2-4 Virtual CPUs.
   a. Let the VM create a Virtual Network
3) Go to Remote Desktop Connection
   a. Enter the Public IP address. This is where we will install files for the OS Ticket Platform.
4) Once we are on our remote desktop, we are going to INSTALL and ENABLE IIS( Internet Install Services) with Windows CGI to run OS Ticket.
   a. Go to Control in Systems(in the start menu), and click run-> Control Parts Program-> Turn Windows on and off.
   b. Scroll Down to Internet Information Services->Web Management Tools-> Click on IIS Management Console
   c. Scroll down to World Wide Web Services-> Application Development and Features. Check CGI and common HTTP Feature-let that install (to check if installed correctly, open a new tab browser and type 127.0.0.1)
5) Go back to the PHP Manager for IIS, and click DOWNLOAD and INSTALL.
6) Install Rewrite Module
   a.Next create a directory C:\\PHP. Next, go to This PC->Drivers->C Drive-> New Folder and call it PHP.
   b.Go back to the install list-> PHP 7.3.8. Extract all and unzip the PHP Folder in the C Drive: C:\\PHP Folder.
7) Go back to the Install list and DOWNLOAD AND INSTALL VC redist.
8) From the Installation Files, DOWNLOAD AND INSTALL MySQL 5.5.62
   a. Go to typical setup, and launch the configuration wizard (after the installation).
   b. Go to standard configuration, and enter the password (password1 or whichever of your choosing).
9) Next we are going to open IIS as ADMIN
10) Register PHP from within IIS
11) Reload IIS (Open IIS, Stop and Start the server)
12) Go to sites, default, then to OS ticket. On the right side click "browse 80"
13) Before we continue, we need to go back and enable extensions.
    a.Go back to IIS, site->Defualt->OS ticket
    b.Double-Click PHP Manager
    c.Click"Enable or Disable and Extension"
      1. ENABLE php_imap.dll
      2. ENABLE php_intl.dll
      3. ENABLE php_opcache dll
    d.Refresh the OS Ticket site in your browse, and observe the changes.
14)Next we are going to rename Ost-config.php
   a. From the C:\intepub\wwwroot\osTicket\inclde\ost-sampleconfig.php
   b. Change it to C:\intepub\wwwroot\osTicket\include\ost-config.php
15) Assign Permissions: ost-config.php
    a.Disable Interheritance->Remove All
    b.New Permissions->Everyone->All
16) Continue Setting up os Ticket in the browser (Click continue)
    a. Name Helpdesk
    b. Default Email (emails from customers)
17) From the Installation Files, provided above, DOWNLOAD AND INSTALL HeidiSQL
    a. Open Heidi SQL
    b. Create a new session, root/Password1( or whichever password you chose previously).
    c. Connect the session
    d. Create a database called "osTicket"
18) Continue Setting up os Ticket in the browser
    a. MySQL Database: osTicket
    b. MySQL Username: root (an example)
    c. MySQL Password: Password1 (enter the password you created)
    d. Click "Install Now!"
19) CONGRATULATIONS! You have now installed osTicket. To access log-in page and browse you can access it here: http://localhost/osTicket/scp/login.php
20) Note:End Users osTicket URL: http://localhost/osTicket/
![image](https://github.com/mroesberry988/osticket-prereqs/assets/134666751/911952b2-0af2-4758-8e14-1a9ef14041d3)

![image](https://github.com/mroesberry988/osticket-prereqs/assets/134666751/f2c2f459-f71b-4d00-9631-d2e141a23972)


<h2>Installation

![image](https://github.com/mroesberry988/osticket-prereqs/assets/134666751/4d55c627-e589-4067-a952-47af4bfa903e)





![image](https://github.com/mroesberry988/osticket-prereqs/assets/134666751/fde07ccc-33af-4de4-89e6-fa3bc25902fb)

![image](https://github.com/mroesberry988/osticket-prereqs/assets/134666751/e6bcab13-05df-40cf-881a-a7d5d15d3e35)





![image](https://github.com/mroesberry988/osticket-prereqs/assets/134666751/9267e7e1-42c8-4709-8a10-9e618bef2faf)



