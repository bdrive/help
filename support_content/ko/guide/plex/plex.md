### NetDrive + PLEX + Cloud Storage 연결 가이드

#### 1. Cloud Storage 선택

NetDrive에서 지원하는 Cloud Storage를 선택하여 Media Storage로 사용합니다.

#####	NetDrive에서 지원하는 Cloud Storage 목록

1.	구글 드라이브/공유 드라이브/공유문서함 (Google Drive/Shared Drive/Shared)
2.	드롭박스 (Dropbox)
3.	드롭박스 비지니스 (Dropbox for Business)
4.	원드라이브/공유문서함 (OneDrive/Shared)
5.	원드라이브 비지니스/공유문서함 (OneDrive for Business/Shared)
6.	박스 (Box)
7.	메가 (MEGA)
8.	유클라우드 비즈 (ucloud biz)
9.	얀덱스 디스크 (Yandex Disk)
10.	구글 클라우드 스토리지 (Google Cloud Storage)
11.	아마존 S3 (Amazon Web Service S3)
12.	애저 블롭 스토리지 (Azure Blob Storage)
13.	애저 파일 스토리지 (Azure File Storage)
14.	스위프트 (Swift)
15.	휴빅 (Hubic)
16.	백블레이즈 B2 (Backblaze B2)
17.	WebDAV (Web Distributed Authoring and Versioning)
18.	FTP/FTPS (File Transfer Protocol, FTP Secure)
19.	SFTP (SSH/Secure File Transfer Protocol)
20.	와사비 (Wasabi)
21.	파일 베이스 (filebase)
22.	오픈스택 (OpenStack)
23.	4쉐어 (4Shared)
24.	클라우드 미 (CloudMe)
 
 ![Supported Protocols](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/plex/Picture1.png)

* 해당 가이드의 환경 구성은 NetDrive에서 지원하는 Cloud Storage 중에 하나인 Google Drive로 테스트하였습니다.

#### 2.	미디어 리소스 확보 및 구성

Plex 네이밍 규칙에 맞게 폴더 구조와 파일 명을 구성합니다.
 
 ![Media Resource](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/plex/Picture2.png)
 
##### 영화 

https://support.plex.tv/articles/naming-and-organizing-your-movie-media-files/

 ![Media Resource](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/plex/Picture3.png)

##### TV Show 

https://support.plex.tv/articles/naming-and-organizing-your-tv-show-files/

 ![Media Resource](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/plex/Picture4.png)

#### 3.	NetDrive와 Cloud Storage 연결

NetDrive에서 Media Storage와 연결하는 Drive Item을 생성하고 PC에 마운트 시킵니다.

Google Drive를 이용할 경우 나만의 Google API 키를 등록하여 사용하는 것이 좋습니다(기본적으로 NetDrive를 이용하는 모든 사용자는 NetDrive에서 제공하는 동일한 Google Drive API를 사용하기 때문에 나만의 Google API 키를 등록하여 사용해야만 빠른 속도의 스트리밍을 이용할 수 있습니다).   
나만의 Google API Key를 생성하고 등록하는 방법   
https://support.bdrive.com/t/slow-google-drive-how-to-register-your-own-google-api-key/18503
 
 ![Connect Storage](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/plex/Picture5.png)

#### 4.	Plex Media Server 설치

Plex 홈페이지에서 회원가입을 하고 Plex Media Server를 다운로드 받아서 PC에 설치합니다.   
https://www.plex.tv/media-server-downloads/   
Plex Media Server를 실행하고 “Add Library”를 이용하여 NetDrive에서 PC에 마운트 한 Media Storage 경로를 Library에 추가합니다. 

 ![Setup Plex](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/plex/Picture6.png)
 
 ![Setup Plex](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/plex/Picture7.png)

* 외부에서 접속이 안될 경우 라우터에서 포트 포워딩 설정이 필요할 수 있습니다.   
Plex Media Server의 “Remote Access” 항목에서 포트 번호를 수동으로 설정한 후 라우터의 포트 포워딩 설정에서 수동으로 설정한 포트를 입력하여 포트 포워딩을 설정합니다.

 ![Setup Plex](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/plex/Picture8.png)

#### 5.	Media 실행

설정은 모두 끝났습니다. 이제 Plex Client Software를 통해서 보고싶은 미디어를 선택하여 실행하면 됩니다.   
아래의 경로에서 실행하려는 디바이스 환경에 맞게 다운로드 받아 설치합니다.   
https://www.plex.tv/media-server-downloads/#plex-app
 
 ![Start Media](https://raw.githubusercontent.com/bdrive/help/master/support_content/en/guide/plex/Picture9.png)

Plex Client Software를 실행하고 로그인합니다. Library 경로에 있는 미디어 파일 목록을 볼 수 있습니다.   
보고싶은 미디어를 선택하여 재생합니다.

