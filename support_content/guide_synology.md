<h3>Connection Guide for NetDrive & Synology NAS WebDAV</h3>

<h4>1. Activating WebDAV in Synology NAS</h4>

<p>
It is required to install WebDAV in Synology NAS.  Go to Package Center and install WebDAV.
</p>
 

2	WebDAV Setup
Run WebDAV Server and check both Enable HTTP and Enable HTTPS.  Basically, Synology WebDAV uses port number 5005 for HTTP and 5006 for HTTPS.
 

3	DDNS Setup
When connecting to Synology NAS through the internet, it is required to complete DDNS setup.  DDNS setup enables to access to Synology NAS through the internet.  (Omit DDNS setup of Synology NAS if already completed)
 

4	Connecting Synology NAS WebDAV and NetDrive
4.1	Add a New Drive Item 
Click “+” button near “Start here” and then add a new Drive Item.
 
4.2	Select WebDAV STORAGE TYPE 
Select your WebDAV item from STORAGE TYPE list and then click “CONNECT”.
 

4.3	Setup WebDAV Connection
Type in the URL and port number of your Synology WebDAV in Server field.  Check “Use SSL(https)” if you use HTTPS.  (By default, Synology NAS WebDAV uses port 5005 for HTTP and 5006 for HTTPS)
Type in User ID and Password in Account field.  (This Account requires the access permission to WebDAV)
 

4.4	Default Setup on Drive Item
Default setup on Drive Item can be performed in Configure a Personal Drive page.  Refer to the manual for detail information. 
https://doc.bdrive.com/19-72-add-configure-drive.html 

 

4.5	Mount a Drive Item 
Click “CONNECT” button from WebDAV Drive Item and this will successfully mount WebDAV to the PC.

 

4.6	Check Mount Status
Using file explorer, check whether Synology NAS WebDAV is correctly mount or not.
 


 
Checklist for Synology NAS WebDAV Connection Issues

	Check Access Permission of WebDAV Server
	“WebDAV server” permission can be set in “User” menu in Control Panel of Synology NAS DSM.
Go to “User” menu in Control Panel and select the user to connect to WebDAV, and then click “Edit”.
 

Go to “Applications” tab and select “Allow” in WebDAV Server field.
 


	Check IP Block List in Synology NAS DSM 
	Check whether user ID is registered in auto block list in Synology NAS DSM.  If user IP is included in the block list, remove the IP from the list.
 


	Check Port Number of Synology NAS WebDAV
	Check whether the port number of Synology NAS WebDAV is correctly set in NetDrive Drive Item WebDAV.
 

 


	Restart Synology NAS
	Occasionally Synology NAS WebDAV application does not operate normally.  In this case, connection failure occurs when trying to access to WebDAV from the internet.  It is recommended to restart Synology NAS and then retry the connection.

	Check Router Setup
	Router setup information seldomly changes after software update of the router.  If port forwarding option is used, it is necessary to check the port number.


