### Checklist for Synology NAS WebDAV Connection Issues

#### Check Access Permission of WebDAV Server
“WebDAV server” permission can be set in “User” menu in Control Panel of Synology NAS DSM.

Go to “User” menu in Control Panel and select the user to connect to WebDAV, and then click “Edit”.

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/troubleshooting/synology/Picture1.png)
Go to “Applications” tab and select “Allow” in WebDAV Server field.

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/troubleshooting/synology/Picture2.png)
#### Check IP Block List in Synology NAS DSM 

Check whether user ID is registered in auto block list in Synology NAS DSM.  If user IP is included in the block list, remove the IP from the list.
 
 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/troubleshooting/synology/Picture3.png)

#### Check Port Number of Synology NAS WebDAV

Check whether the port number of Synology NAS WebDAV is correctly set in NetDrive Drive Item WebDAV.

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/troubleshooting/synology/Picture4.png)

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/troubleshooting/synology/Picture5.png)

#### Check Router Setup

Router setup information seldomly changes after software update of the router.  If port forwarding option is used, it is necessary to check the port number.

#### Restart Synology NAS

Occasionally Synology NAS WebDAV application does not operate normally.  In this case, connection failure occurs when trying to access to WebDAV from the internet.  It is recommended to restart Synology NAS and then retry the connection.

