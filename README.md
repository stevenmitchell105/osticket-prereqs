# osticket-prereqs

<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Create a Virtual Machine in Azure

- Install osTicket v1.15.8

- Install HeidiSQL

- Install MySQL

- Install PHP

- install Microsoft Visual C++ Redistributable

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/eBi5k2l.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First, start by creating a Resource Group inside Azure
</p>
<br />

<p>
<img src="https://i.imgur.com/dEF1c7h.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now, create a Windows 10 Virtual Machine (VM), typically with 2-4 Virtual CPUs. For username and password, it can be anything as we'll be using this info to remote in with our main computer. When creating the Virtual Machine (VM), allow Azure to create a new Virtual Network (Vnet)
</p>
<br />

<p>
<img src="https://i.imgur.com/FjwdtJk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open your Remote Desktop Connection app on your computer and connect to your Virtual Machine that was created in Azure.
</p>
<br />

<p>
<img src="https://i.imgur.com/NE5ftYj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now we need to install / Enable IIS in Windows. Go to your Search Bar > Type "Control Panel" > Click "Programs" > "Turn Windows features on or off" > Scroll down to "Internet Information Services (IIS).
</p>
<br />

<p>
<img src="https://i.imgur.com/LdVGE9a.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once clicked, find the "Internet Information Services" expand it and then expand the "World Wide Web" tab. Afterward, expand the application Developer tab. Finally check the "CGI" button & press Ok. You will need CGI to download the PHP Manager. The PHP manager is a back-end web programming language that allows osTicket to run off a web browser.
</p>
<br />

<h3 align="center">Now Install PHP Manager</h3>
<br />

<p>
<img src="https://i.imgur.com/pmwpPEu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download the PHP manager file, and agree with all the terms. We've now downloaded the PHP manager into our operating system.
</p>
<br />

<h3 align="center">Install Rewrite Module</h3>
<br />

<p>
<img src="https://i.imgur.com/aDlN2c4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download the Rewrite Module file, agree with all the terms and it should now be installed onto the Computer.
</p>
<br />

<br/>
<h3 align="center">CREATE DIRECTORY C:\PHP</h3>
<br />

<p>
<img src="https://imgur.com/hvp56iB" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open File Explorer, type, "C:\" in the search bar, Right-click and create a new folder called, "PHP". Download php-7.3.8-nts-Win32-VC15-x86.zip from Files You Need to Download, Extract it by going to where you download the file, Right-click the PHP 7.3.8 file and press extract to the PHP Folder you just created.
</p>

<br/>
<h3 align="center">VC_REDIST DOWNLOAD</h3>
<br />

<p>
<img src="https://i.imgur.com/Gx8ryBV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and install VC_Redist, Agree with any terms and agreements and finish installing.
</p>

<h3 align="center">DOWNLOAD MySQL </h3>

<p>
<img src="https://i.imgur.com/IVpLg40.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/zdhWXNx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and install MySQL, Agree with any terms and agreements up until you get to the password portion. Here you can create a username and password for the database that you'll be using to store the Ticket Information used in osTicket. 

</p>

<h3 align="center">Install osTicket v1.15.8</h3>

<img src="https://i.imgur.com/0MUJLMU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/1h9goM8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
Extract and copy the “upload” folder INTO c:\inetpub\wwwroot:
</p>
<img src="https://i.imgur.com/pDikkgq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”:
</p>

<h3 align="center">Reload IIS (Open IIS, Stop and Start the server)</h3>

<p>
	<img src="https://i.imgur.com/QeWNlG3.png" height="75%" width="100%" />
</p>
<p>
	Go to sites -> Default -> osTicket:
</p>

<p>
	<img src="https://i.imgur.com/3iXhNbi.png" height="75%" width="100%"/>
</p>
<p>
	On the right, click “Browse *:80”:
</p>
<p>
	<img src="https://i.imgur.com/3iXhNbi.png" height="75%" width="100%"/>
</p>

