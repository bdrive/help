
CONNECT
==================
Select SFTP in STORAGE TYPE and then click CONNECT.


<img class="markdown" src="https://doc.bdrive.com/images/sftp_config_1.jpg">


Type in SFTP User account and Password (if needed).

Uncheck "**Save user and password**" if you do not want to save FTP User account and Password. In this case you need to type these information each time you connect to the drive.

You can also use Private key to connect.  Click "BROWSE" to select private key file.  Putty format is not supported and openssh format is supported only.  If available, you need to insert passphrase in private key file.  You can set to save passphrase as well.


OPTIONS
==================


<img class="markdown" src="https://doc.bdrive.com/images/sftp_config_2.jpg">


* **Use server time for files/folders** : Use the time set of files/folders saved in the server instead of local PC timezone.

* **Use new file permission** : Set access permission to newly created files.

* **Use new folder permission** : Set access permission to newly created folders.

* **Mount Point**
    * **User home** : Connect to user home folder.
    * **System root** : Connect to system root of SFTP server.

* Max sessions : Max sessions : Limit the number of sessions. (NetDrive uses multiple simultaneous sessions to enhance performance when transferring data.)

* Bandwidth :  Control bandwidth settings.

