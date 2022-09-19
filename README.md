# Linux in Window

## 1. Linux 설치

### VMware

- <img src="https://user-images.githubusercontent.com/66783849/190838258-9c73c73f-7660-45ae-b48f-64032e1f45f1.png" width="30%">
- VMware 주식회사는 클라우드 컴퓨팅 및 가상화 소프트웨어를 판매하는 기업이다.
- 다음 소프트 웨어를 공급한다.
  - VM웨어 워크스테이션(VMware Workstation)
  - VM웨어 서버(VMware Server) (프리웨어 제품)
  - VM웨어 플레이어(VMware Player) (프리웨어 제품)
  - x86 호환 컴퓨터를 위한 가상화 소프트웨어
- VM웨어의 데스크탑 소프트웨어는 마이크로소프트 윈도우, 리눅스, macOS을 지원한다.
- VMware Play를 활용하여 Linux를 실행한다.

<br>

### VMware 설치

- [VMware Player 설치 사이트](https://www.vmware.com/kr/products/workstation-player/workstation-player-evaluation.html)
- VMware Player 실행 화면  
  <img src="https://user-images.githubusercontent.com/66783849/190838635-11f3e829-4525-4235-98e7-978f33c8840b.png" width="70%">
- 기본적으로 재공되는 linux.ios들이 존재한다.

<br>

### Ubuntu 설치

<img src="https://user-images.githubusercontent.com/66783849/190838997-93244cf5-1daa-4a49-b1cb-275fd8628110.png" width="30%">

- Linux는 다양한 배포판이 존재한다.
  - 리눅스 베포판이란, 리눅스에서 작동하는 여러 종류의 프로그램을 꾸러미 하나로 모아놓은 것을 말한다.
  - Red Hat, CentOS, Debian, Fedora, Linux Mint, ubuntu 등등이 있다.
    - Utuntu : GNU/Linux를 근간으로 하여 사용자 편의성에 초점을 맞춰 개발된다.
    - RedHat Linux : 전 세계 Linux시장의 70~80%를 점유하고 있다.
      - CentOS Linux는 RedHat의 RHEL버전의 클론 버전으로, 무료 배포본이다.
- Ubuntu를 설치받아 VMware Player로 실행한다.
- [Ubuntu 설치 사이트](https://ubuntu.com/desktop) > Download Ubuntu > Download 를 선택하여 iso를 다운받는다.

<br><br>

## 2. VMware Player - Linux Ubuntu 실행

- VMware Player > Create a New Virtual Machine > Installer disc image file (iso): > [Browser...] 버튼 선택 > 설치한 ubuntu.iso 선택 > [Next>] > 이름 및 비밀번호 작성 > [Next>] > Machine 이름 및 경로 지정 > [Next>] > 저장공간 부여 (본인 16GB로 설정) > Setting 확인 후 [Finish]
- 지정한 Machine 이름의 Player 선택 후 Play한다.  
  <img src="https://user-images.githubusercontent.com/66783849/190839290-2ae6c52e-0760-49bc-a7a1-0dc2e38cd826.png" width="70%">
- Ubuntu가 실행이 되고, 요구하는 사항을 전부 입력하면 완료된다.  
- 설치된 Ubuntu > 메뉴 > Terminal앱을 실행하여 Terminal 창을 연다.  
  <img src="https://user-images.githubusercontent.com/66783849/190839639-86dab1b1-a015-49b0-a195-ea76f7e03170.png" width="49%"> <img src="https://user-images.githubusercontent.com/66783849/190839671-5b860f73-c6fa-4d52-bb8a-444d74e1e906.png" width="49%">

<br><br>


## 3. Linux 명령어

- 파일
  - touch : 0바이트 파일 생성, 파일의 날짜와 시간을 수정한다.
  - vi : 명령을 이용한 file 생성한다.
  - ls : 현재 위치의 파일 목록 조회
  - cd :디렉터리 이동 (Change directory)
  - pwd : 현재 작업 디렉토리의 경로를 보여준다. (print working directory)
  - mkdir : 디렉터리 생성한다. (Make Dirctory)
  - rmdir : 디렉토리를 지운다. (Remove directory)
  - rm : 파일을 삭제한다. (-r로 디렉터리 삭제) (Remove)
  - cat (Catenate) : 파일의 내용을 화면에 출력, 리다이렉션 기호('>')를 사용하여 새로운 파일 생성
  - cp : 파일 및 디렉터리를 복사한다. (Copy)
  - mv : 파일 또는 디렉터리의 이름을 바꾸거나 위치를 이동한다. (Move)
- 기타 명령어
  - 파일
    - file : 파일의 종류를 알아본다.
  - 명령
    - which : 명령어의 위치나 alias를 보여준다. 예) which ls -> /bin/ls
    - whereis : 명령어의 소스, 실행 파일, 메뉴얼 페이지등의 위피를 알려준다.
  - 화면
    - clear : 화면 초기화
  - 문서 보기
    - head : 앞에서 n줄 보여준다.
    - tail : 뒤에서 n줄 보여준다.
    - more, less : 페이지로 문서 보기
    - wc : 텍스트 파일의 행수(-l), 단어수(-w), 문자수(-c)를 알려준다. 가장 긴 라인(-L)
    - umask : 새로운 파일이나 디렉토리 생성 시 기본 허가권 
  - 사용자
    - passwd : 유저의 페스워드를 변경한다.
    - group : 이용자가 속한 그룹들의 목록을 출력한다.
    - who : 로그인 중인 유저를 표시한다.
    - whoami : 현재의 실제 유저 ID의 유저명만을 표시한다.
    - w : 현재 로그인 중인 유저의 정보를 표시한다.
    - hostname : 현재 설정되어 있는 호스트의 이름을 표시하거나 변경한다.
  - 부팅
    - dmesg : 부팅시 커널에 출력되는 상태 정보를 볼 수 있도록 하는 프로그램이다.
  - 프로세스
    - ps : 현재 프로세스들의 상태를 PID(process ID)와 RP를 보여준다. 리눅스에서는 사용자, 파일, 프로세스도 번호로 관리할 수 있다. (-u, -l, -e, -f)
    - kill : 프로세스에 특정한 signal을 보내는 명령이다. 보통 중지시킬 수 없는 프로세스를 종료시킬 때 사용한다.

<br>

### 기본 명령어

#### **touch**

- 0바이트 파일 생성, 파일의 날짜와 시간을 수정한다.
- 사용법
  - touch filename : filename의 파일을 생성
  - touch file1 file2 file3 : 파일을 동시에 생성
  - touch -c filename : filename의 시간을 현재시간으로 갱신 (change time)
  - touch -t 202110291608 filename : filename의 시간을 날짜 정보(YYYYMMDDhhmm)로 갱신 (20211029160 => 2021.10.29.16:08)
  - touch -d '2020-09-22 10:45:30' filename : 지정한 시간으로 접근 시간, 수정 시간이 수정되고, 변경시간은 현재 시간으로 수정된다.
  - touch -r oldfile newfile  : newfile의 날짜 정보를 oldfile의 날짜 정보와 동일하게 변경
  - touch -a filename : 현 시간으로 파일의 접근 시간, 변경 시간을 수정한다.
  - touch -m filename : 파일을 생성, 수정시간을 서버 시간으로 갱신
  - touch --help : 해당 명령어의 도움말을 보여주고 실행이 종료한다.
  - touch --version : version 정보를 출력하고 실행이 종료한다.

<br>

#### **vi**

- 명령을 이용한 file 생성한다.
- 기본 사용법
  - 지정한 이름의 파일이 생성되고 vi의 명령모드로 들어간다.
  - 이때 'i'또는 'a'를 누르고 원하는 내용을 입력한다.
  - Esc키를 누르면 다시 명령모드로 복귀한다.
  - “:wq”을 입력하면 파일에 내용이 저장되고 vi가 종료된다.
- 명령모드
  - G : 파일 끝으로 이동
  - dd : 한줄 잘라내기
  - 3dd : 3줄 잘라내기
  - p : 붙여넣기
  - x : 한글자 삭제
  - dw : 단어 삭제
  - u : 실행 취소
  - o : 줄 맨 앞
  - $ : 줄 맨 뒤
- 마지막 행 모드 (ESC > :~~)
  - :w : 저장
  - :q : 종료
  - :wq : 저장 후 종료
  - :set nu : 라인번호
  - :?문자열 : 커서 위치 뒤로 문자열 찾기
  - :/문자열 : 커서 위치 앞으로 문자열 찾기

#### test 텍스트 파일 만들기 실습
- vi test : test 파일 편집기 실행
- i : 내용 편집
- "Hello, World! \엔터 Im Happy" 입력
- ESC : 명령모드
- 첫 번째 줄 커서 이동 후 dd
- 두 번째 줄 커서 이동 후 p
- "I"에 커서를 이동한 후 a를 눌러 "'"를 입력한다.
- 커서를 이동해 x를 눌러 "'m"을 지운다.
- ":wq" : 저장 및 종료
```mermaid
  flowchart TB
  B-- zz -->A_2["vi 종료"]
  A_1["vi 시작"]--->B["명령모드<br>- 커서 이동<br>- 글자/줄 삭제 복사"]
  B -- i, a --> C["입력모드<br>- 입력 내용<br>버퍼로 옮겨져<br>추가/ 삭제"]
  C -- ESC --> B
  B -- : --> D["마지막 행 모드<br>- 저장<br>- 종료"]
  D -- ESC --> B
  D -- w --> D
  D -- q, 4!, w4 --> A_2
  ```

<br>

#### **ls (List segments)**

- ls (List segments) : 현재 위치의 파일 목록 조회
  - ls -l : 파일의 상세정보
  - ls -a : 숨김 파일 표시
  - ls -t : 파일들을 생성시간순(제일 최신 것부터)으로 표시
  - ls -rt : 파일들을 생성시간순(제일 오래된 것부터)으로 표시
  - ls -f : 파일 표시 시 마지막 유형에 나타내는 파일명을 끝에 표시 ('/' : 디렉터리, '*' : 실행파일, '@' : 링크 등등,,,)
  - ls -SS : 용량순 정렬 (-SSr 오름차순, -h 용량 단위 표시)
  - 묶어서 활용 가능하다. 예) ls -al (숨김파일 포함 상세정보), ls -alSSrh (숨김파일 포함하여 용량정보 내림차순 정렬 상세정보) (폴더는 du 명령어를 통해 용량을 확인할 수 있다.)

