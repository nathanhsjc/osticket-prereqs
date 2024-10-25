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

- Enable Internet Information Services (IIS)
- Install Webplatform Installer
- Install MySQL
- Install C++ Redistributable 
- Configure permissions and install osTicket

<h2>Installation Steps</h2>

![image](https://github.com/user-attachments/assets/52629115-1e11-42c5-ba4d-3e3cb5221c1e)

<p>

</p>
<p>
After creating your virtual machine in Azure, you will log into your virtual machine to get the process of os-Ticket installed. Once in the virtual machine (VM), you will need to enable to enable Internet Information Services (IIS). To do this you will want to unzip and extract the folder os-ticket installation folder onto your desktop. 
</p>
<br />

![image](https://github.com/user-attachments/assets/534f1ed0-5008-41b7-950b-dbd26da1f964)

<p>

</p>
<p>
In this next step proceed to Control Panels then navigate to Programs. Click turn windows feature on or off and then check the IIS box and enable CGI (dependency aapart of the osTicket webserver). To find CGI - expand World Wide Web Services - Expand Application development features and then click on the CGI box.
</p>
<br />

![image](https://github.com/user-attachments/assets/b3449818-f76e-440d-ad19-2fcd4028981d)

<p>

</p>
<p>
We are now at the step to open open the osTicket installation folder. Open up the osTicket installation folder and install PHP Manager and Rewriteamd64. Then proceed to createa a PHP folder on the C drive. 
Open up IIS from the start menu and click "run as administrator". Proceed to click on PHP Manager and then click on the link "Register a new PHP". From there you will go into the PHP folder you created and extract php-cgi onto IIS. Afterwards you will navigate to connections on the left where the name of the server is. You will proceed to click stop on the server and then start for it to load with the new content.

Go back to os-Ticket-Installation-Files and unzip osTicket-v1.15.8.zip and proceed to copy the "upload" folder into “c:\inetpub\wwwroot”. In c:\inetpub\wwwroot rename upload to osTicket. After this step click stop wait a few minutes and click start. This will reload the server. Proceed to sites - default - osTicket and click browse *80.




</p>
<br />

![image](https://github.com/user-attachments/assets/de3f6589-3bd0-412f-bfe5-459925e61283)

<p>
Navigate back to osTicket in IIS and click on PHP manager. Scroll down and click enable or disable an extension to start enabling the extensions for osTicket. 
enable: php_imap.dll, enable: php_intl.dll, enable: php_opcache.dll, and then refresh the osTicket site in your browser, observe the changes then go back to the osTicket site and refresh it. Proceed back into the inetpub > wwwroot > osTicket > folder and scroll down to the ost-sample.php and rename it to ost-config.php. Next will be to configure the permissions. 

To configure permissions, right click properties, click security, edit and then type in the names of those who you want to give permissions to then click apply > ok.
</p>


<p>
.
</p>
<br />

![image](https://github.com/user-attachments/assets/06135798-cbfb-4c69-98c6-ca7c81b128a7)

<p>
Proceed back into the osTicket installation folder onto the desktop. Click on HeidiSQL to install the database. From HeidiSQL you will be able to create the osTicket database. After this step has been completed proceed back into the osTicket installer and enter in your database information for the completion of the installation of osTicket
</p>


<p>

</p>
<br />

![image](https://github.com/user-attachments/assets/4ad5eb38-b82f-4092-b8c1-db2b670934f5)

<p>

</p>


<p>
Congratulations. All the steps have been achieved and now you are able to use the osTicket software.
</p>
<br />
