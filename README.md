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
