### Connection Guide for PLEX + NetDrive + Cloud Storage

#### 1. Select Cloud Storage

Select Cloud Storage supported by NetDrive and use as your Media Storage.

##### Cloud Storage list supported by NetDrive

1.	Google Drive/Shared Drive/Shared
2.	Dropbox
3.	Dropbox for Business
4.	OneDrive/Shared
5.	OneDrive for Business/Shared
6.	Box
7.	MEGA
8.	ucloud biz
9.	Yandex Disk
10.	Google Cloud Storage
11.	Amazon Web Service S3
12.	Azure Blob Storage
13.	Azure File Storage
14.	Swift
15.	Hubic
16.	Backblaze B2
17.	WebDAV (Web Distributed Authoring and Versioning)
18.	FTP/FTPS (File Transfer Protocol, FTP Secure)
19.	SFTP (SSH/Secure File Transfer Protocol)
20.	Wasabi
21.	filebase
22.	OpenStack
23.	4Shared
24.	CloudMe
 
 ![Supported Protocols](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/plex/Picture1.png)

* Google Drive set up configuration (This guide will explain with Google Drive sample case).

#### 2.	Get ready and configure the media resource

Configure folder structure and file name applying Plex naming rule.
 
 ![Media Resource](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/plex/Picture2.png)
 
##### Movie 

https://support.plex.tv/articles/naming-and-organizing-your-movie-media-files/

 ![Media Resource](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/plex/Picture3.png)

##### TV Show 

https://support.plex.tv/articles/naming-and-organizing-your-tv-show-files/

 ![Media Resource](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/plex/Picture4.png)

#### 3.	Connect NetDrive and Cloud Storage

In NetDrive app, create Drive Item which connects to Media Storage and then mount to the PC.

Use your own Google API key when using Google Drive. (Since NetDrive users basically use the same Google Drive API provided by NetDrive, it is recommended to register your own Google API key when high-speed streaming needed).   
How to create and register your own Google API Key   
https://support.bdrive.com/t/slow-google-drive-how-to-register-your-own-google-api-key/18503
 
 ![Connect Storage](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/plex/Picture5.png)

#### 4.	Install Plex Media Server

Join Plex in website and download/install Plex Media Server to your PC.   
https://www.plex.tv/media-server-downloads/   
Run Media Server and then go to “Add Library” to add Media Storage path which was mounted to your PC using NetDrive. 

 ![Setup Plex](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/plex/Picture6.png)
 
 ![Setup Plex](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/plex/Picture7.png)

* Router port forwarding needed when inaccessible on the internet.   
It can be proceeded by manually setting up the port number in “Remote Access” field of Plex Media Server and then typing in the port which was manually set up in router port forwarding.

 ![Setup Plex](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/plex/Picture8.png)

#### 5.	Run Media

Set up is completed.  Now select any media from Plex Client Software and run.   
From the following link, download which optimally fits to your device environment and then install.   
https://www.plex.tv/media-server-downloads/#plex-app
 
 ![Start Media](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/plex/Picture9.png)

Run Plex Client Software and login.  You can check the media file list in Library path.   
Select your favorite media and play.