<br>

#### **cd**

- cd (Change directory) :디렉터리 이동
  - cd [디렉터리 경로] : 이동하려는 디렉터리로 이동 (예 cd folder)
  - cd ~ : 홈 디렉터리로 이동
  - cd / : 최상위 디렉터리로 이동
  - cd . : 현재 디렉터리 
  - cd .. : 상위 디렉터리로 이동
  - cd - : 이전 경로로 이동

<br>

#### **pwd (print working directory)**

- pwd(print working directory) : 현재 작업 디렉토리의 경로를 보여준다.

<br>

#### **mkdir (Make Dirctory)**

- mkdir (Make Dirctory) : 디렉터리 생성
  - mkdir dirname : dirname이라는 디렉터리 생성
  - mkdir dir1 dir2: 한 번에 여러 개의 디렉터리 생성
  - mkdir -p dirname/sub_dirname : dirname이라는 디렉터리 생성, sub_dirname이라는 하위 디렉터리도 생성
  - mkdir -m 700 dirname : 특정 퍼미션(권한)을 갖는 디렉터리 생성 (각각 파일 소유자, 소유 그룹, 일반 사용자에게 부여) (모두에게 권한 부여 : 777)
  - 다음과 같이 활용 가능하다. (예 mkdir -p dir1 dir2/dir2-1 dir2/dir2-2 dir3/dir3-1/dir3-1-1 )

8진수 | 2진수 | 권한 | 의미
-- | -- | -- | --
0 | 0 | --- | 아무 권한 없음
1 | 1 | --x | 실행 권한만 있음
2 | 10 | -w- | 쓰기 권한만 있음
3 | 11 | -wx | 쓰기,실행 권한 있음
4 | 100 | r-- | 읽기 권한만 있음
5 | 101 | r-x | 쓰기,실행 권한 있음
6 | 110 | rw- | 읽기,쓰기 권한 있음
7 | 111 | rwx | 모든 권한 있음

<br>

#### **rmdir (remove directory)**

- rmdir (remove directory) : 디렉터리 삭제
  - rmdir dir1 : dir1이라는 디렉터리를 삭제한다.
  - rmdir dir1 dir2 : 디렉터리 다중 생성
  - rmdir -p dir1/dir2 : 상위 디렉터리도 함께 삭제된다.

<br>

#### **rm (remove)**

- rm (Remove) : 파일 삭제
  - rm file1 : file1을 삭제
  - rm -f file1 : file1을 강제 삭제
  - rm -r dir : dir 디렉터리 삭제 (디렉터리는 -r 옵션 없이 삭제 불가, 하위 내용 포함 삭제)
  - rm -i dir : 파일마다 지울지 확인한다. 
  - 예시 ) rm -ri dir1 > y > y > y > ...

