 <p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
osTicket is a free, open-source customer support and helpdesk ticketing system for managing, tracking, and resolving inquiries from one central dashboard. Here are some easy-to-follow steps to install osTicket on a virtual machine.  <br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 11</b>

<h2>List of Prerequisites</h2>

- Azure Acccount/subscription 
- osTicket Installation

<h2>Installation Steps</h2>

<p>
<img width="1598" height="763" alt="image" src="https://github.com/user-attachments/assets/d3bec9f8-4c40-4bcd-ac59-a595efde72b4" />

</p>
<p>
1. Log in to Azure and create a virtual machine running Windows 11. If you need a guide on how to create a Virtual Machine, I created a guide for that as well; you can find it here: (https://github.com/paulcorral93/How-to-create-a-Virtual-Machine)
</p>
<br />

<p>
<img width="834" height="787" alt="image" src="https://github.com/user-attachments/assets/e46c4f77-8443-4d62-931a-5040a3d5637a" />

</p>
<p>
2. Once you have the Virtual Machine created, access it using Remote Desktop. Click the Start menu on your computer and search "Remote Desktop". Run Remote Desktop.
</p>
<br />

<p>
<img width="396" height="482" alt="image" src="https://github.com/user-attachments/assets/6210a35d-d5b6-445d-8ae9-c26513970093" />
 
</p>
<p>
3. At the bottom left corner of the window, make sure the "Show Options" is expanded so that you may enter the credentials to access your Virtual Machine. Once the Remote Desktop connects to the Virtual Machine, a window will pop up and ask you for the password.
</p>
<br />

<p>
<img width="381" height="392" alt="image" src="https://github.com/user-attachments/assets/11a4c809-93e7-4851-9125-9266e0766a8f" />
</p>
<p>
4. Click "Yes" to access your Virtual Machine.
</p>
<br />

<p>
 <img width="1567" height="799" alt="image" src="https://github.com/user-attachments/assets/9509bd31-79c6-4052-b3a6-b37b5dfa5c86" />

 https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD 
</p>
<p>
5. Copy the link above into a browser inside the Virtual Machine you created and download the ZIP file; it will have all the installation files you will need ahead.  
</p>
<br />

<p>
<img width="851" height="790" alt="image" src="https://github.com/user-attachments/assets/45e4972a-8edd-4326-b9e4-f368daa06358" />

</p>
<p>
6. Open the Start menu and search for "File Explorer". Once opened, expand the Downloads folder.
</p> 
<br /> 

<p>
<img width="1155" height="750" alt="image" src="https://github.com/user-attachments/assets/2ae3d42f-9c08-4de0-9458-6dde0e778c06" />

</p>
<p>
7. We are now going to extract the ZIP folder we downloaded to the desktop. this will make the installtion easier. Right click the ZIP file to bring up the small window and select "Extract All".
</p> 
<br /> 

<p>
<img width="1155" height="604" alt="image" src="https://github.com/user-attachments/assets/75ca882a-7d7a-42b4-82b7-7b0ea55f0ac3" />

</p>
<p>
8. Select the "Browse" box.   
</p> 
<br /> 

<p>
<img width="1167" height="636" alt="image" src="https://github.com/user-attachments/assets/43cca36f-5d94-4cc8-8250-8e8aa2b65591" />

</p>
<p>
9. Click Desktop on the left side of the window. Click on Select Folder to finalize 
</p> 
<br /> 

<p>
<img width="1198" height="630" alt="image" src="https://github.com/user-attachments/assets/2df19fd5-5b77-4670-ad06-9f7a8951b809" />

</p>
<p>
10. The files Should now be on your desktop of the Virtual Machine.
</p> 

<p>
<img width="1089" height="691" alt="image" src="https://github.com/user-attachments/assets/2e76ac38-e869-489d-8e60-ee4a1e3ac58a" />

</p>
<p>
11. Next we will install/enable IIS (Internet Information Services) on Windows with CGI on the Virtual Machine. Open the Start menu and search for the "control Panel" and run the program.
</p> 
<br /> 

<p>
<img width="1298" height="694" alt="image" src="https://github.com/user-attachments/assets/4f2373c8-c09f-4a46-9d17-11d8bb59e2d6" />

</p>
<p>
12. CLick on "Programs" tab.
</p> 
<br /> 

<p>
<img width="1253" height="619" alt="image" src="https://github.com/user-attachments/assets/371343bf-ea6c-4b06-8d8c-8d0ab8050b65" />

</p>
<p>
13. Click on "Turn Windows features on/off"
</p> 
<br /> 

<p>
<img width="1288" height="741" alt="image" src="https://github.com/user-attachments/assets/317d093c-51ef-4018-a17d-9acb11d5f175" />
 
</p>
<p>
14. Make sure the boxes for the following are selected: Select Internet Information Services, Expand Internet Information Services, Expand World Wide Web Services, Expand Application Developement Features, Select CGI. Click "Ok"
</p> 
<br /> 

<p>
<img width="1130" height="599" alt="image" src="https://github.com/user-attachments/assets/067a9ecf-12b0-458d-9812-48e52200ae5e" />
 
</p>
<p>
15. From your Virtual Machine, open the install files that were unzipped to the desktop earlier. The first installation we will run is the PHP Manager for IIS. (PHPManagerForIIS_V1.5.0.msi)
</p> 
<br /> 

<p>
 <img width="498" height="408" alt="image" src="https://github.com/user-attachments/assets/178dfe39-5c5e-4a88-ae66-d733ebaf7f1e" />

</p>
<p>
16. Click "Next".
</p> 
<br /> 

<p>
<img width="503" height="413" alt="image" src="https://github.com/user-attachments/assets/5d447561-d62a-4394-8046-68ddec1c30d8" />

</p>
<p>
17. Click "I Agree" then "Next"
</p> 
<br /> 

<p>
<img width="588" height="546" alt="image" src="https://github.com/user-attachments/assets/0e292da9-3f26-47db-b28e-6cfc59ee73c0" />

</p>
<p>
18. Click "yes".
</p> 
<br /> 

<p>
<img width="522" height="414" alt="image" src="https://github.com/user-attachments/assets/6130874a-eb9d-449e-b79d-597192cb1d2b" />

</p>
<p>
19. Close the window; the installation is done.
</p> 
<br /> 

<p>
<img width="1146" height="604" alt="image" src="https://github.com/user-attachments/assets/85beb19d-ea78-41ed-85e8-32c2502c39ae" />

</p>
<p>
20. Now we will install the Rewrite Module (rewrite_amd64_en-US.msi)
</p> 
<br /> 

<p>
<img width="627" height="434" alt="image" src="https://github.com/user-attachments/assets/eaf9a580-1785-4db1-9bfd-201eaf4980e9" />

</p>
<p>
21. Click " I accept the terms and conditions" and "Install" to begin the installation. 
</p> 
<br /> 

<p>
<img width="496" height="439" alt="image" src="https://github.com/user-attachments/assets/123bef27-f0ce-4182-ac1e-cdb52b063848" />

</p>
<p>
22. Click "yes".
</p> 
<br /> 

<p>
<img width="1207" height="643" alt="image" src="https://github.com/user-attachments/assets/f1a90acc-f1ad-4877-a797-f23e5cb079eb" />

</p>
<p>
23. Open "File Explorer" again; this time, we will create a new Directory in (C:). You can find it on the right side of the window under the "This PC" tab
</p> 
<br /> 

<p>
<img width="1151" height="594" alt="image" src="https://github.com/user-attachments/assets/6b9df21e-e993-421f-922e-7169a395e460" />
<img width="1141" height="608" alt="image" src="https://github.com/user-attachments/assets/abc9da1b-db37-4c3d-999c-977ebf676a47" />

</p>
<p>
24. Right-click in the window to create a new folder, name it "PHP".
</p> 
<br /> 

<p>
<img width="1217" height="703" alt="image" src="https://github.com/user-attachments/assets/ea93d29a-0dd6-4468-bb74-b8af2115869c" />

</p>
<p>
25. From the “osTicket-Installation-Files” folder in the Virtual Machine. 
</p> 
<br /> 

<p>
<img width="1204" height="649" alt="image" src="https://github.com/user-attachments/assets/3a71fbf7-18f9-4076-ac67-90bfc9271f73" />

</p>
<p>
26. Unzip PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) into the “C:\PHP” folder</p> 
<br /> 

