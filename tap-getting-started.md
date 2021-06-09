---
title: Getting Started
description: 
published: true
date: 2021-06-09T04:19:27.061Z
tags: 
editor: markdown
dateCreated: 2021-06-09T04:19:27.061Z
---

# Getting Started
## `tap`이란?
tap은 monun님이 제작하신 여러 유용한 기능이 있는 라이브러리입니다.
## 설치하기
> Tag 부분에는 monun/tap의 릴리즈 태그를 적어주시면 됩니다. (예: 3.4.2)

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
    implementation 'com.github.monun:tap:Tag'
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
    implementation("com.github.monun:tap:Tag")
}
```