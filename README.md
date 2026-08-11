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
<img width="878" height="601" alt="Screenshot 2026-08-10 192316" src="https://github.com/user-attachments/assets/c28fefc8-b5b7-44d9-ae42-91003978eb41" />
</p>
<p>
Create a virtual machine in Azure running Windows 11. After the VM is created, grab the public or private IP address.    
</p>
<br />
<p>
<img width="400" height="234" alt="image" src="https://github.com/user-attachments/assets/39aced63-daa2-4fb7-9799-5f56b99ca7c9" />
</p>
<p>
Using Remote Desktop, log in to the Virtual Machine (VM) with the IP address and login credentials you used to create it. 
</p>
<br />

<p>
<img width="1116" height="593" alt="Screenshot 2026-08-10 193129" src="https://github.com/user-attachments/assets/538d0c0e-9ce1-4ca5-8eba-5056ec186e80" />
</p>
<p>
Inside the VM, bring up the Control Panel to enable/install IIS (Internet Information Services) with CGI.
</p>
<br />

<p>
<img width="796" height="851" alt="Screenshot 2026-08-10 193607" src="https://github.com/user-attachments/assets/c7a6a30a-5072-4973-83d5-dc2924bf7646" />
</p>
  >Open Control Panel >Add/uninstall Programs >Turn on/off Windows features >Check Internet Information Services >Expand Wide Web Services >Expand Application Development Features >Check CGI
</p>
<br />

<p>
<img width="490" height="530" alt="Screenshot 2026-08-10 194035" src="https://github.com/user-attachments/assets/4d57fb5e-46bd-480e-bd20-ddfd7caef071" />
</p>
<p>
<img width="410" height="510" alt="Screenshot 2026-08-10 194102" src="https://github.com/user-attachments/assets/8118a530-bd6e-44de-89aa-435aacb4be29" />
</p>
<p>
>Grab the installation files from https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD and unzip them onto the VM to begin installing the necessary files and programs for osTicket.
  Install PHP Manager (PHPManagerForIIS_V1.5.0.msi) 
  Install Rewrite Module (rewrite_amd64_en-US.msi) 
</p>
<p>
<img width="793" height="382" alt="image" src="https://github.com/user-attachments/assets/3288c8db-7c44-41a1-932a-e8eb00cf363a" />
</p> 
<p>
>Within File Explorer create the directory C:\PHP
</p> 
<p>
<img width="410" height="510" alt="Screenshot 2026-08-10 194102" src="https://github.com/user-attachments/assets/182807e5-2419-437d-b459-e56c99d3a212" />
</p>  
>Unzip php-7.3.8-nts-Win32-VC15-x86.zip into C:\PHP
 >install VC_redist.x86.exe 
</p>
<br />
<p>
<img width="379" height="295" alt="Screenshot 2026-08-10 195607" src="https://github.com/user-attachments/assets/6006438e-90b2-4a13-96e7-820b4d97e31a" />
</p>
<p>
>Install MySQL5.5.62 >Be sure to select "Typical Setup" when prompted >Launch the configuration wizard after the install and select "Standard Configuration" 
</p>
<br />

<p>
<img width="601" height="355" alt="Screenshot 2026-08-10 200321" src="https://github.com/user-attachments/assets/b5b7949b-7cee-4d57-acee-a9012beba830" />
</p>
<p>
  <img width="711" height="482" alt="Screenshot 2026-08-10 200844" src="https://github.com/user-attachments/assets/2a4823db-bb43-4c0f-858b-794839e05839" />
<img width="715" height="568" alt="Screenshot 2026-08-10 200911" src="https://github.com/user-attachments/assets/43c780fa-1879-467b-9ffe-babf71650212" />
<img width="680" height="363" alt="Screenshot 2026-08-10 200944" src="https://github.com/user-attachments/assets/cc83aba9-2d33-4779-931e-151a65486a00" />
<img width="714" height="571" alt="Screenshot 2026-08-10 201021" src="https://github.com/user-attachments/assets/0c1cd716-2982-484c-ab05-f13e55282932" />
</p> 
<p>
>Open IIS as an Admin >Register PHP from within IIS (PHP Manager.C:\PHP\php-cgi.exe) 
>Refresh IIS to update the changes
</p>
<br />

<p>
<img width="515" height="414" alt="Screenshot 2026-08-10 201311" src="https://github.com/user-attachments/assets/17be3534-0646-4ee5-a5fd-7fc3d2d84676" />
</p>
<p>
>unzip osTicket-v1.15.8.zip into C:\inetpub\wwwroot 
</p>
<br />

