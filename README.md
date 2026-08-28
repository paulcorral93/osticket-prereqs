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
 <img width="498" height="408" alt="image" src="https://github.com/user-attachments/assets/178dfe39-5c5e-4a88-ae66-d733ebaf7f1e" />

</p>
<p>
16. Click "Next".
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
 <img width="498" height="408" alt="image" src="https://github.com/user-attachments/assets/178dfe39-5c5e-4a88-ae66-d733ebaf7f1e" />

</p>
<p>
16. Click "Next".
</p> 
<br /> 

<p>
 <img width="498" height="408" alt="image" src="https://github.com/user-attachments/assets/178dfe39-5c5e-4a88-ae66-d733ebaf7f1e" />

</p>
<p>
16. Click "Next".
</p> 
<br /> 