<br>

#### **cat (Catenate)**

- cat (Catenate) : 파일의 내용을 화면에 출력, 리다이렉션 기호('>')를 사용하여 새로운 파일 생성
  - cat file1 : file1의 내용을 출력
  - cat file1 file2 : file1과 file2의 내용을 출력
  - cat file1 file2 | more : file1과 file2의 내용을 페이지별로 출력
  - cat file1 file2 | head : file1과 file2의 내용을 처음부터 10번째 줄까지만 출력
  - cat file1 file2 | tail : file1과 file2의 내용을 끝에서부터 10번째 줄까지만 출력
  - '>' 기호 : 기존에 있는 파일 내용을 지우고 저장
  - '>>' 기호 : 기존 파일 내용 뒤에 덧붙여서 저장
  - '<' 기호 : 파일의 데이터를 명령에 입력
  - cat file1 firle2 > file3 : file1, file2의 명령 결과를 합쳐서 file3라는 파일에 저장
  - car file4 >> file3 : file3에 file4의 내용 추가
  - cat < file1 : file1의 결과 출력
  - cat < file1 > file2 : file1의 출력 결과를 file2에 저장

#### **cp (Copy)**

- cp (Copy) : 파일 및 디렉터리 삭제
  - cp file1 file2 : file1을 file2라는 이름으로 복사
  - cp -f file1 file2 : 강제 복사 (같은 이름이 있으면 강제 붙여넣기 진행)
  - cp -i file1 file2 : 복사할 대상 파일이 이미 존재할 때 덮어 쓸 것인지를 물어본다. (interactive)
  - cp -b file file2 : 덮어쓰거나 지울 때 백업본 파일을 만든다. (file2~가 생성된다)
  - cp -p file1 file2 : 소유권 허가권 시간정보를 유지 복사
  - cp -r dir1 dir2 : 디렉터리 복사. 폴더 안의 모든 하위 경로와 파일들을 복사한다.
  - 예) cp /etc/fstab .

<br>

#### **mv (move)**

- mv : 파일 또는 디렉터리의 이름을 바꾸거나 위치를 이동한다.
  - mv old_name new_name : old_name을 new_name로 변경한다.
  - mv -f : 묻지 않고 덮어 쓴다. (force)
  - mv -i : 덮어쓸지 묻는다.
  - mv -b : 파일 지우기 전에 백업본을 만든다.
  - mv file directory : 파일을 디렉터리로 옮긴다.

