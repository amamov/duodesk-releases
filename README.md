# DuoDesk 배포

아이폰으로 집 컴퓨터(Mac·Windows)를 원격으로 쓰는 DuoDesk의 설치 파일. 최신 파일은 [Releases](../../releases/latest)에 있다.

| 파일 | 설치할 곳 |
|---|---|
| `DuoDesk-iOS.ipa` | 아이폰 (DuoDesk 앱) |
| `DuoDesk-Host-macOS.zip` | 호스트로 쓸 Mac |
| `DuoDesk-Host-Windows.exe` | 호스트로 쓸 Windows PC |

## 1. 호스트 컴퓨터

**Mac**
1. Sunshine 설치: `brew install lizardbyte/homebrew/sunshine`
2. `DuoDesk-Host-macOS.zip`을 풀고 `DuoDesk Host.app`을 응용 프로그램 폴더로 옮겨 실행
3. 창에서 호스트 스위치를 켠다. 처음 연결할 때 시스템 설정 → 개인정보 보호 및 보안 → 화면 및 시스템 오디오 기록에서 sunshine을 허용한다
4. 밖에서도 쓰려면 '어디서나 연결'을 켜고 로그인한다

**Windows** (아직 시험 전)
1. `DuoDesk-Host-Windows.exe` 실행 → 트레이 아이콘에서 설정

## 2. 아이폰

`DuoDesk-iOS.ipa`는 개발용 서명이라 **등록된 기기에만** 설치된다. Mac에 아이폰을 USB로 연결하고:

```bash
xcrun devicectl device install app --device <기기 UDID> DuoDesk-iOS.ipa
```

또는 Apple Configurator / Finder에 IPA를 끌어다 놓는다. 새 아이폰은 개발자 계정에 기기 등록 후 다시 빌드해야 한다.

같은 Wi-Fi면 호스트가 자동으로 나타나고, 처음 연결할 때 아이폰에 뜨는 PIN을 DuoDesk Host에 입력한다.

소스: [amamov/duodesk](https://github.com/amamov/duodesk) (private, GPLv3)
