<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This project outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Connection
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Create a Virtual Machine in Azure
    - OS: Windows 10
    - Name: osticket-vm
    - Username: claborde-osticket
    - Password: Password123!
- Log into the VM with Remote Desktop Connect
- Download the [osTicket-Installation-Files.zip](https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD) and unzip it onto the Desktop
- Install/Enable IIS in Windows with CGI
    - World Wide Web Services ---> Application Development Features ---> CGI

<br />

<h1>Installation Steps</h1>

## Installing the dependencies
### From the `osTicket-Installation-Files` folder, install PHP Manager for IIS
<p>
<img src="https://github.com/user-attachments/assets/fbdebff9-d15a-4d82-9435-51952cb6f741" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/cc5415ae-a939-41c5-a86b-4b6a14787924" height="80%" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### From the `osTicket-Installation-Files` folder, install the Rewrite Module
<p>
<img src="https://github.com/user-attachments/assets/0a50462c-a127-4d9b-a7e1-6fffc45b6ea5" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/cf54af58-deec-4445-8e58-8c2bbbdae509" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Create a directory in the C drive called `PHP`, then unzip the `PHP 7.3.8` from the `osTicket-Installation-Files` folder
<p>
<img src="https://github.com/user-attachments/assets/9041149d-6909-4fc1-bd48-36581eefabdc" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/50960973-de1e-4c42-938f-e585926b248e" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/71aa4757-fc41-4a06-b564-c2c9a9962f06" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/217d0a61-c983-4e8c-af7c-19ff098a493d" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### From the `osTicket-Installation-Files` folder, install the Microsoft Visual C++ 2015-2022 Redistributable executable file
<p>
<img src="https://github.com/user-attachments/assets/cdc4df73-302e-43d4-8bca-cf02b203a029" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/8fa29612-3083-4008-b288-0c3224699cc7" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### From the `osTicket-Installation-Files` folder, install the MySQL server
<p>
<img src="https://github.com/user-attachments/assets/9517972f-7795-4835-b84f-fc07d73ed47e" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/a1cbdd14-e178-492d-b14b-bee3792b2302" width="500" alt="Disk Sanitization Steps"/>
</p>

### Set the MysQL Instance to Standard
<p>
<img src="https://github.com/user-attachments/assets/73760383-d570-4fd5-bba2-d8281974d9a7" width="500" alt="Disk Sanitization Steps"/>
</p>

### Install the following as a Windows Service
<p>
<img src="https://github.com/user-attachments/assets/f1fc6751-f388-4ab8-8022-afd65d1dee4a" width="500" alt="Disk Sanitization Steps"/>
</p>

### Set the password to `root`
<p>
<img src="https://github.com/user-attachments/assets/efe6e911-3ba1-40c8-8af4-f2030470e32c" width="500" alt="Disk Sanitization Steps"/>
</p>

### Click execute to allow the windows machine to execute the following steps then click finish
<p>
<img src="https://github.com/user-attachments/assets/86a81870-e5b3-48d2-bed7-80d262752d7d" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />


## Configuring IIS
### Open IIS as an admin
<p>
<img src="https://github.com/user-attachments/assets/de6fab47-2bd1-4e10-aacf-61aeac76b8fe" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Register PHP from within IIS
<p>
<img src="https://github.com/user-attachments/assets/31d07241-6183-4fbb-9698-f3ea1300d606" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/30c6581d-c763-42b9-944d-bad7f1d2f437" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/51f25505-86d7-45c3-ad95-769dc4c06db1" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/5d373aa2-d2c3-4bd8-b251-c1fb0940c88e" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />


## Installing osTicket
### From the `osTicket-Installation-Files` folder, unzip the `osTicket-v1.15.8.zip` file and copy the "upload" folder into `C:\inetpub\wwwroot` directory
<p>
<img src="https://github.com/user-attachments/assets/97526b21-bca6-4945-8585-d6bb0e2f8a77" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/c0461e8a-8c3a-47fd-812c-277ea40ac13f" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/49481ea0-e082-4ec1-9723-ba5846ca75ce" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/80ec812b-121d-42ad-b2b0-6cc0c766e2d7" width="500" alt="Disk Sanitization Steps"/>
</p>

### Within the `C:\inetpub\wwwroot` directory, rename the folder "upload" to "osTicket"
<p>
<img src="https://github.com/user-attachments/assets/0bceb21c-6a25-42a5-9081-5a5c9cb94f8e" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/4fd51b82-e71f-40e8-9362-1278846ae052" width="500" alt="Disk Sanitization Steps"/>
</p>

### Reload the IIS server
<p>
<img src="https://github.com/user-attachments/assets/f561a108-c7c8-4d15-a8a9-d75c0ed5c8fe" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/e38c9098-6567-4691-8329-960276470a13" width="500" alt="Disk Sanitization Steps"/>
<br />

### The osTicket website should now be available
<p>
<img src="https://github.com/user-attachments/assets/e78ae976-aa55-4e37-a00f-379c20aaa42d" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />


## Configuring osTicket
### Go to Sites --> Default --> osTicket and on the right of the application, click `Browse *:80`
<p>
<img src="https://github.com/user-attachments/assets/66972603-cb48-4515-9d3d-1110d94f8fe0" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/a6396dea-de42-4ad2-a7c1-943d189378dc" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Enable extensions `php_imap.dll`, `php_intl.dll` and `php_imap.dll`
<p>
<img src="https://github.com/user-attachments/assets/f08198a8-d561-4acb-928f-be266fb65491" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/e5c94fdb-4c5f-4ee3-a6ad-a925234b0fe1" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/e5c94fdb-4c5f-4ee3-a6ad-a925234b0fe1" width="500" alt="Disk Sanitization Steps"/>
</p>

### php_imap.dll
<p>
<img src="https://github.com/user-attachments/assets/41757042-24f8-4145-8866-c7774d0491a1" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/8fc9145d-73ca-476d-b5de-164b29b1fd46" width="500" alt="Disk Sanitization Steps"/>
</p>

### php_intl.dll
<p>
<img src="https://github.com/user-attachments/assets/c0071632-b4ea-493d-91db-86cbb2bf88c8" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/e53fd626-b5fc-4451-a9b1-6e85035530e8" width="500" alt="Disk Sanitization Steps"/>
</p>

### php_imap.dll
<p>
<img src="https://github.com/user-attachments/assets/a6719c54-efe1-45c3-aee0-bb647f7612cc" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/a9986aad-a853-42ea-8adb-4112056ad3ce" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### All of the required extensions should now have a green check mark next to them
<p>
<img src="https://github.com/user-attachments/assets/55418420-69e3-404a-91c0-cfffeac90b67" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Renaming the osTicket sample configuration file
<p>
<img src="https://github.com/user-attachments/assets/b4f9ab81-2735-48d0-8315-3c043c07df43" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/d199752a-37cd-40f1-8d30-dc2487bef87d" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Assigning Permissions for the osTicker configuration file
<p>
<img src="https://github.com/user-attachments/assets/fc75186e-28b0-4592-8def-7190e2521588" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/aec3f72a-9342-4457-8423-45834405b924" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/42f3ae63-4089-4541-9b6d-91631b73c05c" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/42f3ae63-4089-4541-9b6d-91631b73c05c" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />




