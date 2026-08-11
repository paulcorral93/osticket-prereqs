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

- Windows 11</b>

<h2>List of Prerequisites</h2>

- Azure subscription 
- osTicket Installation

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create a virtual machine in Azure running Windows 11.    
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Using Remote Desktop, log into the Virtual Machine (VM) to begin. 
Inside the VM, bring up the Control Panel to enable/install IIS (Internet Information Services) with CGI ().
  -Open Control Panel >Add/uninstall Programs >Turn on/off Windows features >Check Internet Information Services >Expand World Web Services >Expand Application Development Features >Check CGI
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
>Grab the installation files from https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD and unzip them onto the VM to begin installing the necessary files and programs for osTicket.
  Install PHP Manager (PHPManagerForIIS_V1.5.0.msi) 
  Install Rewrite Module (rewrite_amd64_en-US.msi) 
>Within File Explorer create the directory C:\PHP 
>Unzip php-7.3.8-nts-Win32-VC15-x86.zip into C:\PHP >install VC_redist.x86.exe 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
>Install MySQL5.5.62 >Be sure to select "Typical Setup" when prompted >Launch the configuration wizard after the install ans select "Standard Configuration" 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
>Open IIS as an Admin >Register PHP from within IIS (PHP Manager.C:\PHP\php-cgi.exe) 
>Refresh IIS to update the changes
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
>unzip osTicket-v1.15.8.zip into C:\inetpub\wwwroot 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
>Within C:\inetpub\wwwroot Rename upload to "osTicket" >Refresh IIS to update the changes 
</p>
<br />

<p>
<img width="712" height="501" alt="Screenshot 2026-08-10 191848" src="https://github.com/user-attachments/assets/acac0ed1-a161-4133-bbb4-a807cd789f97" />
</p>
<p>
>Within IIS expand Sites, expand Default, click osTicket on the right side of the window click Browse *:80 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
>Go back to IIS, sites -> Default -> osTicket >Double-click PHP Manager >Click “Enable or disable an extension” | Enable: php_imap.dll | Enable: php_intl.dll | Enable: php_opcache.dll 
>Refresh the osTicket site in your browser, observe the changes
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
>Rename: ost-config.php
From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
To: C:\inetpub\wwwroot\osTicket\include\ost-config.php
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
>Assign Permissions: ost-config.php
  Disable inheritance -> Remove All
  New Permissions -> Everyone -> All
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
>Continue Setting up osTicket in the browser (click Continue)
  Name Helpdesk
  Default email (receives email from customers)
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
>From the “osTicket-Installation-Files” folder, install HeidiSQL.
Open Heidi SQL
Create a new session, root/root
Connect to the session
Create a database called “osTicket”
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
>Continue Setting up osTicket in the browser
  MySQL Database: osTicket
  MySQL Username: root
  MySQL Password: root
Click “Install Now!”
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Browse the help desk login page: http://localhost/osTicket/scp/login.php
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
End Users osTicket URL:
http://localhost/osTicket/ 

</p>
<br />
<p>
   
</p>
<p>

</p>
