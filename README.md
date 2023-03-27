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

- Item 1 - First sign up for Microsoft Azure account. Then create a VM (Virtual Machines) in Azure. To do this you will first need to create a Resource Group.
- Item 2 - Then Create a Virtual Machine in Microsoft Azure using the same resource group.The VM will need to be in Windows 10 using a 2-4 Virtual CPUs and it must be allowed to create a new Virtual Network (Vnet).
- Item 3 - Download Remote Desktop application so you can connect to the VM
- Item 4 - Click on the VM (VM-osticket) to get the IP address. Once you have the IP copy and pase it into the remote desktop application. Then add PC and login with the same username/password that was created when making the VM.
- Item 5 - 

<h2>Prerequisite Steps</h2>

<p>
<img src="https://i.imgur.com/P8QPmTr.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Created the VM in Azure using the same resource group. Click on the VM-osticket.
</p>
<br />

<p>
<img src="https://i.imgur.com/jqQEKsq.jpg height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Copy the IP address assigned in the VM-osticket.
</p>
<br />

<p>
<img src="https://i.imgur.com/aftdaT8.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open Microsoft Remote Desktop and click add new PC.
</p>
<br />

<p>
<img src="https://i.imgur.com/MRVr9px.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Paste the IP address copied from VM-osticket.
</p>
<br />

<p>
<img src="https://i.imgur.com/JC9PZfB.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Input the username and password use to set up the VM.
</p>
<br />

<p>
<img src="https://i.imgur.com/V44A2wn.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Wala..!! the VM is successfully opened.
</p>
<br />

<p>
<img src="https://i.imgur.com/ALiVkoG.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This is what the VM should look like once you are complete.
</p>
<br />

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/J2ezyFA.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Right click on start. Click on run. Then type in control. Once your in control click on programs, turn windows features on or off. Scroll down to IIS (Internet Information Services), click and expand it, expand WWS (WorldWide Web Services), expand application development, click on CGI then click ok. This step will install and enable IIS in windows with CGI. 
</p>
<br />

<p>
<img src="https://i.imgur.com/JApqyti.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download PHPManagerforIIS
</p>
<br />
<p>
<img src="https://i.imgur.com/yQ7CQng.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and install the rewrite module
</p>
<br />

<p>
<img src="https://i.imgur.com/IGiP9zO.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and install PHP 7.3.8 and create a new directory in C drive C:\PHP. To do this go into the C drive, right click on new, folder, rename it PHP. Then relocate the PHP 7.3.8 file into the C drive by extracting it to the PHP folder
</p>
<br />

<p>
<img src="https://i.imgur.com/BJ0Twdw.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download VC_redist.x86.exe
</p>
<br />

<p>
<img src="https://i.imgur.com/iTAa84g.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download Mysql. Once it is install follow the instructions and create a password to root. Then click execute.
</p>
<br />
                                                                                                 
<p>
<img src="https://i.imgur.com/BJ0Twdw.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />  
                                                                                                 
<p>
<img src="https://i.imgur.com/BJ0Twdw.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />  
                                                                                                 
<p>
<img src="https://i.imgur.com/BJ0Twdw.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />                                                                                                 
