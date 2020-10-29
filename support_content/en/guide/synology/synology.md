### Connection Guide for NetDrive & Synology NAS WebDAV<br>

#### 1. Activating WebDAV in Synology NAS

It is required to install WebDAV in Synology NAS.  Go to Package Center and install WebDAV.
 
 ![Install WebDAV](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture1.png)<br><br>

#### 2. WebDAV Setup

Run WebDAV Server and check both Enable HTTP and Enable HTTPS.  Basically, Synology WebDAV uses port number 5005 for HTTP and 5006 for HTTPS.
 
 ![Setup WebDAV](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture2.png)<br><br>

#### 3. DDNS Setup

When connecting to Synology NAS through the internet, it is required to complete DDNS setup.  DDNS setup enables to access to Synology NAS through the internet.  (Omit DDNS setup of Synology NAS if already completed)
 
 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture3.png)<br><br>

#### 4. Connecting Synology NAS WebDAV and NetDrive<br><br>
##### Add a New Drive Item

Click “+” button near “Start here” and then add a new Drive Item.
 
 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture4.png)<br><br>

##### Select WebDAV STORAGE TYPE 

Select your WebDAV item from STORAGE TYPE list and then click “CONNECT”.
 
 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture5.png)<br><br>

##### Setup WebDAV Connection

Type in the URL and port number of your Synology WebDAV in Server field.  Check “Use SSL(https)” if you use HTTPS.  (By default, Synology NAS WebDAV uses port 5005 for HTTP and 5006 for HTTPS)
Type in User ID and Password in Account field.  (This Account requires the access permission to WebDAV)
 
 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture6.png)<br><br>

##### Default Setup on Drive Item

Default setup on Drive Item can be performed in Configure a Personal Drive page.  Refer to [the manual](https://www.netdrive.net/support/?type=documents&path=netdrive_manual&page=add-configure-drive) for detail information. 

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture7.png)<br><br>
 
##### Mount a Drive Item 

Click “CONNECT” button from WebDAV Drive Item and this will successfully mount WebDAV to the PC.

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture8.png)<br><br>
 
##### Check Mount Status

Using file explorer, check whether Synology NAS WebDAV is correctly mount or not.
 
 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture9.png)<br><br><br>
 
#### 5. Checklist for Synology NAS WebDAV Connection Issues<br><br>
##### Check Access Permission of WebDAV Server

“WebDAV server” permission can be set in “User” menu in Control Panel of Synology NAS DSM.

Go to “User” menu in Control Panel and select the user to connect to WebDAV, and then click “Edit”.

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture10.png)<br><br>
 
Go to “Applications” tab and select “Allow” in WebDAV Server field.

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture11.png)<br><br>

##### Check IP Block List in Synology NAS DSM 

Check whether user ID is registered in auto block list in Synology NAS DSM.  If user IP is included in the block list, remove the IP from the list.
 
 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture12.png)<br><br>

##### Check Port Number of Synology NAS WebDAV

Check whether the port number of Synology NAS WebDAV is correctly set in NetDrive Drive Item WebDAV.

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture13.png)<br><br>

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture14.png)<br><br>

##### Restart Synology NAS

Occasionally Synology NAS WebDAV application does not operate normally.  In this case, connection failure occurs when trying to access to WebDAV from the internet.  It is recommended to restart Synology NAS and then retry the connection.<br><br>

##### Check Router Setup

Router setup information seldomly changes after software update of the router.  If port forwarding option is used, it is necessary to check the port number.<br><br>


