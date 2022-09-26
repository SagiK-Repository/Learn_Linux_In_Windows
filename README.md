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

- 기초 명령어
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
  - echo : 한 줄을 표시한다.
- 기타 명령어
  - 파일
    - file : 파일의 종류를 알아본다.
  - 명령
    - which : 명령어의 위치나 alias를 보여준다. 예) which ls -> /bin/ls
    - whereis : 명령어의 소스, 실행 파일, 메뉴얼 페이지등의 위피를 알려준다.
    - man : 로컬 시스템상에서 여러 참고 문서들을 이용하여 특정 명령이나 자원들의 메뉴얼 출력명령 (man -f ls : ls 요약 설명)
    - whatis : man page의 이름과 개요를 보여주는 명령어로, "man -f"와 같다.
    - apropos : whatis DB를 검색하여 검색하는 명령어와 관련이 있는 명령어를 간단히 설명과 보여준다.
  - 화면
    - clear : 화면 초기화
  - 문서 보기
    - head : 앞에서 n줄 보여준다.
    - tail : 뒤에서 n줄 보여준다.
    - more, less : 페이지로 문서 보기
    - wc : 텍스트 파일의 행수(-l), 단어수(-w), 문자수(-c)를 알려준다. 가장 긴 라인(-L)
    - umask : 새로운 파일이나 디렉토리 생성 시 기본 허가권 
    - nl : 각 라인에 번호를 붙여 표준출력으로 보여준다.
    - pr : 표준 출력으로 파일을 재구성하거나 쓰기 위한 명령으로 문서 파일을 양식화 하는 도구로 사용된다.
    - tac : 파일의 내용을 맨 아래 줄부터 역순으로 출력하는 명령어이다. cat의 반대버전이다.
  - 사용자
    - passwd : 유저의 페스워드를 변경한다.
    - group : 이용자가 속한 그룹들의 목록을 출력한다.
    - who : 로그인 중인 유저를 표시한다.
    - whoami : 현재의 실제 유저 ID의 유저명만을 표시한다.
    - w : 현재 로그인 중인 유저의 정보를 표시한다.
    - users : 현재 시스템을 사용하는 사용자를 표시한다.
    - hostname : 현재 설정되어 있는 호스트의 이름을 표시하거나 변경한다.
    - id : 유저의 ID 정보를 표시한다.
    - finger : 유저의 정보(로그인 정보, 실명, 터미널명, 로그인 시각 등)를 표시한다.
    - chfn : 유저의 정보를 변경한다.
    - chage : 유저 계정의 패스워드 유효기간을 설정한다.
    - gpasswd : 그룹 이용자를 설정한다.
    - newgrp : 실효 그룹 ID를 변경한다.
    - logname : 현재 사용자의 로그인 유저명을 표시한다. (root 무상관)
    - last : 유저의 로그인 이력을 출력한다.
    - lastlog : 유저의 마지막 로그인 기록을 표시한다.
    - uptime : 현재 로그인한 후의 총 시간과 시스템 사용 현황을 보여 준다.
  - 부팅
    - dmesg : 부팅시 커널에 출력되는 상태 정보를 볼 수 있도록 하는 프로그램이다.
  - 프로세스
    - ps : 현재 프로세스들의 상태를 PID(process ID)와 RP를 보여준다. 리눅스에서는 사용자, 파일, 프로세스도 번호로 관리할 수 있다. (-u, -l, -e, -f)
    - pstree : 프로세스들의 계층적인 트리구조 형태로 출력한다.
    - kill : 프로세스에 특정한 signal을 보내는 명령이다. 보통 중지시킬 수 없는 프로세스를 종료시킬 때 사용한다.
    - nice : 프로세스의 우선순위를 변경하는 명령이다. 명령으로 NI값을 설정한다.
    - killall : 같은 데몬의 여러 프로세스를 한번에 종료한다.
    - top : 현재 시스템의 프로세스 상태를 실시간으로 화면에 보여준다.
    - jobs : 백그라운드로 실행중인 프로세스나 현재 중지된 프로세스의 목록을 출력해주는 명령어
    - renice : 실행중인 프로세스의 우선순위를 변결할 때 사용하는 명령이다.
    - pidof : 실행중인 특정 프로그램의 프로세스 ID를 출력한다.
    - pkill : 특정 프로세스에 signal을 보낸다.
    - fuser : 사용중인 프로세스의 소유자를 보여주거나 신호를 보낸다.
