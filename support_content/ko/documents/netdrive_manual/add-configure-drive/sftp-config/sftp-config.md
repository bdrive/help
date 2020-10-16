### SFTP

CONNECT
==================
STORAGE TYPE에서 SFTP를 선택한 후, CONNECT 버튼을 누르면 아래와 같은 창이 나타납니다.

<img class="markdown" src="https://doc.bdrive.com/images/sftp_config_1.jpg">

* sftp 서버의 주소와 port를 입력합니다.
* User account와 Password를 필요로 하는 접속이라면 입력합니다. User account와 password를 저장하고 싶지 않다면 "Save user and password"를 체크하지 않습니다. 그러면 Connect할때마다 User account와 password를 입력해야 합니다. 

* Private key를 이용해서도 접속할 수 있습니다. "BROWSE"를 눌러서 private key file을 선택합니다. putty format은 지원하지 않고 openssh format만 지원하고 있습니다. private key file에 passpharse가 있다면 입력합니다. passphrase의 저장도 선택할 수 있습니다.


OPTIONS
==================

<img class="markdown" src="https://doc.bdrive.com/images/sftp_config_2.jpg">

* Use server time for files/folders : local pc의 timezone 적용을 하지 않고 서버에 저장되어 있는 파일 또는 폴더의 시간을 그대로 보여줍니다.

* Use new file permission : 새로운 파일을 생성할때 파일의 접근 권한을 설정할 수 있습니다.

* Use new folder permission : 새로운 폴더를 생성할때 폴더의 접근 권한을 설정할 수 있습니다.

* Mount Point
    * User home : 사용자의 홈 폴더를 연결합니다.
    * System root : sftp 서버의 시스템 루트를 연결합니다.

* Max sessions : NetDrive의 성능을 위해 동시에 여러개의 세션을 사용하여 데이터를 주고 받습니다. 이때 사용하는 세션의 수를 제한할 수 있습니다.

* Bandwidth : 대역폭을 조절할 수 있습니다.