<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, Prerequisites and Installation](https://www.youtube.com/watch?v=hDPEtOzDSPY)



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Enable Internet Information Services (IIS)
- Web Platform Install
- Install My SQL (Set Up Usernames And Passwords)
- Configure permissions and Install Osticket

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/GHNUHGr.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/oGl7432.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
After I created my Azure Virtual Machine Windows 10, 4 vCPUs and named it 'osticket-vm'. I Logged into the VM with Remote Desktop. Within the VM (osticket-vm), I downloaded the osTicket-Installation-Files.zip and unzip it onto my desktop. I am going to use the files in this folder to install osTicket and some of the dependencies. I went ahead and Installed / Enabled IIS in Windows WITH CGI (World Wide Web Services -> Application Development Features -> [X] CGI.) Checked by checking the local host, 127.0.0.1 to loot back.
</p>
<br />

<p>
<img src="https://i.imgur.com/52eS6Pr.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the “osTicket-Installation-Files” folder, I installed PHP Manager for IIS, Rewrite module, PHP 7.3.8, VC_redist.x86.exe
</p>
<br />

<p>
<img src="https://i.imgur.com/0Ks09Rd.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/fwnz4i8.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/zhhiJds.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/mQQgNUz.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install my SQL, Typical setup, Launch configuration WIzard (after install), Standard Configuration, Setup Root Password. What this does is installs a database for this computer (osticket). 
</p>
<br />

<p>
<img src="https://i.imgur.com/VLRRjA1.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/4t1mHDX.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/h0Sv9wR.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/OOZVlwc.jpeg" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Back to IIS, sites -> Default -> osTicket, Double-click PHP Manager, Clicked the Enable or disable the following extensions:
Enable: php_imap.dll
Enable: php_intl.dll
Enable: php_opcache.dll
Assign Permissions: ost-cofig.php, Downloaded and installed HeidiSQL, continued setting up osticket in the browser
</p>
<br />
