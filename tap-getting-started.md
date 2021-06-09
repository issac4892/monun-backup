---
title: Getting Started
description: 
published: true
date: 2021-06-09T19:27:00.166Z
tags: 
editor: markdown
dateCreated: 2021-06-09T04:19:27.061Z
---

# Getting Started
## `Tap`이란?
[Tap](https://github.com/monun/tap/)은 제가 제작한 여러 유용한 기능이 있는 라이브러리입니다.

#### 지원 기능
 * 개체 패킷
 * 가상 개체
 * 가상 발사체
 * 개체별 이벤트 리스너
 * YamlConfiguration을 이용한 문자열 템플릿
 * 추가적인 인벤토리 함수
 * GitHub를 통한 업데이트 (BETA)
 * Tick 기반 태스크 스케쥴러 (Ticker)

## 설치하기
> version 부분에는 monun/tap의 릴리즈 태그를 적어주시면 됩니다. (예: 3.4.2)

Groovy DSL
```groovy
allprojects {
    repositories {
        ...
        maven { url 'https://jitpack.io' }
    }
}

...
dependencies {
    implementation 'com.github.monun:tap:version'
}
```
\
Kotlin DSL
```kotlin
repositories {
    maven("https://jitpack.io")
}

...
dependencies {
    implementation("com.github.monun:tap:version")
}
```

> 플러그인 구현체는 [Releases](https://github.com/monun/tap/releases/latest) 에서 얻으 실 수 있으며, Tap의 의존성으로 [ProtocolLib](https://github.com/dmulloy2/ProtocolLib/releases/latest)와 [Kotlin Plugin](https://github.com/monun/kotlin-plugin/releases)이 필요합니다.

ProtocolLib은 [Jenkins 최근 성공 빌드](https://ci.dmulloy2.net/job/ProtocolLib/lastSuccessfulBuild/artifact/target/ProtocolLib.jar)에서 받으시면 편리하나, **언제나 불안정 할 수 있음**을 미리 알려드립니다.