<p>
<img width="1137" height="625" alt="image" src="https://github.com/user-attachments/assets/39b39b1c-8294-462a-b65b-176e335380ea" />

</p>
<p>
27. From the “osTicket-Installation-Files” folder, install VC_redist.x86.exe.
<br /> 

<p>
<img width="500" height="317" alt="image" src="https://github.com/user-attachments/assets/88ed1dea-9e9a-4e79-91d8-2640a767614b" />

</p>
<p>
28. Click "I Agree" and "Install". 
</p> 
<br /> 

<p>
<img width="486" height="417" alt="image" src="https://github.com/user-attachments/assets/645bd27a-e97f-49aa-a8ba-2231e07eca71" />

</p>
<p>
29. Click "Yes."  
</p> 
<br /> 

<p>
<img width="1152" height="616" alt="image" src="https://github.com/user-attachments/assets/2729d788-4dba-442f-8895-f1047ed7b2d8" />

</p>
<p>
30. From the “osTicket-Installation-Files” folder we have been using, click to install MySQL 5.5.62 (mysql-5.5.62-win32.msi)
</p> 
<br /> 

<p>
<img width="526" height="406" alt="image" src="https://github.com/user-attachments/assets/aaf09a69-df6d-4dcb-9725-0b44695d1570" />

