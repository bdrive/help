### WebDAV

CONNECT
==================
STORAGE TYPE에서 WebDAV를 선택한 후, CONNECT 버튼을 누르면 아래와 같은 창이 나타납니다.

<img class="markdown" src="https://doc.bdrive.com/images/webdav_config_1.jpg">

WebDAV server의 주소를 입력합니다. 

* Synology NAS의 경우 기본 port는 5005, SSL을 사용하는 경우의 port는 5006입니다.

User account와 password를 입력합니다. 저장하고 싶지 않다면 "Save user and password"를 체크하지 않으면 됩니다. 그러면 접속할 때마다 입력해야합니다.


OPTIONS
==================

<img class="markdown" src="https://doc.bdrive.com/images/webdav_config_2.jpg">

* Use server time for files/folders : local pc의 timezone 적용을 하지 않고 서버에 저장되어 있는 파일 또는 폴더의 시간을 그대로 보여줍니다.

* MS SharePoint Server : 설치형 SharePoint Server에 WebDAV 으로 접속할때 체크합니다. Office365에서 제공하는 Sharepoint Online은 지원되지 않습니다.

* Attempt converting non-UTF-8 files to UTF-8 : 파일 이름이 UTF-8 인코딩이 아닌 경우, 파일명을 UTF-8로 변경하는 것을 시도하는 것에 대한 옵셥입니다.

* Bandwidth : 대역폭을 조절할 수 있습니다.