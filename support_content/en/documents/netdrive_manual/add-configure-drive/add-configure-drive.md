### Add and Configure Drives

Click "+" button at lower right side to add drive items. You can also change drive configuration of each added drive item by clicking "CONFIG".

<img class="markdown" src="https://doc.bdrive.com/images/add_configure_drive_1.jpg">

- Select remote storage type from STORAGE TYPE field and then click "CONNECT" to authenticate remote storage.
  Available drive item types are as below.

  - [Backblaze B2](/support/?type=documents&path=netdrive_manual/add-configure-drive&page=backblaze-b2-config)
  - [Box](/support/?type=documents&path=netdrive_manual/add-configure-drive&page=box-config)
  - [Dropbox](/support/?type=documents&path=netdrive_manual/add-configure-drive&page=dropbox-config)
  - [FTP](/support/?type=documents&path=netdrive_manual/add-configure-drive&page=ftp-config)
  - [Google Drive](/support/?type=documents&path=netdrive_manual/add-configure-drive&page=google-drive-config)
  - [Google Cloud Storage](/support/?type=documents&path=netdrive_manual/add-configure-drive&page=google-cloud-storage-config)
  - [hubiC](/support/?type=documents&path=netdrive_manual/add-configure-drive&page=hubic-config)
  - [OneDrive](/support/?type=documents&path=netdrive_manual/add-configure-drive&page=onedrive-config)
  - [OneDrive for Business](/support/?type=documents&path=netdrive_manual/add-configure-drive&page=onedrive-for-business-config)
  - [S3](/support/?type=documents&path=netdrive_manual/add-configure-drive&page=s3-config)
  - [S3 Compatible](/support/?type=documents&path=netdrive_manual/add-configure-drive&page=s3-comp-config)
  - [SFTP](/support/?type=documents&path=netdrive_manual/add-configure-drive&page=sftp-config)
  - [Swift](/support/?type=documents&path=netdrive_manual/add-configure-drive&page=swift-config)
  - [ucloud biz](/support/?type=documents&path=netdrive_manual/add-configure-drive&page=ucloud-biz-config)
  - [WebDAV](/support/?type=documents&path=netdrive_manual/add-configure-drive&page=webdav-config)
  - [Amazon Drive (discontinued)](/support/?type=documents&path=netdrive_manual/add-configure-drive&page=amazon-drive-config)

* "OPTIONS" button allows to set available options values of each storage type.

- After authentication, click "BROWSE" button to browse the remote path.

<img class="markdown" src="https://doc.bdrive.com/images/add_configure_drive_2.jpg">

- Type in the name of the drive item in LABEL category.

<img class="markdown" src="https://doc.bdrive.com/images/add_configure_drive_3.jpg" style="width:300px">

- Click "COLOR" button to select the background color of each drive item.

<img class="markdown" src="https://doc.bdrive.com/images/add_configure_drive_4.png" style="width:300px">

- Select drive letter for each mounted drive in MOUNT category. You may also select drive type, either network drive or local drive.

<img class="markdown" src="https://doc.bdrive.com/images/add_configure_drive_5.jpg" style="width: 500px">

- AUTO CONNECT OPTIONS

  - **No automatic mount** : Connects only when user proceeds CONNECT command.
  - **Mount on boot** : Connects on system boot (Windows only). Note connected drives will be shown to all windows users since it is connected by SYSTEM account.
  - **Mount on login** : Connects when Bdrive account is logged on after NetDrive Application is executed.

* UPLOAD OPTIONS : This option applies when you upload files using Windows Explorer or macOS Finder

  - **Use background uploading** : After configuring a file in local cache, uploads files to remote site. Even the file copy is completed in Windows Explorer, it is possible that NetDrive is still uploading the file in background.
  - **Use on-the-fly uploading in Explorer** : Copies files without using cache. It might be slightly slower than background uploading.

- READ ONLY OPTIONS

  - **Writable drive** : Connects as writable drives.
  - **Read only drive** : Connects as read only drives. Create/delete/rename of file or folder is not possible.

* ADVANCED OPTION

  - **Always retrieve file list from server** : Does not use cache on file list but instead calls for the file list from the server. It might be slight slower in terms of speed.
  - **As a removable drive** : Connects as removable drive such as USB memory stick.
  - **Treat files and folders starting with a dot as hidden** : Files and folders with starting dot will not be shown.

- Click "OK" button to finish adding a drive item.