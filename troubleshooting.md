---
title: Troubleshooting
description: Minecraft Server Error & Gradle Build Error FaQ
published: true
date: 2021-06-08T02:35:33.973Z
tags: 
editor: markdown
dateCreated: 2021-06-08T02:35:26.622Z
---

# Troubleshooting
이 문서는 마인크래프트 서버 실행 시 + Gradle 빌드시 나오는 오류 메시지들에 대한 해결 모음입니다.

# ※ 질문 하기 전에 ※

Google과 같은 검색 사이트에서 직접 검색하여 먼저 문제를 찾아 보시는 것을 추천 드립니다.

관련된 내용을 무조건 GitHub Issue나 Discussion에 작성하지 마시고, `"오류내용이 이거와 관련해서밖에 나올 수 없다!"` 라고 생각하는 경우에 이슈를 달아 주시길 바라겠습니다.

---

# 마인크래프트 서버 오류 문제 해결

## Java Version Error:

오류 내용이

```
org.bukkit.plugin.InvalidPluginException: java.lang.UnsupportedClassVersionError: ~~~ has been compiled by a more recent version of the Java Runtime (class file version 55.0), this version of the Java Runtime only recognizes class file versions up to 52.0
```

와 비슷하거나 같은 경우, 자바 버전에 관련된 문제입니다. [Java Installation](https://monun.me/ko/java-installation) 문서를 확인하고 와주세요.

## Unknown Dependency:

오류 내용이
```
org.bukkit.plugin.UnknownDependencyException: Unknown dependency ~~~. Please download and install ~~~ to run this plugin.
```
와 비슷하거나 같은 경우, 의존성 플러그인이 누락된 문제입니다. 의존성 플러그인을 다운받아 주세요.

제가 제작한 의존 가능한 플러그인들은 [Tap](https://github.com/monun/tap/releases), [Kotlin](https://github.com/monun/kotlin-plugin/releases)등이 있으며, 다른 이들이 만든 의존성 플러그인들은 [WorldEdit](https://dev.bukkit.org/projects/worldedit/files), [ProtocolLib](https://github.com/dmulloy2/ProtocolLib/releases) 등이 있습니다.

---

# Gradle 빌드 오류 문제 해결

