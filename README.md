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

Welcome to OS Ticket Lab. Above listed is the prerequistes need for the lab. Below are the steps taken to install OS Ticket:

1) Create a resource Group in Azure.
2) Create a VM using Windows 10 with a 2-4 Virtual CPUs.
   a. Let the VM create a Virtual Network
3) Go to Remote Desktop Connection
   a. Enter the Public IP address. This is where we will install files for the OS Ticket Platform.
4) Once we are in our remote desktop, we are going to INSTALL and ENABLE IIS( Internet Install Services) with Windows CGI to run OS Ticket.
   a. Go to Control in Systems(in the start menu), and click run-> Control Parts Program-> Turn Windows on and off.
   b. Scroll Down to Internet Information Services->Web Management Tools-> Click on IIS Management Console
   c. Scroll down to World Wide Web Services-> Application Development and Features. Check CGI and common HTTP Feature-let that install (to check if installed correctly, open a new tab browser and type 127.0.0.1)
5) Go back to the PHP Manager for IIS, and click DOWNLOAD and INSTALL.
6) Install Rewrite Module
   a.Next create a directory C:\\PHP. Next, go to This PC->Drivers->C Drive-> New Folder and call it PHP.
   b.Go back to the install list-> PHP 7.3.8. Extract all and unzip the PHP Folder in the C Drive: C:\\PHP Folder.
7) Go back to the Install list and DOWNLOAD AND INSTALL VC redist.
8) Also from the Installation Files, DOWNLOAD AND INSTALL MySQL 5.5.62
   a. Go to typical setup, launch configuration wizard (after the install).
   b. Go to standard configuration, enter password.
9) Next we are going to open IIS
10) Register PHP from within IIS
11) Reload IIS (Open IIS, Stop and Start the server)
12) Go to sites, default, then to OS ticket. On the right side click "browse 80"
13) Before we continue, we need to go back and enable extenstions.
    a.Go back to IIS, site->Defualt->OS ticket
    b.Double-Click PHP Manager
    c.Click"Enable or Disable and Extension"
      1. ENABLE php_imap.dll
      2. ENABLE php_intl.dll
      3. ENABLE php_opcache dll
    d.Refresh the OS Ticket site in your browse, observe the changes.
14)
![image](https://github.com/mroesberry988/osticket-prereqs/assets/134666751/911952b2-0af2-4758-8e14-1a9ef14041d3)

![image](https://github.com/mroesberry988/osticket-prereqs/assets/134666751/f2c2f459-f71b-4d00-9631-d2e141a23972)


<h2>Installation

![image](https://github.com/mroesberry988/osticket-prereqs/assets/134666751/4d55c627-e589-4067-a952-47af4bfa903e)





![image](https://github.com/mroesberry988/osticket-prereqs/assets/134666751/fde07ccc-33af-4de4-89e6-fa3bc25902fb)

![image](https://github.com/mroesberry988/osticket-prereqs/assets/134666751/e6bcab13-05df-40cf-881a-a7d5d15d3e35)





![image](https://github.com/mroesberry988/osticket-prereqs/assets/134666751/9267e7e1-42c8-4709-8a10-9e618bef2faf)



