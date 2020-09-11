### Google Drive

#### 1.	Google Drive가 느린 경우 - 나만의 Google API 키 등록

---

NOTE: NetDrive의 모든 사용자는 파일에 액세스하기 위해 동일한 Google Drive API client ID를 공유합니다. 다운로드 또는 업로드 속도가 느릴 경우, 나만의 client ID를 등록합니다.

---

**1. 브라우저에서 ‘https://console.developers.google.com’를 열고 Google 계정에 로그인합니다.**

**2. '프로젝트 선택'을 클릭합니다.**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/2/212a8ffa5381dd8527068913b6ce9ffca80ace8b.png" width="700px" style="border: 1px solid black;">


**3. 'NEW PROJECT’를 클릭합니다.**

이미 프로젝트가 있는 경우 해당 프로젝트를 사용할 수 있습니다.

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/5/59018053aa7fd122e5d6c75da19ec5f154a3893a.png" width="700px" style="border: 1px solid black;">



**4. 프로젝트 이름, 소속, 위치를 입력하고 생성합니다.**

 자신의 소속 및 위치를 설정해야 합니다.

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/d/d5ae3065fc9b0aea3530629a0abae5fc96b42cb5.png" width="700px" style="border: 1px solid black;">


**5. 프로젝트 생성에 시간이 걸릴 수 있습니다. 기다렸다가 다시 ' Select a project'을 선택한 다음 생성한 프로젝트를 엽니다.**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/7/75597fa3448b51257f7f38e93319aae0c9c0dbee.png" width="700px" style="border: 1px solid black;">



**6. 'ENABLE APIS AND SERVICES'를 클릭합니다.**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/f/f9ece0e7cd443f058b0e07e006eac0b4243d53b9.png" width="700px" style="border: 1px solid black;">



**7. 'Google Drive API'를 검색하고 'Google Drive API'를 클릭합니다.**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/8/8672a8337204f895c8babf88f3cb7157b1340579.png" width="700px" style="border: 1px solid black;">




**8. Google Drive API를 활성화합니다.**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/5/5b845dd5e4009f8efb6704970efabf7f237105e3.png" width="700px" style="border: 1px solid black;">


**9. Google Drive API 이름을 클릭하여 대시보드로 돌아갑니다.**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/c/c6b8773bafb532a03022d222f9a83b56ad304a3b.png" width="700px" style="border: 1px solid black;">


**10. 'OAuth consent screen’를 클릭합니다.**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/d/dad3c339657c929ddc993a00065182905c0ae548.png" width="700px" style="border: 1px solid black;">


User Type으로 ‘Internal’을 선택합니다

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/8/828386a26e3bebd2d4404b0563edc1ea0ffc1f96.png" width="700px" style="border: 1px solid black;">


**11. 애플리케이션 이름, 애플리케이션 로고 및 지원 이메일을 설정합니다.**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/b/b0f65335d7a8ac6072a8c4444d6d77191c2c5b70.png" width="700px" style="border: 1px solid black;">


**12. ‘Add scope’ 버튼을 클릭합니다.**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/f/f2764b7448695adba97026c41790a1d33853ee38.png" width="700px" style="border: 1px solid black;">


**13. 'Google Drive API …/auth/drive'를 선택하고 'ADD' 버튼을 클릭합니다.**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/1/1bc33f4cab830e0c4116d125a5ea97387409df6e.png" width="700px" style="border: 1px solid black;">

**14. Authorized domains에 'bdrive.com'을 입력합니다.**

OAuth가 NetDrive 또는 CloudSync에서 작동하려면 이것이 필요합니다.

>**Enter를 누르는 것을 잊지 마십시오!**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/7/764c30029bb14c7d842986a2c1b87f2fc7ace89e.png" width="700px" style="border: 1px solid black;">


**15. 추가 링크를 입력하고 'Save' 버튼을 클릭합니다.**

이 API 키를 CloudSync에 사용하려면 도메인을 ‘https://cloudsync.bdrive.com/’으로 변경하십시오.

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/3/35424dd6476e89313a5259b2d709221f4a3372f7.png" width="700px" style="border: 1px solid black;px" style="border: 1px solid black;">

복사 및 붙여 넣기:
* https://netdrive.bdrive.com 
* https://netdrive.bdrive.com/wiki/netdrive/privacy-policy 
* https://netdrive.bdrive.com/wiki/nertdrive/eula 

이 API 키는 사용자 전용이므로 아래와 같은 경고를 무시하십시오.

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/e/e635a7cc4243013c4eeff10d1afd1296ff303227.png" width="700px" style="border: 1px solid black;">


**16. 'Credentials'를 클릭합니다.**

'Create credentials'를 선택합니다.

'OAuth client ID'를 선택합니다.

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/3/35eee24abc789fae73bb3d0be7861dd32a600cc5.png" width="700px" style="border: 1px solid black;">


**17. ' Web application'을 선택하고 이름을 지정합니다.**

'Authorized redirect URIs'에 'https://accounts.bdrive.com/oauth/'을 추가합니다. Enter 키를 누르는 것을 잊지 마십시오.

'Create' 버튼을 클릭합니다.

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/c/c4e8b86863a83ec9c6bae57950f8007d9d65c8cc.png" width="700px" style="border: 1px solid black;">

**‘https://accounts.bdrive.com/oauth/’**를 입력한 후 Enter 키를 눌러야 합니다.

리다이렉트 URI가 성공적으로 추가되면 화면에 다음과 같은 URI가 표시됩니다.

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/7/72acc976179271ed338d349043049eda8e7a24eb.png" width="700px" style="border: 1px solid black;">


**18. 당신의 OAuth client ID와 client secret이 표시됩니다.**

이것은 나중에 필요합니다. client ID 및 client secret를 텍스트 파일에 저장합니다.

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/0/0122f2495f834a442850be1015b5aff8fe8366c3.png" width="500px" style="border: 1px solid black;">

**19. 브라우저에서 ‘https://accounts.bdrive.com’을 열고 로그인합니다.**

'Manage Cloud Service Secrets'를 클릭합니다.

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/optimized/2X/8/825ef7311a73184dee331eecb8eb96ccf1e6c354_2_1380x842.png" width="700px" style="border: 1px solid black;">

**20. 'Register'을 클릭합니다.**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/9/995d1ffb7f5911e83fd27e3b207fe168c97d8e8c.png" width="500px" style="border: 1px solid black;">

**21. Type에서 'Google Drive'를 선택하고 18 단계에서 저장한 client ID와 secret를 입력합니다.**

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/original/2X/1/1feb3d17103373e7866457165a4dc80b9ea1f444.png" width="500px" style="border: 1px solid black;">

**22. ‘Register’ 버튼을 클릭하여 완료**

중요: 등록된 client ID와 secret를 사용하려면 새로운 Drive Item을 추가해야 합니다.

새로운 Google Drive Item을 추가하면 웹 브라우저가 열리고 client ID를 선택할 수 있습니다.

<img src="https://files-discourse-bdrive-com.s3.dualstack.us-east-1.amazonaws.com/optimized/2X/6/6f29a9f4df89cbbf0e02d2fe80db92d9c838660f_2_1034x582.png" width="700px" style="border: 1px solid black;px" style="border: 1px solid black;">

**23. client ID와 secret를 사용하려면 새로운 Google Drive Item을 추가해야 합니다.**