- 중급 명령어
  - 문서 가공
    - expand : space to tab (expend -t 3 filename)
    - expand : tab to space (unexpend -t 3 filename)
    - fmt : 간단한 문서 포맷도구로 문단의 들여쓰기 중복되는 공백문자 등을 처리할 수 있다. 
    - paste : 여러 파일의 해당 라인을 합친다. (paste, paste -s, paste -d 구분자)
    - split : 하나의 파일을 여러 개의 작은 파일로 분리하는 명령어이다. 
  - 파일 이상유무
    - pwck : 패스워드 파일의 이상 유무를 체크한다.
    - grpck : 그룹 파일의 이상 유무를 체크한다.
  - 동작
    - sleep : 잠쉬 쉬게 하는 명령어
    - clock : cmos에 설정된 시간이나 값을 보여주거나 변경한다.
  - 특정 동작
    - procinfo : /proc 디렉토리의 내용을 화면에 보여준다.
  - 환경
    - env : 프로그램을 다른 환경에서 실행한다.
    - source : 현재 셸 환경에서 주어진 파일을 읽어서 실행
  - 네트워크
    - stty : 터미널 라인 설정을 변화/출력
- 고급 명령어
  - 소유자
    - chown : 파일의 소유자를 바꾼다. (이 명령은 root가 아닌경우 제약이 많다.) (change owner)
    - chgrp : 파일의 소유그룹을 변경한다.
  - 특정 동작
    - watch : 화면에 출력하지 않고 프로그램을 주기적으로 실행한다.
    - makewhatis : 새로운 매뉴얼 페이지 추가시 관련 데이터 갱신 시켜주는 명령어이다.
    - info : man 명령처럼 특정한 명령어에 대한 매뉴얼 페이지를 보여주는 명령어이다.
    - uname : 시스템의 정보를 출력해주는 명령이다.
    - rdate : 원격으로 시간을 맞추어 주는 명령어이다.
  - 동기화
    - sync : 메모리를 디스크 자료와 동기화 한다.
  - 네트워크
    - reset : 터미널을 초기화한다.
    - ifconfig : 네트워크 인터페이스를 설정된다.
    - ping : 외부 네트워크와 연결이 정상적으로 이루어졌는지 확인하는 명령이다.
    - netstat : 네트워크의 상태, routing table, 인터페이스 통계등의 상태를 출력한다.
    - ftp : 인터넷 파일 전송 프로그램이다.
    - telnet : telnet TELNET 프로토콜을 이용한 사용자 인터페이스
    - rlogin : 원격 로그인을 한다.
    - rcp : 원격 파일 복사.
  - 메시지
    - mail : 시스템 사용자간의 홈 디렉토리(또는 /var/spool/mail/’사용자계정’)의 전자우편함을 두어서 그 곳을 통해서 메시지를 주고받을 수 있는 명령이다. 
    - mesg : Write를 사용해서 들어오는 메시지 수신 여부를 확인하고 제어하는 명령이다. 

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

#### **pstree**

- pstree : 프로세스들의 계층적인 트리구조 형태로 출력한다.
  - pstree
  - pstree -a : 각 프로세스의 명령행 인자까지 보여준다
  - pstree -h : 현재 프로세스와 조상 프로세스를 하이라이트로 강조해서 보여준다.
  - pstree -n : PID 값으로 정렬해서 보여준다.
  - pstree -p : PID 값을 같이 보여준다.

<br>

#### **nice**

- nice : 프로세스의 우선순위를 변경하는 명령이다. 명령으로 NI값을 설정한다.
  - NI 값은 -20 ~ 19가 존재한다. 값이 작을 수록 우선순위가 높다.
  - 일반 사용자는 NI값을 증가시킬 수 밖에 없고, 루트권한자는 값을 감소시켜 우선순위를 높일 수 있다.
  - nice -값 [ProcessName]
  - nice -10 bash : bash의 NI값을 10으로 변경시킨다.

<br>

#### **man**

- man : 로컬 시스템상에서 여러 참고 문서들을 이용하여 특정 명령이나 자원들의 메뉴얼 출력명령
  - man ls : ls 명령어의 메뉴얼 페이지를 보여준다.
  - man -k keyword : keyword 키워드가 발견되는 모든 메뉴얼의 내용을 검색하여 보여준다.
  - man -f keyword : keyword 레 대한 간략한 개요와 정보를 보여준다.
  - man -w keyword : 메뉴얼 페이지의 파일 위치를 보여준다.

