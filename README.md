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
<img src="https://i.imgur.com/cgILGS4.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To register PHP manager. First open IIS as an admin, the click PHP manager, register, browse for PHP, then click PHg-cgi. Once you have done that go back to vm-osticket and restart IIS.
</p>
<br />  
                                                                                                 
<p>
<img src="https://i.imgur.com//s8QIzCY.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once Osticket is downloaded. The file upload in www.root has to be renamed as osticket. In order to do this locate the C-drive, inetpub, wwwroot. Drop upload into wwwroot then rename it to osticket. Then go to IIS click sites, default web, osticket then browse *:80 on the left. Doing so will show that osticket is now installed.
</p>
<br />  
                                                                                                 
<p>
<img src="https://i.imgur.com/nFg4vQr.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Then go to the C-drive locate inetpub,wwwroot, osticket, ost-sampleconfig.php and rename it to ost-config.php. Once that is done we can now assign permissions to everyone by right clicking ost-config.php. Then properties to give everyone permission and disable inheritance
</p>
<br />                                                                                                 

  <p>
<img src="https://i.imgur.com/8S38R11.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Continue setting up Osticket
</p>
<br /> 
                                                                                                 
 <p>
<img src="https://i.imgur.com/mZFxwP7.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download HeidiSql and setup the admin username, password and email
</p>
<br />                      
                                                                                                 
 <p>
<img src="https://i.imgur.com/nDo5PS2.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Osticket is now running successfully.
</p>
<br />                      
                                                                                                 
 <p>
<img src="https://i.imgur.com/Vr0kcxc.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Login in with the same admin account that was used to setup Osticket.
</p>
<br />                      
                                                                                                 
 <p>
<img src="https://i.imgur.com/sliP5tJ.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This is what Osticket (ticketing system) looks like when it is installed correctly.
</p>
<br />                                                                                                                      
