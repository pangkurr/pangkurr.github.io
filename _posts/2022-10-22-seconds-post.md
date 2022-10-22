---
layout: post
title: notion post 1
image: 
date: 2022-10-22 p.m 3:46
tags: noition
categories: test
---

# Git 특징 및 설치, 환경설정

### GIT 기능(특징)

1. 버전관리
    - 문서를 수정할때마다 버전별로 기록이 가능해서 언제 어느것을 수정했는지 확인이 가능하다.
2. 백업
    - 작업중인 자료를 인터넷 상의 공간(원격 저장소)에 백업할 수 있다.
    - 대표적인 원격저장소로 **GitHub** 가 있다.
    - 보통 Git과 GitHub는 같이 사용한다.
3. 협업
    - 원격저장소 기준으로 여러 사람이 함께 작업이 가능하다.
    - 버전관리
4. 터미널 창에 직접 명령을 실행하는 CLI(Command Line Interface) 방식
    - 대부분의 개발자들이 선호한다.

다양한 Git 관련 프로그램

[GUI Clients](https://git-scm.com/downloads/guis)

## Git 설치방법 - windows  (아래 Mac 용 있음)

1. 사이트 접속

[Git](https://git-scm.com/)

1. 각 운영체제(windows, Mac 등)에 맞게 프로그램을 다운로드한다.

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/cca819c7-c98a-4092-af49-46c3f3f71ba8/Untitled.png)

1. [Git Bash] 찾아 실행

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/194304c1-8996-4a5a-bd49-b48bb0076423/Untitled.png)

1. `git --version` 명령어 입력 후 버전 정보가 나온다면 설치 완료

---

## Git 설치방법 - macOS

(사진 첨부는 못했습니다.)

1. 터미널 실행
2. [Homebew] 설치 (아래 사이트에서 코드 복사 붙여넣기 하시면 된다.)

[Homebrew](https://brew.sh/)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/dbf24e3a-ab2f-43cb-8b8f-053d040faefa/Untitled.png)

1. `brew` 명령어를 통해 설치 확인
2. `brew install git` 명령어 입력하여 git 설치
3. 이전에 설치 했었다면 `brew upgrade git` 명령어로 최신버전으로 업데이트
4. `git version` 설치 확인

## Git 환경설정 - Windows, macOS

```jsx
//이름설정
git config --global user.name "Your Name"
// 이메일 설정 (유출되도 상관없는 이메일(공적인 이메일 등)
git config --global user.email "you@your-email.com"
// 한글 출력 오류 방지
git config --global core.quotepath false

// 자모 분리 현상 방지 macOS 유저만, (혹시나 windows에서도 
//현상이 일어난다면 그때 적용)
git config --global core.precomposeunicode true
```
