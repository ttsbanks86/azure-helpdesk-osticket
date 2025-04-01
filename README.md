<p align="center">
  <img src="screenshots/10_osticket_logo.png" alt="OSTicket Logo" width="300"/>
</p>

# OSTicket Deployment Project (Azure VM)

This project documents the deployment of the open-source support ticket system OSTicket on a Windows 10 virtual machine in Microsoft Azure.

---

## Tools Used

- Microsoft Azure  
- Windows 10 (Azure VM)  
- IIS (Internet Information Services)  
- PHP  
- MySQL (XAMPP / HeidiSQL)  
- OSTicket v1.15.x  
- Remote Desktop (RDP)  

---

## Screenshots

### 1. Azure VM Created  
![Azure VM Created](screenshots/01_azure_vm_created.png)  
The Azure portal confirms that a Windows 10 VM has been successfully created. The public IP address is visible and will be used to connect remotely and access the OSTicket interface later.

### 2. RDP into Server  
![RDP Access](screenshots/02_rdp_into_server.png)  
RDP session confirms we have connected to the Azure VM. The same public IP appears at the top of the screen, matching the Azure configuration.

### 3. IIS Installed  
![IIS Installed](screenshots/03_iis_installed.png)  
The IIS Manager confirms that the web server role has been installed and is ready to host PHP-based applications like OSTicket.

### 4. PHP Info Page  
![PHP Info](screenshots/04_php_info_page.png)  
A PHP info page loaded through IIS confirms that PHP is installed and running on the web server.

### 5. MySQL Running in XAMPP  
![MySQL XAMPP](screenshots/05_mysql_xampp_running.png)  
XAMPP's MySQL service is running and verified through HeidiSQL. This will store OSTicket's data.

### 6. OSTicket Files Uploaded  
![OSTicket Files](screenshots/06_osticket_files_uploaded.png)  
The OSTicket application files are extracted into C:\inetpub\wwwroot\osticket, the default web root for IIS.

### 7. OSTicket Web Installer  
![Web Installer](screenshots/07_osticket_web_installer.png)  
The OSTicket installer is loaded in the browser from the VM's local web server, confirming that all dependencies (PHP, MySQL, IIS) are connected.

### 8. OSTicket Installation Successful  
![Installed Success](screenshots/08_osticket_installed_success.png)  
The system confirms OSTicket is installed. Final permissions and cleanup instructions are shown before admin login.

### 9. Ticket Demo (Optional)  
![Ticket Demo](screenshots/09_ticket_demo_optional.png)  
A sample ticket was created in the OSTicket dashboard, showing the system is fully operational and ready for use.

---

## Final Result

OSTicket is now fully deployed and accessible through a web browser using the VM's public IP. This proves the full installation and configuration of a help desk ticketing system on a cloud-hosted Windows environment.

---

## Credits

Built as part of the CourseCareers IT Helpdesk final project.
