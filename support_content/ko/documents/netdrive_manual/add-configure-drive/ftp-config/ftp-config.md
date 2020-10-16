### FTP

CONNECT
==================
STORAGE TYPE에서 FTP를 선택한 후, CONNECT 버튼을 누릅니다.

<img class="markdown" src="https://doc.bdrive.com/images/ftp_config_1.jpg">


<img class="markdown" src="https://doc.bdrive.com/images/ftp_config_2.jpg">


그러면 위와 같이 FTP의 접속 정보를 입력할 수 있는 창이 나타납니다.

ftp 서버의 주소와 사용하는 port를 정확하게 입력합니다.
SSL/TLS를 사용한다면 "Use SSL/TLS"를 체크합니다.

Active Mode를 사용해야 하는 경우에는 "Use Active Mode"를 체크합니다.

User에는 FTP 사용자 계정을 입력하고, Password에는 FTP 사용자 계정의 비밀번호를 입력합니다.

익명으로 접속하는 경우에는 "Anonymous"를 체크합니다.

FTP 사용자 계정과 비밀번호를 저장하고 싶지 않다면 "Save user and password"를 체크하지 않습니다. 
그러면 드라이브 아이템을 연결하려고 할때마다 FTP 사용자 계정과 비밀번호를 입력해야 합니다.

접속 정보를 모두 입력하고 "OK" 버튼을 누르면 접속 시도를 하게 되고, 성공하면 이전의 창으로 돌아갑니다.

OPTIONS
==================

<img class="markdown" src="https://doc.bdrive.com/images/ftp_config_3.jpg">

* Charset : 파일이름의 인코딩 정보를 설정합니다. 
    * Autodetect : FTP 서버가 UTF-8을 지원하는지 지원하지 않는지 검출한 후 동작합니다.
    * Force UTF-8 : FTP 서버와 파일이름을 주고 받을때 강제로 UTF-8을 사용합니다.
    * Local charset : FTP 서버와 파일이름을 주고 받을때 local pc의 charset을 이용합니다.

* Use server time for files/folders : local pc의 timezone 적용을 하지 않고 서버에 저장되어 있는 파일 또는 폴더의 시간을 그대로 보여줍니다.

* Max sessions : NetDrive의 성능을 위해 동시에 여러개의 세션을 사용하여 데이터를 주고 받습니다. 이때 사용하는 세션의 수를 제한할 수 있습니다.

* Bandwidth : 대역폭을 조절할 수 있습니다.