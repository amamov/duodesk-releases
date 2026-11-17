# DuoDesk 배포

아이폰으로 집 컴퓨터(Mac·Windows)를 원격으로 쓰는 DuoDesk의 호스트 설치 파일. 최신 파일은 [Releases](../../releases/latest)에 있다.

| 파일 | 설치할 곳 |
|---|---|
| `DuoDesk-Host-macOS.zip` | 호스트로 쓸 Mac |
| `DuoDesk-Host-Windows.exe` | 호스트로 쓸 Windows PC |

아이폰 앱은 TestFlight로 배포한다.

## 호스트 컴퓨터

**Mac**
1. Sunshine 설치: `brew install lizardbyte/homebrew/sunshine`
2. `DuoDesk-Host-macOS.zip`을 풀고 `DuoDesk Host.app`을 응용 프로그램 폴더로 옮겨 실행 (Apple 공증을 받아 바로 열린다)
3. 창에서 호스트 스위치를 켠다. 처음 연결할 때 시스템 설정 → 개인정보 보호 및 보안 → 화면 및 시스템 오디오 기록에서 sunshine을 허용한다
4. 밖에서도 쓰려면 '어디서나 연결'을 켜고 로그인한다

**Windows** (아직 시험 전)
1. `DuoDesk-Host-Windows.exe` 실행 → 트레이 아이콘에서 설정

## 아이폰

같은 Wi-Fi면 호스트가 자동으로 나타나고, 처음 연결할 때 아이폰에 뜨는 PIN을 DuoDesk Host에 입력한다.
