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
  <img src="https://user-images.githubusercontent.com/66783849/190839639-86dab1b1-a015-49b0-a195-ea76f7e03170.png" width="50%">  
  <img src="https://user-images.githubusercontent.com/66783849/190839671-5b860f73-c6fa-4d52-bb8a-444d74e1e906.png" width="50%">

## 3. Linux 명령어

### 파일 생성

#### touch

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

#### vi

- vi

# 참조

- Linux 종류
  - https://www.leafcats.com/186
  - https://hanamon.kr/%EB%A6%AC%EB%88%85%EC%8A%A4%EB%8A%94-%EB%AC%B4%EC%97%87%EC%9D%B4%EA%B3%A0-%EC%9A%B0%EB%B6%84%ED%88%AC%EB%8A%94-%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80/
