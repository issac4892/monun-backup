---
title: How to use Kotlin Plugin
description: Instructions on using Kotlin Plugin
published: true
date: 2021-06-09T19:35:49.344Z
tags: 
editor: markdown
dateCreated: 2021-06-09T19:35:49.344Z
---

# Kotlin Plugin

[Kotlin Plugin](https://github.com/monun/kotlin-plugin)은 Kotlin을 의존성으로 갖는 플러그인들을 위해 제작된 플러그인입니다.

여러가지 Kotlin 관련 라이브러리를 담고 있습니다.

이 플러그인이 있다면 본인의 플러그인에 Kotlin을 전부 담지 않아도 됩니다.

## 사용법

사용법은 간단합니다.

[Releases](https://github.com/monun/kotlin-plugin/releases)에서 자신의 Kotlin 버전에 알맞는 플러그인을 다운로드하시어 서버에 적용하시고,

본인 플러그인 depend 항목에 Kotlin 을 적어주면 됩니다.

```yaml
depend: [Kotlin]
```

### 라이브러리 목록:

- Kotlin Stdlib
- Kotlin Reflect
- Kotlinx Serialization Json
- Kotlinx Coroutines Core
- Kotlin Exposed (Core, Dao, Jdbc)
- etc...