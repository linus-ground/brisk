# Brisk

가볍고 빠른 macOS용 RSS 리더. 이 저장소는 배포 전용이에요. 소스 코드는 없고, 설치 파일(DMG)은 [Releases](https://github.com/linus-ground/brisk/releases)에, 홈페이지와 업데이트 정보는 [GitHub Pages](https://linus-ground.github.io/brisk/)에 있어요.

## 필요 환경

- Apple Silicon(M1 이후) Mac, macOS 14 Sonoma 이상
- Intel Mac에서는 실행되지 않아요.

## 설치

1. [최신 릴리스](https://github.com/linus-ground/brisk/releases/latest)에서 `Brisk-x.y.z.dmg`를 받아 열어요.
2. Brisk를 '응용 프로그램(Applications)' 폴더로 끌어다 놓아요.
3. 응용 프로그램 폴더에서 Brisk를 실행해요.

## 업데이트

0.6.0부터는 앱이 하루 한 번 새 버전을 확인해서 알려 줘요([Sparkle](https://sparkle-project.org)). '업데이트 설치'를 누르면 알아서 바꾸고 다시 실행해요. 메뉴 막대 아이콘이나 Brisk 메뉴의 '업데이트 확인…'으로 바로 확인할 수도 있어요.

0.5.x에서는 한 번만 직접 바꿔 주세요.

1. 메뉴 막대의 Brisk 아이콘 → '종료' (창을 닫아도 메뉴 막대에서 계속 실행 중이에요)
2. 새 DMG의 Brisk를 '응용 프로그램' 폴더로 끌어다 놓고 '대치'
3. 다시 실행

구독 목록, 읽은 글, 설정은 업데이트해도 그대로 남아요.

## 라이선스

[PolyForm Noncommercial 1.0.0](LICENSE.md). 개인 사용, 공부, 연구, 비영리 단체 등 **비상업적 목적으로는 자유롭게** 쓰고 나눌 수 있어요. 상업적 목적(회사 업무용 도구, 유료 판매·서비스에 포함 등)으로는 쓸 수 없어요. 함께 들어 있는 오픈소스는 [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md)를 보세요.

## 저장소 구성

- `docs/index.html` — 홈페이지 (GitHub Pages)
- `docs/appcast.xml` — 앱이 읽는 업데이트 목록. 각 DMG의 EdDSA 서명이 들어 있어서, 서명이 맞지 않는 파일은 앱이 설치하지 않아요.