</p>
<p>
31. Click "Next". 
</p> 
<br /> 

<p>
<img width="510" height="390" alt="image" src="https://github.com/user-attachments/assets/df433602-c898-4c45-b770-f2e7fe2b4ad1" />

</p>
<p>
32. Click "I Agree" and "Next". 
</p> 
<br /> 

<p>
<img width="1152" height="596" alt="image" src="https://github.com/user-attachments/assets/483199e0-2784-436c-aec9-3e5643a3dac2" />

</p>
<p>
33. Select "Typical Setup"
</p> 
<br /> 

<p>
<img width="608" height="427" alt="image" src="https://github.com/user-attachments/assets/efa46e72-fd7d-4a2d-bf36-a3a38e3ad1fa" />

</p>
<p>
34. Click "Install".
</p> 
<br /> 

<p>
<img width="476" height="409" alt="image" src="https://github.com/user-attachments/assets/97572a96-412b-471d-baa1-f8cfca1d404d" />

</p>
<p>
35. Click "Yes". 
</p> 
<br /> 

<p>
<img width="645" height="464" alt="image" src="https://github.com/user-attachments/assets/51b77b2f-0b50-478a-a745-f3bc0cba7e90" />

</p>
<p>
25. Click Finish, but make sure the box for "launch SQL instance configuration wizard" is checked.
</p> 
<br /> 

<p>
<img width="497" height="457" alt="image" src="https://github.com/user-attachments/assets/cedb819b-5340-4126-a3a7-f77ba8decd83" />

</p>
<p>
25. Click Yes.
</p> 
<br /> 

<p>
<img width="525" height="385" alt="image" src="https://github.com/user-attachments/assets/8cc9bcaf-d594-4c37-98c7-5f185c9c7325" />

</p>
<p>
25. After the configuration window opens, click "Next".
</p> 
<br /> 

<p>
<img width="517" height="397" alt="image" src="https://github.com/user-attachments/assets/058e7f92-b8f9-4240-a982-a9a9fcc37f4f" />

</p>
<p>
25. Select "Standard Configuration"
</p> 
<br /> 

<p>
<img width="525" height="389" alt="image" src="https://github.com/user-attachments/assets/084445a5-b4f6-4dac-bb45-8a9eafd9ce5a" />

</p>
<p>
25. Click "Next".
</p> 
<br /> 

<p>
<img width="502" height="385" alt="image" src="https://github.com/user-attachments/assets/60d26281-cd22-4b83-b2be-a9ee6abdee4a" />

