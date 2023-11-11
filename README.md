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

- Enable IIS with CGI and Common HTTP Features
- Enable IIS Management Console
- Download and Install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi)
- Download and Install Rewrite Module (rewrite_amd64_en-US.msi)
- Create the directory C:\PHP
- Download PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) and unzip the contents into C:\PHP
- Download and install VC_redist.x86.exe.
- Download and install MySQL 5.5.62 (mysql-5.5.62-win32.msi)
- Open IIS as an Admin
- Register PHP from within IIS
- Reload IIS (Open IIS, Stop and Start the server)
- Download and Install osTicket v1.15.8
- Reload IIS (Open IIS, Stop and Start the server) and launch osTicket
- Enable extensions (php_imap.dll, php_intl.dll, opcache.dll)
- Rename: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php to C:\inetpub\wwwroot\osTicket\include\ost-config.php
- Assign Permissions: ost-config.php
- Setup osTicket ( Name helpdesk, assign default email)
- Download and install and configure HeidiSQL
- Continue setting up osTicket in browser with HeidiSQL configuration credentials
- Installation complete. Browse to your help desk login page: http://localhost/osTicket/scp/login.php

  

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/QUegyTk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
Open Control Panel -> programs -> turn Windows Features on or off. Go through the list, locate Internet Information Services and check the box and expand. Expand world wide web services -> Application Development Features -> check the CGI box. Collapse Application Development Features and Expand Common HTTP Features. Make sure all the boxes within it are checked. Go ahead and click on okay and wait for IIS to install successfully.
</p>
<br />

<p>
<img src="https://i.imgur.com/1y73WNS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Expand Internet Information Services -> Expand Web Management Tools -> Check the IIS Management Console box
</p>
<br />

<p>
<img src="https://i.imgur.com/EMdThcy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download PHP Manager For IIS (PHPManagerForIIS_V1.5.0.msi). Run the setup and click next through the installation process to install successfully.
</p>
<br />

<p>
<img src="https://i.imgur.com/Xfvu8qo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download Rewrite Module (rewrite_amd64_en-US.msi). Run the setup, agree to the license and click next through the installation process to install successfully.
</p>
<br />

<p>
<img src="https://i.imgur.com/L5y823a.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, open File Explorer and create a PHP directory in drive C. Simply create a new folder in drive C and rename it as PHP.
</p>
<br />

<p>
<img src="https://i.imgur.com/G8EJUxu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download PHP 7.3.8 and unzip the contents into C:\PHP
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