<br>

#### **whatis**

- whatis : man page의 이름과 개요를 보여주는 명령어로, "man -f"와 같다.

<br>

#### **apropos**

- apropos : whatis DB를 검색하여 검색하는 명령어와 관련이 있는 명령어를 간단히 설명과 보여준다.
  - apropos jpeg : jpeg와 관련된 명령어 whatis와 같이 보여준다.

<br><br>

### 중급 명령어

#### **expand**

- expand : 일반적으로 설정되어 있는 탭(Tab)의 크기(8)를 원하는 공백(space)의 수로 바꾸어 화면에 출력하다.
  - Tab을 Space로 전환시켜준다. (수정x 표준출력o)
  - Tab의 크기는 8칸이다.
  - expand -t 3 tab : tab 문서 내부의 tab을 3개의 space로 변환

<br>

#### **unexpand**

- unexpand : 스페이스의 크기를 탭으로 전환시켜준다.
  - unexpand -a filename : 행의 시작부분의 공백 뿐만 아니라 모든 공백을 변환한다.
  - unexpand -t 3 filename : 지정한 공백크기를 하나의 Tab(8칸)으로 변환한다.

<br>

#### **cut**

- cut : 데이터의 열(column)을 추출할 때 사용한다.
  - cut -c 1-2 file : file의 첫 번째 필드 부터 두 번째 필드만 문자수로 따져 출력.
  - cut -f 1-10 file : file의 첫 번째 필드 부터 열 번째 필드만 필드수로 따져 출력.
  - cut -c 1-2 -d file : 필드 구분자를 짓는다.(-d, TAB)

<br>

#### **fmt**

- fmt : 간단한 문서 포맷도구로 문단의 들여쓰기 중복되는 공백문자 등을 처리할 수 있다. 
  - fmt filename : 
  - fmt -u filename : 중복되는 공백 문자를 모두 하나로 취급한다.
  - fmt -t filename : 단락의 처음 두 라인의 들여쓰기를 원래대로 유지한다.
  - fmt -w filename : 최대 라인 폭을 설정한다. w를 생략하고 -뒤에 직접 입력해도 된다.
  - fmt -w 10 filename

<br>

#### **nl**

- nl : 각 라인에 번호를 붙여 표준출력으로 보여준다.
  - nl filename : 라인을 붙여 출력
  - nl -s'구분자' file : 라인 번호와 문자열 사이에 '구분자' 설정

<br>

#### **paste**

- paste : 여러 파일의 해당 라인을 합친다.
  - 각 라인의 해당 라인을 연속적으로 출력하고, 새로운 라인 앞에서는 탭을 삽입한다.
  - paste file1 file2 : file1의 내용과 file2의 내용을 합친다. (a   b) o, (a<br>b) x 
  - paste -d 구분자 file1 file2 : 결합하는 라인의 구분자를 지정한다. 기본 값은 TAB 문자이다.
  - paste -s file1 file2 : 한 파일의 내용을 먼저 연속적으로 출력한 후, 다음 파일을 덧 붙여 출력한다. 

<br>

#### **pr**

- pr : 표준 출력으로 파일을 재구성하거나 쓰기 위한 명령으로 문서 파일을 양식화 하는 도구로 사용된다.
  - pr fimename : 표준출력
  - pr +'n' -'c' filename : 지정한 페이지(n)부터 출력(기본 1)하고 ,열의 수(c)만큼 출력한다.
  - pr -n filename : 라인 번호를 붙인다.
  - pr -d filename : 라인 사이를 한 라인씩 띄어 출력한다.
  - pr -h filename : 각 페이지의 헤더를 명시한다.
  - pr -l 라인 filename : 페이지의 길이를 '라인'수로 지정한다. (기본 66)
  - pr -m filename : 각 파일을 열대로 합쳐서 출력한다. (최대 8라인 합치기)
  - pr -w width filename : 라인 폭을 width에 지정한 수로 설정 (기본 27)

<br>

#### **split**

- split : 하나의 파일을 여러 개의 작은 파일로 분리하는 명령어이다. 
  - newfile을 지정하지 않으면 xaa, xab... 등과 같은 형태로 저장된다.
  - split filename newfile : 기본값 1000라인 단위로 filaname파일을 분리하여 newfile에 저장한다.
  - split -b 사이즈 filename newfile : 파일을 주어진 바이트 크기로 분리한다.
  - split -c 사이즈 filename newfile : 파일을 주어진 라인 크기에 맞도록 분리한다.
  - split -l 라인 filename newfile : 파일을 주어진 라인 수 단위로 분리한다.
  - split -넘버 filename newfile : -l 옵션을 사용한 것과 동일한 역할을 한다.


