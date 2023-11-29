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
- Download, install and configure HeidiSQL
- Continue setting up osTicket in the browser with HeidiSQL configuration credentials
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
<img src="https://i.imgur.com/vBX3hrg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download VC redist.x86.exe. Run the installation file and click next through the installation process to install successfully.
</p>
<br />

<p>
<img src="https://i.imgur.com/D8cdI6D.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download MySQL 5.5.62 (mysql-5.5.62-win32.msi) and install. Choose a typical setup and run the installation. Launch the Configuration wizard after installation is successful.
</p>
<br />

<p>
<img src="https://i.imgur.com/UnwpAfD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the configuration window, select standard configuration, click next, and check the 'install as Windows service' box.
</p>
<br />

<p>
<img src="https://i.imgur.com/bDoXCND.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create a new root password and continue to finish the configuration.
</p>
<br />

<p>
<img src="https://i.imgur.com/A2tMBpL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open IIS as an Administrator
</p>
<br />

<p>
<img src="https://i.imgur.com/k4BNVnj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Register PHP from within IIS. Open IIS and locate PHP Manager in the window. Click on it to open and click on 'Register new PHP version'. Reload IIS, Stop and start the server.
</p>
<br />

<p>
<img src="https://i.imgur.com/wDHFW72.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download osTicket v1.15.8. Open the folder and copy "upload" folder to C:\inetpub\wwwroot. Within C:\inetpub\wwwroot , rename "upload" to "osTicket"
</p>
<br />

<p>
<img src="https://i.imgur.com/DHfJIx6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open IIS, start and stop the server. Go to sites->Default->osTicket->click on "Browse*:80" 
</p>
<br />

<p>
<img src="https://i.imgur.com/Krdxtvo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Enable "php_imap.dll", "php_intl.dll", and "php_opcache.dll" extensions. GO back to IIS, sites->Default->osTicket->Double click on PHP Manager. Find the extension and click on enable 
</p>
<br />

<p>
<img src="https://i.imgur.com/ijDf6Ri.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Rename: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php to C:\inetpub\wwwroot\osTicket\include\ost-config.php
</p>
<br />

<p>
<img src="https://i.imgur.com/bugxOHJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Assign Permissions: locate ost-config.php (C:\inetpub\wwwroot\osTicket\include\ost-config.php). Right-click and click on properties->security->Advanced. click on disable all inheritance->remove all. Assign new permissions by clicking on New permission->Everyone->All
</p>
<br />

<p>
<img src="https://i.imgur.com/l4r3f3H.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Setup osTicket in the browser. Name the Helpdesk and provide all the required information
</p>
<br />

<p>
<img src="https://i.imgur.com/gv4UC2z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and install HeidiSQL. Open HeidiSQL and create a new session with username: root and password: Password1. Connect to the session.
</p>
<br />

<p>
<img src="https://i.imgur.com/TLz5u7d.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create a database called "osTicket".
</p>
<br />

<p>
<img src="https://i.imgur.com/ohcG66c.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
continue to setup osTicket in the browser. In the database section use these credentials MySQL Database: osTicket, MySQL Username: root, MySQL Password: Password1. Click “Install Now!”
</p>
<br />

<p>
<img src="https://i.imgur.com/1javyws.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Installation complete. Browse to your help desk login page: http://localhost/osTicket/scp/login.php
</p>
<br />