</p>
<p>
25. Make sure to put in "root" for the password and then click "Next".
</p> 
<br /> 

<p>
<img width="515" height="395" alt="image" src="https://github.com/user-attachments/assets/c5fdeeb8-2cc7-49c2-b454-cca885ea7613" />

</p>
<p>
25. Click "Execute"
</p> 
<br /> 

<p>
<img width="895" height="707" alt="image" src="https://github.com/user-attachments/assets/7331a0de-bd99-48f6-8112-93c3031891b8" />

</p>
<p>
25. Click Start Menu and search for "IIS"; this time, we will open it as Administrator.
</p> 
<br /> 

<p>
<img width="1302" height="660" alt="image" src="https://github.com/user-attachments/assets/904ff81c-bcf3-47b0-8d20-ab66f05eb14a" />

</p>
<p>
25. Now register PHP from within IIS. To do this, begin by clicking PHP Manager in IIS. (installed this earlier)  
</p> 
<br /> 

<p>
<img width="1195" height="623" alt="image" src="https://github.com/user-attachments/assets/e5b71a4e-070f-40fb-bc3d-c1f8e35e3612" />

</p>
<p>
25. Click "Register new PHP version"
</p> 
<br /> 

<p>
<img width="1031" height="548" alt="image" src="https://github.com/user-attachments/assets/ae4351ec-a8f1-472e-b1c5-aba81bf4b5b5" />

</p>
<p>
25. Click the "..." box to select the right file from the PHP folder located at C:\. 
</p> 
<br /> 

<p>
<img width="1083" height="585" alt="image" src="https://github.com/user-attachments/assets/9e0e4b2a-5388-4911-80d1-9a1821ea5bf2" />

</p>
<p>
25. Click "C:\PHP\php-cgi.exe"
</p> 
<br /> 


<p>
<img width="1200" height="624" alt="image" src="https://github.com/user-attachments/assets/d31765a6-aed1-4a78-bc28-0208c02d8787" />

</p>
<p>
25. Head back to the IIS homepage and on the right side of the window, select "Restart" to apply the changes just made.
</p> 
<br /> 

<p>
<img width="1143" height="609" alt="image" src="https://github.com/user-attachments/assets/592c48b6-fee8-4aa3-a4cb-7c66b1ff51e7" />

</p>
<p>
25. Open up osTicket-Installation-Files located on the desktop of the Virtual Machine. Within “c:\inetpub\wwwroot”.
</p> 
<br /> 

<p>
<img width="1187" height="637" alt="image" src="https://github.com/user-attachments/assets/e97a2927-30ea-4e94-bd19-49a47212e136" />

</p>
<p>
25.  Extract “osTicket-v1.15.8.zip” into “c:\inetpub\wwwroot”.
</p> 
<br /> 

<p>
<img width="1141" height="603" alt="image" src="https://github.com/user-attachments/assets/e79d2ce9-8805-4c64-825b-2e1c5524c06f" />

</p>
<p>
25.   Inside “c:\inetpub\wwwroot” rename “upload” to “osTicket”
 
</p> 
<br /> 

<p>
<img width="1201" height="619" alt="image" src="https://github.com/user-attachments/assets/868ccd5b-1a9f-4360-90bf-24a89cd878fa" />

</p>
<p>
25.  Go back to IIS and restart the program after the files are finished extracting.
</p> 
<br /> 

<p>
<img width="1213" height="641" alt="image" src="https://github.com/user-attachments/assets/7e65663f-74e0-4ab7-a367-f5ca0a574e65" />

</p>
<p>
25. From the IIS home window, expand the Sites tab, then expand Default Web Site, click on the osTicket folder

</p> 
<br /> 

<p>
<img width="1222" height="649" alt="image" src="https://github.com/user-attachments/assets/ea72d29b-d2b9-4a29-af23-cc0a0a16e5d7" />

</p>
<p>
25.  On the right, click “Browse *:80”
</p> 
<br /> 

<p>
<img width="1059" height="790" alt="image" src="https://github.com/user-attachments/assets/5933e46a-a85b-43dc-9791-35b19d793bd7" />

</p>
<p>
25.  This should open osTicket in your browser.
</p> 
<br /> 

