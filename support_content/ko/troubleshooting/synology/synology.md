### Synology NAS WebDAV 연결 문제 체크사항

#### 사용자가 WebDAV 서버에 대한 권한이 있는지 확인

Synology NAS DSM의 제어판에 있는 "User" 메뉴에서 "WebDAV 서버"의 권한을 설정할 수 있습니다.

제어판에서 “User” 메뉴를 선택하고 WebDAV과 연결하는 사용자를 선택한 후에 “Edit” 버튼을 누릅니다.

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/troubleshooting/synology/Picture1.png)

“Applications” 탭으로 이동하여 WebDAV Server의 “Allow” 항목을 선택합니다.

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/troubleshooting/synology/Picture2.png)

#### Synology NAS DSM에서 사용자의 IP가 차단되었는지 확인

Synology NAS DSM의 차단 목록에서 사용자의 IP가 등록되었는지 확인합니다. 만약 사용자의 IP가 차단 목록에 등록되어 있다면 차단 목록에서 제거합니다.

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/troubleshooting/synology/Picture3.png)

#### Synology NAS WebDAV 설정 포트 확인

Synology NAS WebDAV에서 설정한 포트를 NetDrive의 Drive Item WebDAV 연결 설정에 알맞게 입력했는지 확인합니다.

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/troubleshooting/synology/Picture4.png)

 ![DDNS Setup](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/troubleshooting/synology/Picture5.png)

#### Synology NAS 재시작

간헐적으로 Synology NAS WebDAV 응용 프로그램이 제대로 작동하지 않는 경우가 있습니다. 이럴 경우 외부에서 WebDAV에 연결하는데 실패가 발생합니다. Synology NAS를 재시작하고 다시 연결을 시도합니다.

#### 라우터 설정 확인

라우터의 Software update 이후 라우터의 설정이 바뀌는 경우가 있습니다. 포트 포워딩을 사용할 경우 포트 변경이 없는지 확인합니다.

