# Google Drive

---

NOTE: All users of NetDrive share the same Google Drive API client ID for accessing their files. If your connection suffers from slow download and/or upload please register your own client ID.

---

**1. Open [https://console.developers.google.com](https://console.developers.google.com) in your browser and log in to your google account.**


**2. Click 'Select a project'**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/2/212a8ffa5381dd8527068913b6ce9ffca80ace8b.png" width="700px" style="border: 1px solid black;">


**3. Click 'NEW PROJECT'**

If you have a project already, you can use it.

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/5/59018053aa7fd122e5d6c75da19ec5f154a3893a.png" width="700px" style="border: 1px solid black;">



**4. Input project name, Organization and Location then create it.**

You need to set your own Organization and Location.

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/d/d5ae3065fc9b0aea3530629a0abae5fc96b42cb5.png" width="700px" style="border: 1px solid black;">


**5. Create project may take some time. Wait and choose 'Select a project' again then open project that you've created.**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/7/75597fa3448b51257f7f38e93319aae0c9c0dbee.png" width="700px" style="border: 1px solid black;">



**6. Click 'ENABLE APIS AND SERVICES'**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/f/f9ece0e7cd443f058b0e07e006eac0b4243d53b9.png" width="700px" style="border: 1px solid black;">



**7. Search for 'google drive api' and click 'Google Drive API'**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/8/8672a8337204f895c8babf88f3cb7157b1340579.png" width="700px" style="border: 1px solid black;">




**8. Enable it**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/5/5b845dd5e4009f8efb6704970efabf7f237105e3.png" width="700px" style="border: 1px solid black;">


**9. Click API name to get back to dashboard**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/c/c6b8773bafb532a03022d222f9a83b56ad304a3b.png" width="700px" style="border: 1px solid black;">


**10. Click 'OAuth consent screen'**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/d/dad3c339657c929ddc993a00065182905c0ae548.png" width="700px" style="border: 1px solid black;">


Select Internal as User Type:

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/8/828386a26e3bebd2d4404b0563edc1ea0ffc1f96.png" width="700px" style="border: 1px solid black;">


**11. Set your application name, application logo and support email**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/b/b0f65335d7a8ac6072a8c4444d6d77191c2c5b70.png" width="700px" style="border: 1px solid black;">



**12. Click Add scope button**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/f/f2764b7448695adba97026c41790a1d33853ee38.png" width="700px" style="border: 1px solid black;">



**13. Select 'Google Drive API ../auth/drive and click 'ADD' button**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/1/1bc33f4cab830e0c4116d125a5ea97387409df6e.png" width="700px" style="border: 1px solid black;">

**14. Enter 'bdrive.com' for Authorized domains**

We need this for OAuth to work in NetDrive or CloudSync.


>**Don't forget to press enter!**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/7/764c30029bb14c7d842986a2c1b87f2fc7ace89e.png" width="700px" style="border: 1px solid black;">


**15. Enter additional links and click 'Save' button**

If you want to use this API key for CloudSync change domains to https://cloudsync.bdrive.com/.

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/3/35424dd6476e89313a5259b2d709221f4a3372f7.png" width="700px" style="border: 1px solid black;px" style="border: 1px solid black;">

For copy and paste:

* https://netdrive.bdrive.com
* https://netdrive.bdrive.com/wiki/netdrive/privacy-policy
* https://netdrive.bdrive.com/wiki/nertdrive/eula

Ignore warnings like below because this API key is for you only.

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/e/e635a7cc4243013c4eeff10d1afd1296ff303227.png" width="700px" style="border: 1px solid black;">


**16. Click 'Credentials'**

**Select 'Create credentials'**

 **Select 'OAuth client ID'**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/3/35eee24abc789fae73bb3d0be7861dd32a600cc5.png" width="700px" style="border: 1px solid black;">


**17. Choose 'Web application' and name it.**

**Add 'https://accounts.bdrive.com/oauth/' to 'Authorized redirect URIs'. Don't forget to press Enter key.**

**Click 'Create' button**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/c/c4e8b86863a83ec9c6bae57950f8007d9d65c8cc.png" width="700px" style="border: 1px solid black;">

You need to press enter after input **https://accounts.bdrive.com/oauth/**.

If the redirect uri is successfully added your screen will show the uri like this:

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/7/72acc976179271ed338d349043049eda8e7a24eb.png" width="700px" style="border: 1px solid black;">


**18. Your OAuth client ID and client secret will be displayed**

**We need this later. Save your client ID and client secret to a text file**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/0/0122f2495f834a442850be1015b5aff8fe8366c3.png" width="500px" style="border: 1px solid black;">

**19. Open [https://accounts.bdrive.com](https://accounts.bdrive.com) in your browser and log in.**

**Click 'Manage Cloud Service Secrets**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/optimized/2X/8/825ef7311a73184dee331eecb8eb96ccf1e6c354_2_1380x842.png" width="700px" style="border: 1px solid black;">

**20. Click 'Register'**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/9/995d1ffb7f5911e83fd27e3b207fe168c97d8e8c.png" width="500px" style="border: 1px solid black;">

**21. Choose 'Google Drive' in type and input client id and secret from step 18.**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/1/1feb3d17103373e7866457165a4dc80b9ea1f444.png" width="500px" style="border: 1px solid black;">

**22. Click register  and its done!!**

**IMPORTANT: You have to add new drive item to use registered client id and secret.**

When adding new Google Drive item web browser will be opened and you can select your client ID.

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/optimized/2X/6/6f29a9f4df89cbbf0e02d2fe80db92d9c838660f_2_1034x582.png" width="700px" style="border: 1px solid black;px" style="border: 1px solid black;">