<p>
<img width="1201" height="624" alt="image" src="https://github.com/user-attachments/assets/daf23c73-61a0-42b1-8a45-321c6ec0d27a" />

</p>
<p>
25.  Go back to the IIS home page, expand sites, expand Default, click the osTicket folder

</p> 
<br /> 


<p>
<img width="1201" height="626" alt="image" src="https://github.com/user-attachments/assets/91ad78bf-6424-4d84-a53f-e390ab75d747" />

</p>
<p>
25. Click PHP Manager 

</p> 
<br /> 

<p>
<img width="1207" height="625" alt="image" src="https://github.com/user-attachments/assets/da19e191-b598-40c0-b8b5-c3814feaae47" />

</p>
<p>
25.  Under PHP Extensions, click “Enable or disable an extension”

</p> 
<br /> 

<p>
<img width="1197" height="625" alt="image" src="https://github.com/user-attachments/assets/17d962b4-ff41-4251-a605-6a7ea1422ca4" />

</p>
<p>
25.  Click php_imap.dll; on the right side of the window, click Enable 


</p> 
<br /> 

<p>
<img width="1206" height="634" alt="image" src="https://github.com/user-attachments/assets/79a5ff91-f9aa-448c-902e-3b5f1efa2674" />

</p>
<p>
25. Click php_intl.dll; on the right side of the window, click Enable 


</p> 
<br /> 


<p>
<img width="1205" height="637" alt="image" src="https://github.com/user-attachments/assets/9871a6ed-30fe-4721-af46-49b5a5d57b0d" />

</p>
<p>
25.  Click php_opcache.dll; on the right side of the window, click Enable

</p> 
<br /> 


<p>
<img width="1204" height="621" alt="image" src="https://github.com/user-attachments/assets/257b6ce3-2103-49c5-bc5e-b396718e7c66" />

</p>
<p>
25. Refresh IIS for the home window 

</p> 
<br /> 


<p>
<img width="1051" height="789" alt="image" src="https://github.com/user-attachments/assets/0b9eeb49-9b3d-4d64-8d71-974a86c53161" />
<img width="1059" height="787" alt="image" src="https://github.com/user-attachments/assets/ca2067d7-45d7-433d-82a1-d19e6a476196" />

</p>
<p>
25.  Refresh the osTicket site in your browser, and observe the changes
 
</p> 
<br /> 

<p>
<img width="1168" height="631" alt="image" src="https://github.com/user-attachments/assets/737f718a-3116-485d-8ea6-a8b3782ef25f" />

</p>
<p>
25. Using File Explorer, open the inetpub folder in Windows (C:)

</p> 
<br /> 
<p>
<img width="1140" height="609" alt="image" src="https://github.com/user-attachments/assets/52775ca5-07bf-491f-836a-b2bf65275a1a" />

</p>
<p>
25.  Open the wwwroot folder


</p> 
<br /> 

<p>
<img width="1169" height="616" alt="image" src="https://github.com/user-attachments/assets/b9de8a62-2c25-4091-a1de-085062c54e92" />

</p>
<p>
25. Open the osTicket Folder.

</p> 
<br /> 

<p>
<img width="1171" height="605" alt="image" src="https://github.com/user-attachments/assets/5fb22ae0-bbbf-41ff-b620-ffc078e2978e" />

</p>
<p>
25. Open the include folder 

</p> 
<br /> 

<p>
<img width="1161" height="597" alt="image" src="https://github.com/user-attachments/assets/b4743b39-f367-4560-bf34-1bfe6be54a2b" />
<img width="1147" height="610" alt="image" src="https://github.com/user-attachments/assets/97d4abbf-487f-4e3f-a1a9-0245d0d4d3c3" />

</p>
<p>
25. Rename the "ost-sampleconfig.php" file to "ost-config.php"

</p> 
<br /> 

<p>
<img width="1204" height="621" alt="image" src="https://github.com/user-attachments/assets/257b6ce3-2103-49c5-bc5e-b396718e7c66" />

</p>
<p>
25. Refresh IIS for the home window 

</p> 
<br /> 