<br>


#### **tac**

- tac : 파일의 내용을 맨 아래 줄부터 역순으로 출력하는 명령어이다. cat의 반대버전이다.

<br>

#### **id**

- id : 유저의 ID 정보를 표시한다.
  - 실효유저ID/실효유저명, 실효그룹ID/실효그룹명, 소속그룹ID/소속그룹명에 대한 정보를 표시한다.
  - id User : User의 ID 정보를 표시한다.

옵션 | 의미
-- | --
-u | 실효 유저 ID를 표시한다.
-g | 실효 그룹 ID를 표시한다.
-G | 소속 그룹 ID를 표시한다.
-n | ID 대신 이름을 표시한다.   -u, -g, -G 옵션과 조합해 사용한다.
-r | 실효 ID 대신 실제 ID를 표시한다.   -u, -g 옵션과 조합해 사용한다.

<br>


#### **finger**

- finger : 유저의 정보를 표시한다.
  - 로그인 정보, 실명, 터미널명, 로그인 시각 등의 정보를 출력한다.
  - finger : 현재 로그인해 있는 유저들에 대한 정보를 보여준다.
  - finger User : User의 로그인 정보를 출력한다.
  -  


<br>

#### **chfn**

- chfn : 유저의 정보를 변경한다.
  - finger 명령어를 실행했을 경우 표시되는 유저 정보를 변경한다.
  - chfn [options] [user] 

<br>

#### **chage**

- chage : 유저 계정의 패스워드 유효기간을 설정한다.

옵션 | 의미
-- | --
-l | 유저의 패스워드 만기 정보를 보여준다.
-m mindays | 패스워드를 변경한 후 다시 변경할 수 있는 최소 일수(mindays)를 설정한다.
-M maxdays | 패스워드가 유효한 최대 일수(maxdays)를 설정한다.
-W warndays | 패스워드 만기일 이전에 유저에게 경고 메시지를 보일 일수(warndays)를 설정한다.
-E expiredate | 유저의 패스워드 만기일(expiredate)을 설정한다. 지정된   날짜 이후에는 해당 계정은 잠금 상태가 된다.

<br>


#### **gpasswd**

- gpasswd : 그룹 이용자를 설정한다.
  - 그룹의 패스워드 설정, 그룹 맴버 추가/삭제 설정에 사용된다.
  - 설정된 정보는 /etc/group, etc/gshadow에 저장된다.
  - 옵션없이 실행하면 대화형식으로 그룹 패스워드를 설정한다.

<br>

#### **newgrp**

- newgrp : 실효 그룹 ID를 변경한다.
  - 유저의 실효그룹ID를 유저가 속한 다른 그룹ID로 전환하는 명령어이다.
  - newgrp [group]

<br>


#### **pwck**

- pwck : 패스워드 파일의 이상 유무를 체크한다.
  - pwck [options] [passwd-file]
  - options
    - "-r" : 읽기 전용 모드로 실행한다.

<br>

#### **grpck**

- grpck : 그룹 파일의 이상 유무를 체크한다.
  - grpck [options] [group-file]
  - options
    - "-r" : 읽기 전용 모드로 실행한다.


<br>


#### **users : 현재 시스템을 사용하는 사용자를 표시한다.**

<br>

#### **logname**

- logname : 현재 사용자의 로그인 유저명을 표시한다. (root 무상관)
  - root에 상관없이 시스템에 로그인한 사용자의 유저명을 확인할 수 있다.

<br>

#### **last**

- last : 유저의 로그인 이력을 출력한다.
  - last [options] [user]
    - options
      - "-n" : n행만을 표시한다.
      - "-f file" : 로그인 로그파일을 저장한다.
      - "-x" : 시스템 셧 다운 및 런레벨 변경 사항을 표시한다.

<br>

#### **lastlog**

- lastlog : 유저의 마지막 로그인 기록을 표시한다.
  - last [options]
    - options
      - "-u user" : user의 마지막 로그인 정보만 표시한다.
      - "-t days" : 현재 시간으로부터 정해진 날짜 이내에 로그인한 사용자에 대해서 표시한다.

