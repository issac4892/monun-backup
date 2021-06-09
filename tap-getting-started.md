---
title: Getting Started
description: 
published: true
date: 2021-06-09T09:13:56.966Z
tags: 
editor: markdown
dateCreated: 2021-06-09T04:19:27.061Z
---

# Getting Started
## `tap`이란?
tap은 제가 제작한 여러 유용한 기능이 있는 라이브러리입니다.

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