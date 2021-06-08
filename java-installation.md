---
title: Java Installation
description: Java Installation Guide
published: true
date: 2021-06-08T04:46:48.684Z
tags: 
editor: markdown
dateCreated: 2021-06-08T02:08:12.642Z
---

# Java Installation

## 안내 사항

자바 버전 오류 관련되어서 이 문서로 오게 되었거나, 혹은 자바 설치 법을 몰라서 이 문서를 직접 찾아오셨다면, 잘 오셨습니다.

이 문서에서는 자바를 설치하는 내용을 안내하고 있습니다.

[PaperMC](https://papermc.io/)의 [Java 8](https://papermc.io/java16) 버전 지원 중단 공지와 관련된 이유로 JDK 16 기준으로 설명 함을 알려드립니다.

---

## 경고!

JDK 16 버전을 설치함으로써 환경변수가 자동으로 설정 될 수 있고 그로 인해 원래 작업하시던 내용에 영향을 미칠 수 있습니다.

이 점 유의하시어 진행을 해 주시길 바랍니다.

(참고: JDK16을 이용하지 않을 시 개발된 플러그인 및 라이브러리의 사용이 제한 될 수 있습니다.)

---

Oracle에서 직접 지원하는 안정적인 [Oracle JDK 16](https://www.oracle.com/java/technologies/javase-jdk16-downloads.html)를 설치 하거나,

GPL 라이선스로 제공되는 OpenJDK를 다운로드 할 수도 있습니다.

이 문서에서는 GPL 라이선스를 사용하는 OpenJDK를 기준으로 설치를 설명합니다.

# OpenJDK 설치

---

## Windows

> OJDKBuild에서 다운로드: [여기](https://github.com/ojdkbuild/ojdkbuild/)로 접속해 README.md에 있는 .msi를 실행하면 됩니다.

> AdoptOpenJDK에서 다운로드: [여기](https://github.com/AdoptOpenJDK/openjdk16-binaries/releases)로 접속해 Assets에 있는 .msi를 설치하시면 됩니다.

> [Chocolatey](https://chocolatey.org/)를 이용하여 AdoptOpenJDK를 설치 할 수 있습니다. 명령은 다음과 같습니다:

```
choco install adoptopenjdk16
```

---

## macOS

HomeBrew를 사용하여 AdoptOpenJDK에서 다운로드 합니다.

```
brew tap AdoptOpenJDK/openjdk
brew install --cask adoptopenjdk16
```

- `brew cask install` 은 Deprecated 되었습니다. [참고](https://brew.sh/2020/12/01/homebrew-2.6.0/)

---

## Linux

#### Debian 계열 Linux 환경 (apt 사용)

```shell
sudo add-apt-repository ppa:openjdk-r/ppa
sudo apt update
sudo apt install openjdk-16-jre
```

#### 이외 Linux 환경

```shell
wget https://download.java.net/java/GA/jdk16.0.1/7147401fd7354114ac51ef3e1328291f/9/GPL/openjdk-16.0.1_linux-x64_bin.tar.gz
tar xvzf openjdk-16.0.1_linux-x64_bin.tar.gz

# 아래의 내용을 /etc/profile 이나 ~/.bashrc 에 추가하셔서 자동으로 적용되게 해주세요.

export JAVA_HOME=(자바 경로)
export PATH=$JAVA_HOME/bin:$PATH

source ~/.zshrc # bash 사용시 ~/.bashrc, ~/.bash_proile
```

#### Linux Global Environment

```shell
$ sudo echo "export JAVA_HOME=(자바 경로)" >> /etc/environment # you can use /etc/profile instead of /etc/environment
$ sudo echo "export PATH=$JAVA_HOME/bin:$PATH" >> /etc/environment # you can use /etc/profile instead of /etc/environment
$ sudo reboot # do not use -f option
```

재부팅 하신 이후 ``java -version``으로 버전을 확인하세요.

이외의 JDK 바이너리 파일들은 https://jdk.java.net/ 에서 확인 가능합니다.