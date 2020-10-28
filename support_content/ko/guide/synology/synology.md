### NetDrive & Synology NAS WebDAV 연결 가이드

#### 1. Synology NAS에서 WebDAV 활성화

Synology NAS에서 WebDAV을 설치해야 합니다. 패키지 센터로 이동하여 WebDAV Server 패키지를 설치합니다.
 
 ![Install WebDAV](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture1.png)

#### WebDAV 설정

WebDAV Server를 실행하고 HTTP 활성화 및 HTTPS 활성화 두 항목을 선택합니다. 기본적으로 Synology WebDAV은 HTTP 포트로 5005를 사용하고 HTTPS 포트로 5006을 사용합니다.
 
 ![Setup WebDAV](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture2.png)

#### DDNS 설정

로컬 네트워크가 아닌 외부에서 Synology NAS에 접속하기 위해서는 DDNS 설정이 필요합니다. DDNS 설정을 통해 외부에서 Synology NAS에 접속할 수 있습니다. (이미 Synology NAS에 접속 가능하게 DDNS가 설정되어 있다면 생략)
 
 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture3.png)

#### Synology NAS WebDAV과 NetDrive 연결

#####	새로운 Drive Item 추가

“Start here”에 있는 “+” 버튼을 눌러 새로운 Drive Item 추가를 시작합니다.
 
 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture4.png)

#####	WebDAV STORAGE TYPE 선택

STORAGE TYPE 리스트에서 WebDAV 항목을 선택한 후 “CONNECT” 버튼을 누릅니다.
 
 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture5.png)

##### WebDAV 연결 설정

Server 항목에서 Synology WebDAV 연결에 대한 URL과 포트를 입력합니다. HTTPS를 사용할 경우 “Use SSL(https)” 항목을 선택합니다. (Synology NAS WebDAV에서 기본적으로 설정된 HTTP 포트는 5005, HTTPS 포트는 5006을 사용)

Account 정보에 User ID, Password를 입력합니다. (해당 Account가 WebDAV에 접근할 수 있는 권한이 있어야 합니다)

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture6.png)

##### Drive Item에 대한 기본 설정

Configure a Personal Drive 페이지에서 Drive Item에 대한 기본 설정을 합니다. Drive Item의 기본 설정에 대해서는 [매뉴얼](https://www.netdrive.net/support/?type=documents&path=netdrive_manual/add-configure-drive&page=webdav-config)을 참고하시기 바랍니다. 

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture7.png)
 

##### Drive Item 마운트

생성된 WebDAV Drive Item에서 “CONNECT” 버튼을 눌러 추가한 WebDAV을 PC에 마운트 시킵니다.

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture8.png)
 

##### 마운트 된 WebDAV 확인

파일 탐색기에서 Synology NAS WebDAV이 정상적으로 마운트 된 것을 확인할 수 있습니다.
 
 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture9.png)
 
#### Synology NAS WebDAV 연결 문제 체크사항

##### 사용자가 WebDAV 서버에 대한 권한이 있는지 확인

Synology NAS DSM의 제어판에 있는 "User" 메뉴에서 "WebDAV 서버"의 권한을 설정할 수 있습니다.

제어판에서 “User” 메뉴를 선택하고 WebDAV과 연결하는 사용자를 선택한 후에 “Edit” 버튼을 누릅니다.

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture10.png)

“Applications” 탭으로 이동하여 WebDAV Server의 “Allow” 항목을 선택합니다.

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture11.png)

##### Synology NAS DSM에서 사용자의 IP가 차단되었는지 확인

Synology NAS DSM의 차단 목록에서 사용자의 IP가 등록되었는지 확인합니다. 만약 사용자의 IP가 차단 목록에 등록되어 있다면 차단 목록에서 제거합니다.

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture12.png)

##### Synology NAS WebDAV 설정 포트 확인

Synology NAS WebDAV에서 설정한 포트를 NetDrive의 Drive Item WebDAV 연결 설정에 알맞게 입력했는지 확인합니다.

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture13.png)

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/synology/Picture14.png)

##### Synology NAS 재시작

간헐적으로 Synology NAS WebDAV 응용 프로그램이 제대로 작동하지 않는 경우가 있습니다. 이럴 경우 외부에서 WebDAV에 연결하는데 실패가 발생합니다. Synology NAS를 재시작하고 다시 연결을 시도합니다.

##### 라우터 설정 확인

라우터의 Software update 이후 라우터의 설정이 바뀌는 경우가 있습니다. 포트 포워딩을 사용할 경우 포트 변경이 없는지 확인합니다.