<br>

#### **sleep**

- sleep : 잠쉬 쉬게 하는 명령어
  - sleep [n] : n초만큼 대기
  - 기본시간은 초단위, 분(m), 시간(h), 날짜(d)도 가능하다.
  - 예) ls; sleep 5; ls
    - ls 출력 후 5초 뒤 다시 ls 출력한다.

<br>

#### **tty**

- tty : 현재 로그인 되어 있는 터미널의 장치 이름을 알려준다.

<br>

#### **clock**

- clock : cmos에 설정된 시간이나 값을 보여주거나 변경한다.
  - clock -w : cmos의 시간을 시스템 시간으로 저장

<br>

#### **killall**

- killall : 같은 데몬의 여러 프로세스를 한번에 종료한다.
  - killall [options] [프로세스명]
  - killall -w : 시그널을 받은 프로세스들이 종료될 때 까지 기다린다.
  - 예) killall httpd : Apache 웹서버 데몬을 모두 종료한다.
  - 예) killall -HUP httpd : httpd 데문을 다시 실행시킨다.

<br>

#### **top**

- top : 현재 시스템의 프로세스 상태를 실시간으로 화면에 보여준다.
  - top -l : 프로세스의 번호를 추가하여 보여준다.

<br>

#### **jobs**

- jobs : 백그라운드로 실행중인 프로세스나 현재 중지된 프로세스의 목록을 출력해주는 명령어
  - jobs -l : 프로세스 번호를 추가해서 보여준다.

<br>

#### **fg**

- fg : 백그라운드 프로세스를 포그라운드 프로세스로 전환하는 명령어이다.
  - fg %작업번호
  - 예) fg %2 : 작업번호 2번을 포그라운드로 전환한다.


<br>

#### **bg**

- bg : 포그라운드프로세스를 백그라운드 작업으로 전환하는 명령이다.
  - bg %작업번호
  - 프로세스를 실행한 후 <kbd>Ctrl</kbd>+<kbd>z</kbd>키를 눌러 작업을 잠시 중지시킨 후에 bg명령어를 이용하여 작업을 백그라운드로 보낼 수 있다.

<br>

#### **renice**

- renice : 실행중인 프로세스의 우선순위를 변결할 때 사용하는 명령이다.
  - 프로세스와 그 소유자와 루트 권한자만이 명령을 내릴 수 있다.
  - 명형도 NI값을 부여함으로써 수선순위가 변경되며, nice와 같이 -21~19 사이의 값을 부여한다.
  - renice options 값 PID
    - options
      - -r : 그룹의 ID 지정
      - -u : 사용자 ID 지정
      - -p : 프로세스 ID 지정

<br>

#### **nohup**

- nohup : 사용자가 로그아웃하거나 터미널 창을 닫아도 해당 프로세스를 백그라운드로 작업될 수 있도록 해주는 명령어이다.
  - nohup [명령]

<br>

#### **pidof**

- pidof : 실행중인 특정 프로그램의 프로세스 ID를 출력한다.
  - pidof 프로그램명
  - 예) pidof httpd

<br>

#### **uptime**

- uptime : 현재 로그인한 후의 총 시간과 시스템 사용 현황을 보여 준다.

<br>



#### **procinfo**

- procinfo : /proc 디렉토리의 내용을 화면에 보여준다.

<br>

#### **echo**

- echo : 한 줄을 표시한다.
  - echo -n wow : 마지막에 개행문자 없이 wow를 출력한다.
  - echo -e wom : 문자열에서 다음 백슬래시로 이스테이프된 문자의 번역을 하도록 한다.

<br>

#### **env**

- env : 프로그램을 다른 환경에서 실행한다.
  - env[-]  [-i] [-u   name] [--ignore-environment] [--unset=name] [--help] [--version] [name=값]... [명령 [인수...]] 
  - [options]
    - -u : 만약 존재한다면 환경으로부터 name 변수를 제거한다.
    - -i, - : 상속된 환경을 무시하고 텅 빈 환경에서 시작한다.

<br>

#### **source**

- source : 현재 셸 환경에서 주어진 파일을 읽어서 실행
  - source filename : 파일을 읽어서 실행한다.

<br>

#### **stty**

- stty : 터미널 라인 설정을 변화/출력
  - stty [-a,--all,-g,--help,--save,--version] 


<br>

#### **pkill**

