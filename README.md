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

<h2>Installation Steps</h2>

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
<br />