<p>
<img width="515" height="498" alt="Screenshot 2026-08-10 203520" src="https://github.com/user-attachments/assets/f05a1fc7-d75d-4523-ade5-53cceabde8be" />
<img width="509" height="499" alt="Screenshot 2026-08-10 203537" src="https://github.com/user-attachments/assets/e1b52d5d-12f6-4589-b104-17c44b0b5730" />
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
<img width="715" height="665" alt="Screenshot 2026-08-10 201436" src="https://github.com/user-attachments/assets/f4412011-ea85-464c-b5b9-544ea8a1b4c7" />
<img width="711" height="493" alt="Screenshot 2026-08-10 201526" src="https://github.com/user-attachments/assets/5a349e2f-87d1-42a1-8537-11203ba7095a" />
</p>
<p>
>Go back to IIS, sites -> Default -> osTicket >Double-click PHP Manager >Click “Enable or disable an extension” | Enable: php_imap.dll | Enable: php_intl.dll | Enable: php_opcache.dll 
>Refresh the osTicket site in your browser, observe the changes
</p>
<br />

<p>
<img width="537" height="491" alt="Screenshot 2026-08-10 201630" src="https://github.com/user-attachments/assets/d391c1ec-2be3-41cb-8960-c34f07c78071" />
<img width="524" height="423" alt="Screenshot 2026-08-10 201714" src="https://github.com/user-attachments/assets/40120583-e1a4-4515-9af0-7c175889809f" />
</p>
<p>
>Rename: ost-config.php
From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
To: C:\inetpub\wwwroot\osTicket\include\ost-config.php
</p>
<br />

<p>
<img width="282" height="388" alt="Screenshot 2026-08-10 201808" src="https://github.com/user-attachments/assets/9cc8d3b7-5eb1-4f75-ac30-71f0db1c5854" />
<img width="587" height="393" alt="Screenshot 2026-08-10 201827" src="https://github.com/user-attachments/assets/0ee26e93-14d0-4f59-9ead-0e8e746aedfd" />
<img width="394" height="211" alt="Screenshot 2026-08-10 201908" src="https://github.com/user-attachments/assets/20613aa4-d834-42ad-93cb-a9184e8c7a8f" />
<img width="590" height="396" alt="Screenshot 2026-08-10 201923" src="https://github.com/user-attachments/assets/cf49917d-a91e-4ce2-a141-9eb3b0788329" />
<img width="699" height="452" alt="Screenshot 2026-08-10 201934" src="https://github.com/user-attachments/assets/0a2a2085-0b5f-4f70-a4e4-9cc8ea2677d0" />
<img width="350" height="193" alt="Screenshot 2026-08-10 201946" src="https://github.com/user-attachments/assets/87ebe822-2f6d-4714-a00d-2be137abbb7b" />
<img width="700" height="454" alt="Screenshot 2026-08-10 202015" src="https://github.com/user-attachments/assets/932af81c-80c9-46c2-8d5f-e796cdad1196" />
</p>
<p>
>Assign Permissions: ost-config.php
  Disable inheritance -> Remove All
  New Permissions -> Everyone -> All
</p>
<br />

<p>
<img width="625" height="620" alt="Screenshot 2026-08-10 202131" src="https://github.com/user-attachments/assets/94cdb4bf-96db-4d23-ab46-3f853699b1e6" />
</p>
<p>
>Continue Setting up osTicket in the browser (click Continue)
  Name Helpdesk
  Default email (receives email from customers)
</p>
<br />

<p>
<img width="509" height="468" alt="Screenshot 2026-08-10 202211" src="https://github.com/user-attachments/assets/43d9a7ca-4f94-4ef2-80b2-52afac1dced8" />
<img width="523" height="353" alt="Screenshot 2026-08-10 202331" src="https://github.com/user-attachments/assets/8cca6f90-c5c5-4480-8ecc-c7f87c022c61" />
<img width="668" height="427" alt="Screenshot 2026-08-10 202358" src="https://github.com/user-attachments/assets/1d27e6cf-3c87-448f-97eb-29fa88c14044" />
<img width="657" height="385" alt="Screenshot 2026-08-10 202417" src="https://github.com/user-attachments/assets/b90a4489-43f3-476a-8e3d-9176e69a1b01" />

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
<img width="619" height="358" alt="Screenshot 2026-08-10 202452" src="https://github.com/user-attachments/assets/5fc3bf7b-38ce-4d6e-8797-011d1dcd784d" />
<img width="690" height="603" alt="Screenshot 2026-08-10 202557" src="https://github.com/user-attachments/assets/33fd5bbd-76fa-4a99-ab42-2ff76122ecb6" />

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
<img width="702" height="599" alt="Screenshot 2026-08-10 202641" src="https://github.com/user-attachments/assets/ca025b91-3b8e-4928-9439-a23f27f092c4" />
</p>
<p>
Browse the help desk login page: http://localhost/osTicket/scp/login.php
</p>
<br />

<p>
<img width="743" height="698" alt="Screenshot 2026-08-10 210649" src="https://github.com/user-attachments/assets/cf06cbf1-b236-4a6e-bd5d-b029e5752425" />
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