- pkill : 특정 프로세스에 signal을 보낸다.
  - pkill [-signal] [-fnvx] [-P ppid,...] [-g pgrp,...]  [-s sid,...] [-u euid,...] [-U uid,...] [-G  gid,...] [-t term,...] [pattern] 


<br>

### 고급 명령어

#### **chown**

- chown : 파일의 소유자를 바꾼다. (이 명령은 root가 아닌경우 제약이 많다.) (change owner)
  - chown [options] [newowner] file(s)
    - [options]
      - -R : 서브 디렉토리까지 설정된다.

<br>

#### **chgrp**

- chgrp : 파일의 소유그룹을 변경한다.
  - chown [option] newgorup file(s)
    - [options]
      - -R : 서브 디렉토리까지 설정된다.


<br>

#### **watch**

- watch : 화면에 출력하지 않고 프로그램을 주기적으로 실행한다.
  - watch [-dhv] [-n  <seconds>]  [--differences[=cumulative]] [--help] [--interval=<seconds>] [--version] <command> 
    - [options]
      - -n : 인터벌을 주기로 프로그램을 실행시킨다.


<br>

#### **sync**

- sync : 메모리를 디스크 자료와 동기화 한다.

<br>


#### **reset**

- reset : 터미널을 초기화한다.
  - reset [-IQVqrs] [-] [-e ch] [-i ch] [-k ch]  [-m  mapping]  [terminal] 

<br>

#### **ifconfig**

- ifconfig : 네트워크 인터페이스를 설정된다.
  - ifconfig [ interface ] 
  - ifconfig eth0 : Eth0로 지정된 네트워크 장치의 IP address, NetMask, Broadcast 등의 정보를 출력한다.
  - ifconfig eth0 down : 현재 장동중인 네트워크 장치 eth0를 중지한다.
  - ifconfig eth0 210.119,33,193 netmask 255.255.255.0 up
    - IP address를 210.119.33.193로 부여하고, Netmask 는 255.255.255.0을 사용하도록 eth0을 활성화


<br>

#### **ping**

- ping : 외부 네트워크와 연결이 정상적으로 이루어졌는지 확인하는 명령이다.
  - ping -b 192.168.1.255 : Broadcast에 packet을 전송한다.
  - ping -c 3 192.168.0.1 : Host에 packet를 3번 전송한다.
  - ping -i 2 192.168.10.12 : Host에 packet을 전송하되, 간격은 2초에 한 번씩으로 설정한다.

<br>

#### **netstat**

- netstat : 네트워크의 상태, routing table, 인터페이스 통계등의 상태를 출력한다.
  - [options]
    - -r : routing table을 출력한다.
    - -i : 모든 네트워크 인터페이스 정보를 출력한다.
    - -n : 주소를 숫자로 출력한다.
    - -p : PID와 프로그램 이름을 출력한다.
    - -ㅣ : listening 상태인 소켓 정보만 출력한다.
    - -a : listening & non listening 소켓 모두 출력한다.
    - -u : udp 프로토콜을 사용하는 소켓만 출력한다.
    - -t : tcp 프로토콩을 사용하는 소켓만 출력한다.
    - netstat -vattcp : 프로토콜을 사용하는 서비스들과 그 상태를 출력한다.
    - netstat -vauudp : 프로토콜을 사용하는 서비스들과 그 상태를 출력한다.
    - netstat –taptcp : 프로토콜을 사용하는 서브스들과 그 상태, PID, 프로그램 이름정보를 출력한다.
    - netstat –rn : route –n 명령과 비슷한 결과를 출력

<br>

#### **ftp**

- ftp : 인터넷 파일 전송 프로그램이다.
  - ftp [-pinegvd] [host] 
  - 예) ftp ubilab.sunmoon.ac.kr

<br>

#### **telnet**

- telnet : telnet TELNET 프로토콜을 이용한 사용자 인터페이스 
  - telnet [-d] [-a] [-n  추적파일] [-e escape문자] [[-l 사용자ID] 호스트 [포트]] 
  - 예) telnet ubilab.sunmoon.ac.kr

<br>

#### **rlogin**

- rlogin : 원격 로그인을 한다.
  - rlogin [-8EKLdx] [-e char] [-l username] host 
  - -l : 다른 id를 사용하여 로그인하기 위해서는 -l 옵션을 사용한다.

<br>

#### **rcp**

