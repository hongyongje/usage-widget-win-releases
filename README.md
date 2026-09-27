# 코딩 도구 사용량 위젯 — Windows 배포

Claude Code · Codex 의 사용 한도와 세션 상태를 바탕 화면 한쪽에 보여 주는 위젯의 **설치 파일과 자동 업데이트**를 내려받는 곳입니다. 소스 코드는 비공개 저장소에 있습니다.

## 설치

[최신 릴리스](https://github.com/hongyongje/usage-widget-win-releases/releases/latest)에서 `ClaudeUsageWidget-<버전>-Setup.exe` 를 받아 실행합니다.

- 관리자 권한이 필요 없고 사용자 폴더에 설치됩니다.
- .NET Framework 4.8 을 씁니다(Windows 10 1903 이후에는 기본으로 들어 있습니다).
- 이미 설치되어 있으면 그 위에 덮어 설치합니다. 설정과 기록은 그대로 남습니다.

## 자동 업데이트

설치된 위젯은 12시간마다 이 저장소의 최신 릴리스에서 `latest.json` 을 확인하고, 새 판이 있으면 알림을 띄웁니다. 알림을 누르면 받아서 설치 프로그램을 엽니다. 저절로 설치되지는 않습니다.

- `latest.json` — 버전 · 설치 파일 이름 · SHA-256 · 크기 · 릴리스 태그
- `latest.json.sig` — 위 파일에 대한 ECDSA P-256 서명
- 위젯에는 검증용 **공개키**만 들어 있습니다. 서명이 맞지 않는 매니페스트와, SHA-256 이 다른 설치 파일은 받아들이지 않습니다.

## 저작권

Copyright © 2026 Yong-Je Hong. All rights reserved.

본문 글꼴 Pretendard — Copyright (c) 2021, Kil Hyung-jin · SIL Open Font License 1.1.