<br>



### 기타 명령어

#### **which : 명령어의 위치나 alias를 보여준다. 예) which ls -> bin/ls**

<br>

#### **whereis : 명령어의 소스, 실행 파일, 메뉴얼 페이지등의 위피를 알려준다.**

<br>

#### **file : 파일의 종류를 알아본다. ( 예 file file -> file : UTF-8 Unicode text )**

<br>

#### **clear : 화면 초기화**

<br>


#### **head**

- head : 파일의 첫 부분을 보여주는 명령. 텍스트 파일 앞에서 주어진 수 만큼의 행을 보여준다. (기본 10줄)
  - head -3 file : file의 내용 3행만큼 보여준다.

<br>

#### **tail**

- tail : head와 반대로 파일을 끝자리 부분을 보여준다. 주어진 개수만큼 줄을 버여준다.
  - tail -3 file : file의 내용 뒤에서 3행만큼 보여준다.
  - tail -3 -c file : 마지막 3바이트만 출력한다.
  - tail -f file : 특정 파일의 끝 부분에 새로운 행이 추가될 경우, 실시간으로 출력한다. (log를 볼 때 유용)

<br>

#### **more**

- more : 출력을 페이지 단위로 나누어 보여준다.
  - f, SPACE : 다음 페이지를 보여준다.
  - Enter : 한줄 씩 보여준다.
  - q, Q : 종료
  - b, ^B : 이전 페이지를 보여준다.
  - /검색어 : 검색어에 해당하는 단어를 검색한다.
  - = : 현재 line을 보여준다.
  - :f : 현재 파일의 이름과 현재 line number를 보여준다.
  - 예) more TNT cptest

<br>

#### **less**

- more의 상위호환 기능이다.

#### **wc**

- wc : 텍스트 파일의 행수, 단어수, 문자수를 알려준다.

<br>

#### **passwd**

- passwd : 유저의 패스워드를 변경한다.
  - passwd user : user의 패스워드를 변경한다.
  - passwd -l player : 유저의 계정을 잠근다.
  - passwd -d player : 유저의 페스워드를 삭제한다.
  - passwd -u player : 유저 계정의 잠금 상태를 해제한다.
  - passwd -n min : 패스워드에 변경가능 기한을 설정. min : 해당 일 수
  - passwd -x max : 패스워에 유효기간을 설정. max가 지난 후 패스워드 변경을 요구한다.
  - passwd -w warn : 패스워드 유효기간이 끝나기 warn일 전부터 메시지를 표시한다.

<br>

#### **group**

- group : 이용자가 속한 그룹들의 목록을 출력한다.

<br>

#### **who**

- who : 로그인 중인 유저를 표시한다.

<br>

#### **whoami**

- whoami : 현재의 실제 유저 ID의 유저명만을 표시한다.

<br>

#### **w**

- w : 현재 로그인 중인 유저의 정보를 표시한다.
  - w : 현재시간, 시스템 가동시간, 유저수 등등을 표시한다. 유저명, 터미널명, 로그인 호스트명, 로그인 시각, 실행중인 프로세스 등의 유저 정보를 표시한다. 
  - w user : user의 정보를 표시한다.
  - w -h user : 시스템 정보를 표시하지 않는다.
  - w -s user : 로그인의 시각과 프로세스 정보를 표시하지 않는다.
  - w -f user : 리모트 호스트명을 표시하지 않는다.

<br>

#### **chmod**

- chmod : 파일에 접근, 읽기, 실행 등의 허가권을 설정한다.
  - chmod a*rw test.txt
  - chmod 700 test.txt

<br>

#### **umask**