- rcp : 원격 파일 복사
  - rcp [-px] file1 file2 
  - rcp [-px] [-r] file ... directory 
  - [options]
    - -p : 원본 파일의 변경날짜와 모드를 유지하여 복사한다.
    - -x : 호스트 간의 모든 정보 전달을 DES 암호화한다.
    - -r : 디렉토리 내의 하위 디렉토리와 파일을 로컬 시스템으로 복사한다.
    - -D : 지정한 포트로 접속한다.


<br>

#### **fuser**

- fuser : 사용중인 프로세스의 소유자를 보여주거나 신호를 보낸다.
  - fuser [option] 디렉토리명 
  - [options]
    - -V : fuser 명령의 버전을 보여준다.
    - -l : fuser 명령에서 사용하는 시그널목록을 보여준다.
    - -v : 프로세스를 PID, USER, ACCESS, COMMAND 등의 형식으로 보여준다.
    - -k : KILL 시그널을 보낸다.
    - -m : 특정파일, 마운트된 파일시스템, 블록장치 등에게 신호를 보낼 때 k옵션과 같이 쓰인다.


<br>

#### **makewhatis : 새로운 매뉴얼 페이지 추가시 관련 데이터 갱신 시켜주는 명령어이다.**

<br>

#### **info**

- info : man 명령처럼 특정한 명령어에 대한 매뉴얼 페이지를 보여주는 명령어이다.
  - 제공되지 않는 명령어도 존재한다.
  - 예) info mkdir

<br>

#### **uname **

- uname : 시스템의 정보를 출력해주는 명령이다.
  - OS의 버전이나 vender, machine type등을 알 수 있다. 
  - [Opetions]
    - ‐m : 시스템의 hardware이름을 알려준다. arch명령과 같다.
    - ‐n : 네트워크상의 nodename을 알려준다. 일반적으로 호스트 네임을 말한다.
    - ‐r : OS의 release를 알려준다.
    - ‐s : 시스템 이름을 알려준다. 옵션 없이 실행시킨 것과 같다.
    - ‐p : 프로세서의 타입을 알려준다.
    - ‐v : OS의 버전을 알려준다. 커널의 생성날짜이다.
    - ‐a : 위의 모든 정보를 보여준다.

<br>

#### **rdate**

- rdate : 원격으로 시간을 맞추어 주는 명령어이다.
  - 다른 서버의 시간을 참조하여 표준시간으로 설정하는 명령이다. 
  - 이 명령어는 해당서버의 NTP(Network Time Protocol)서버시간을 참조한다. 
  - rdate option 원격지 서버
  - [options]
    - -p : 원격지서버의 시간을 출력해준다.
    - -s : 원격지서버의 시간을 시스템의 시간으로 설정한다.
  - 예) rdate -s time.bora.net


<br>

#### **mail**

- mail : 시스템 사용자간의 홈 디렉토리(또는 /var/spool/mail/’사용자계정’)의 전자우편함을 두어서 그 곳을 통해서 메시지를 주고받을 수 있는 명령이다. 
  - mail [option] [IDs] (여러개 아이디 가능) 
    - [options]
      - 
      - -r : [메시지 번호]	메일을 보낸 사람에게 답장을 쓴다.
      - -d : [메시지 번호]	메일을 삭제한다.
      - -n : 다음차례의 메일을 보여준다.
      - -q : 메일확인상태에서 빠져 나온다.
      - -pre : 메일상태를 확인한 뒤 /user/spool/mail로 보낸다.
      - -s : 파일이름	메일의 내용을 파일로 저장한다.
      - -visual : 메일의 내용을 편집하여 저장할 때 사용한다. vi 편집기를 사용할 수 있다.
  - main 전송 : "mail freedom" > 내용 입력
  - main 입력시 메일 확인을 할 수 있다.


<br>

#### **mesg**

- mesg : Write를 사용해서 들어오는 메시지 수신 여부를 확인하고 제어하는 명령이다. 
  - mesg [n/y]
  - mesg n : 비수신 상태
  - mesgis n : 현대 상태는 메시지 비수신 상태이다.
  - mesg y : 수신 상태
  - mesgis y : 현대 상태는 메시지 수신 상태이다.

<br>

#### ** **

<br>

#### ** **

<br>

#### ** **

<br>

#### ** **

<br>

## 4. Linux 파일과 디렉토리

