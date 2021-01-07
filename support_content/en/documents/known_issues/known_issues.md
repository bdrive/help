### File listing (WebDAV, FTP/FTPS/ SFTP)

For WebDAV, FTP/FTPS, SFTP protocols file list reloading from server will be blocked for a folder where files are being uploaded. File listing for other folders are working without any limits.

Because of this limitations, files uploaded to **the same folder** from other users will be shown when file uploading is finised.

### File system is not available (macOS)

<img class="markdown" src="https://doc.bdrive.com/images/manual_limitations_fs_not_available.jpg">

When you cannot mount remote storage on macOS

NetDrive needs to register a virtual device for user to access virtual file systems. The number of available virtual device slots are limited by macOS. So if you are using other softwares that uses these device slots NetDrive will not be able to register its virtual device and it cannot connect to remote storages.

You can list currently registered virtual devices using following command.

    $ kextstat
    Index Refs Address            Size       Wired      Name (Version) UUID <Linked Against>
    1  119 0xffffff7f80c58000 0xc340     0xc340     com.apple.kpi.bsd (19.2.0) C509F3BC-8645-439D-83FF-246EF205D74F
    2   12 0xffffff7f80c99000 0x5d00     0x5d00     com.apple.kpi.dsep (19.2.0) 4FD0D85E-D4C8-4EA5-85EE-58576053BC4B
    3  145 0xffffff7f80c11000 0x257a0    0x257a0    com.apple.kpi.iokit (19.2.0) EF98EB82-7671-47D2-8209-4107EC24B00D
    4    0 0xffffff7f83535000 0x57e0     0x57e0     com.apple.kpi.kasan (19.2.0) BA25574A-60E7-46D4-9D88-58E508D4BD94
    5  151 0xffffff7f80c00000 0x100b0    0x100b0    com.apple.kpi.libkern (19.2.0) 951CBB94-0DD9-40D3-B0C3-2BD5545A4CBA
    6  134 0xffffff7f80c37000 0x62e0     0x62e0     com.apple.kpi.mach (19.2.0) 2F53974D-C9C7-4F5B-AB4D-8AB55924F774
    7   87 0xffffff7f80c3e000 0x104c0    0x104c0    com.apple.kpi.private (19.2.0) 74F84085-D361-41A0-A3D5-0E616E23E88C
    8   89 0xffffff7f80c4f000 0x8200     0x8200     com.apple.kpi.unsupported (19.2.0) D822DE60-38DA-4E55-8422-C371551488BA
    9    2 0xffffff7f80d5d000 0x10000    0x10000    com.apple.kec.Libm (1) 93FADEC1-CBCF-3B33-A28E-6DC4C01CA22D <5>
    ...

It can list more than hundred devices registered to your system (YMMV).

Use following command to list only third party devices.

    $ kextstat | grep -v com.apple

You can unload kext using following command.

    $ sudo kextunload -b com.company.virtualfilesystem

After unload some kexts please install NetDrive again to register NetDrive virtual device.

### Locked files shown to be deleted (Windows)

From NetDrive 3.9 we supports file locking. Locked files cannot be overwritten, renamed or deleted. On Windows operating system when you try to delete locked file it is deleted and will disappear from Windows Explorer but actually the file is not removed from your server. After refresh or remount you can find your file again.

This is a known issue and we are looking for the solution.

### Failed to upgrade from 3.7 and below (Windows)

If you have problem when upgrading from NetDrive 3.7 and below please uninstall first and install recent version.

### Failed to unzip on Finder (macOS)

macOS tries to create a temporary folder in parent folder and unzip files into the temporary folder.

Unzip fails if the zip files is located at the root folder or a folder where it's parent folder cannot create a temporary folder (like top most folder of Synology WebDAV).

In this case move the zip file to subdirectories, unzip the file and move back the unzipped files. It's better to move the zip file to your local hard disk for unzipping.