- umask : 새로운 파일이나 디렉토리 생성 시 기본 허가권 지정과 관련된 명령어이다.
  - umask : 현재 설정값을 본다.
  - umask -S : 현재 설정값을 문자로 표기한다. (u=rwx, g=rwx, o=rx)
  - umask 0352 : 0352로 허가권을 부여한다.
  - 기본적으로 파일이 생성될 때 보통 0666이라는 허가권을 요청한다. 

<br>

#### **cal**

- cal : 달력을 보여주는 명령이다.
  - cal : 현재 시스템의 날짜가 속한 달의 달력을 보여준다.
  - cal -j : 1월 1일부터 날짜수를 계산하여 출력한다.
  - cal -y : 올해의 달력을 표시한다.
  - cal 2006 : 2006년도 달력을 버여준다.
  - cal 5 2006 : 2006년도 5월 달력을 보여준다.

<br>

#### **date**

- date : 시스템의 날짜와 시간을 표시하거나 변경한다.
  - date -s 06:44 : 현재시간 변경

<br>

#### **hostname**

- hostname : 현재 설정되어 있는 호스트의 이름을 표시하거나 변경한다.
  - hostname [호스트이름] 

<br>

#### **dmesg**

- dmesg : 부팅시 커널에 출력되는 상태 정보를 볼 수 있도록 하는 프로그램이다.


<br>

#### **ps**

- ps : 현재 프로세스들의 상태를 PID(process ID)와 RP를 보여준다. 리눅스에서는 사용자, 파일, 프로세스도 번호로 관리할 수 있다.
  - ps -a : 다른 사용자에 의해 생선된 프로세스들도 보여준다.
  - ps -u : 프로세스의 소유자에 대한 정보를 자세히 보여준다.
  - ps -l : 프로세스의 정보들을 옆으로 길게 보여준다.
  - ps -x : 터미널 컨트롤과 관련이 없는 프로세스도 보여준다.
  - ps -e : 프로세스에 관련된 환경변수 정보를 함께 출력한다.
  - ps -f : 프로세스간에 상속관계를 보여준다.

<br>

#### **kill**

- kill : 프로세스에 특정한 signal을 보내는 명령이다. 보통 중지시킬 수 없는 프로세스를 종료시킬 때 사용한다.
  - kill option -시그널번호/시그널이름ID
  - kill -l : 시그널의 종류를 나열한다.
    - 15 SIGTERM : 가능한 정산 종료시키는 시그널로써, kill의 기본 시그널이다.
    - 1 SIGHUP(HUP) : 재시작
    - 2 SIGINT(INT) : 인터럽트 실행중지 (<kbd>Ctrl</kbd> + <kbd>c</kbd>와 동일)
    - 3 QUIT : 실행중지
    - 9 SIGKILL : 강제종료
    - 18 CONT : STOP에 의해 정지된 프로세스를 다시 실행시킨다. (countinue)
    - 19 STOP : 무조건적 정지
    - 20 TSTP : 실행 정지 후 다시 실행시키기 위해 대기시키는 시그널이다.
  - kill 724 : 724번 프로세스에 15번 시그널인 SIGTERM을 보낸다.
  - kill -9 756 757 758 : pid가 756, 757, 758 프로세스를 강제 종료(SIGKILL)한다.
  - kill -KILL PID 756 757 758 : (위와 동일)
  - kill -HUP 10118 : kill -1 10118와 동일하다.
  - kill %2 : 작업번호가 2인 프로세스를 종료시킨다.


<br>

#### ** **

<br>

#### ** **

<br>

#### ** **

<br>

#### ** **

<br>

### 

<br>

# 참조

- Linux 종류
  - https://www.leafcats.com/186
  - https://hanamon.kr/%EB%A6%AC%EB%88%85%EC%8A%A4%EB%8A%94-%EB%AC%B4%EC%97%87%EC%9D%B4%EA%B3%A0-%EC%9A%B0%EB%B6%84%ED%88%AC%EB%8A%94-%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80/