- 파일 경로
  - 파일 경로는 루트 디렉터리인(절대경로) "/"에서 시작하여 특정 파일이나 디렉터리를 표시한다.
  - 홈 디렉터리 : 일반 사용자가 자신만의 파일들을 관리하기 위해 사용하는 디렉터리("~")이다.
    - 홈 디렉터리는 "echo $HOME"명령을 입력하여 확인한다.
- 디렉터리 작업
  - 명령은 다음 방법을 통해 입력된다.
    - $ 명령 [옵션] [인수]
      - 명령 : 수행하고자 하는 UNIX 명령
      - 옵션 : 명령 수행에 필요한 선택사항
      - 인수 : 명령을 수행하는데 필요한 정보
  - 현재 디렉터리 : "pwd"명령어를 통해 확인한다.
  - 디렉터리 변경 : "cd"명령어를 통해 변경한다.
  - 특수 경로
    - "." : 현재 작업 디렉터리
    - ".." : 상위 작업 디렉터리
    - "~" : 사용자 홈 디렉터리
- 디렉터리 내용 확인
  - 현재 디렉터리 내용 확인은 "ls" 명령어를 통해 이루어진다.
    - ls file : 파일 이름이나 디렉터리의 내용을 확인한다.
      - -F : 파일의 타입을 표시
      - -l : 파일의 크기 및 권한에 대한 정보 표시
      - -a : "."을 포함한 파일까지 모두 출력
      - -R : 하위 디렉터리의 내용을 제귀적으로 호출
  - 사용 권한
    - r : 읽기 권한
    - w : 쓰기 권한
    - x : 실행 권한
    - \- : 해당 권한 없음
  - 메뉴얼 페이지 사용은 "man"을 통해 이루어진다.
    - man ls : ls 명령에 대한 메뉴얼 페이지를 출력
    - man -k calendar : calendar와 관련된 명령어 출력
- 파일 링크 관리
  - "In"을 통해 파일의 링크를 생성한다.
    - In /etc/passwd passwd : /etc/passwd 파일을 passwd로 링크시킨다.
  - 하드링크
    - 하나의 파일에 여러 개의 링크를 생성한다.
    - 존재하지 않는 파일에 대해 심볼릭링크 파일을 작성할 수 없다.
    - 연결되어 있는 파일이 어떤 파일인지 알기 어렵다.
    - 같은 파일 시스템간에서만 작성할 수 있다.
      - ls -i unix : unix 파일의 아이노드를 확인한다. (8913092)
      - In unix linux : unix 파일에 대해 하드링크 작성
      - ls -i uinx linux : 두 파일의 아이노드가 같음을 확인한다. (8913092)
  - 심볼릭 링크(Symbolic link)
    - 파일에 또 다른 이름이 부여하지만, 하드링크처럼 아이노드에 링크되지 않는다.
    - 존재하지 않는 파일에 대해 심볼릭 링크 파일을 작성할 수 있다.
    - 커널에 의해 처리된다.
    - 연결되어 있는 파일을 찾기 쉽다.
    - 다른 파일 시스템간에 작성할 수 있다.
      - In -s car pen : car 라는 파일에 대해 심볼릭 링크 작성
      - ls -i car pen : 아이노드 번호가 다르다.
- 사용자권한 자동 부여
  - 사용자가 파일을 만들면 자동으로 파일의 접근권한이 부여된다.
  - 파일 작성 마스크("mask")를 사용하여 접근권한을 수정한다.

## 5. Linux 사용권한과 시스템 보호

- 파일 사용 권한
  - Unix 시스템은 멀티유저 시스템이다.
  - 한 사용자의 사용이 다른 사용자에게 피해가 되지 않도록 보호장치를 마련해 놓았다.
    - 읽기 권한 : 파일 또는 디렉터리의 내용을 볼 수 있다.
    - 쓰기 권한 : 파일 내용 수정 또는 디렉터리 내 새파일 생성 가능하다.
    - 실행 권한 : 파일을 실행 또는 디렉터리로 이동할 수 있다.
  - "chmod"를 통해 파일 사용권한을 설정할 수 있다.
    - chmod u+wx linux
    - chmod a-x linux

################ ppt 26~

###

# 참조

- Linux 종류
  - https://www.leafcats.com/186
  - https://hanamon.kr/%EB%A6%AC%EB%88%85%EC%8A%A4%EB%8A%94-%EB%AC%B4%EC%97%87%EC%9D%B4%EA%B3%A0-%EC%9A%B0%EB%B6%84%ED%88%AC%EB%8A%94-%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80/
