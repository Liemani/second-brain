---
updated: "2026-06-09"
---
# macOS 화면 기록 자동화 검토

macOS에서 근무 시간 동안 주기적으로 화면을 자동 캡처하는 방식을 검토한 작업 기록이다.

## 결과

`launchd + shell script + screencapture` 구조는 현재 macOS 보안 정책 하에서 GUI 화면 캡처 자동화 방식으로 안정적으로 동작하지 않았다.

## 환경

- 적용 대상: `macOS 사용자 환경`
- 대상: `근무 시간대 주기 화면 캡처 자동화`
- 방식: `launchd + shell script + screencapture`

## 수행 절차

### 1. LaunchAgent 등록

1. `~/Library/LaunchAgents/com.user.screen_log.plist`를 준비했다.
2. `StartInterval=1800`으로 30분 간격 실행을 설정했다.
3. LaunchAgent 등록 및 실행 여부를 확인했다.

### 2. 스크립트 기본 문제 수정

1. Bash 주석 누락으로 발생한 syntax error를 수정했다.
2. 스크립트에 실행 권한을 부여했다.
3. 스크립트 자체가 실행 가능한 상태인지 확인했다.

### 3. 외부 볼륨 실행 문제 확인

1. 스크립트를 `/Volumes/mac/.environment/daemon/screen_log.sh`에 두고 실행을 시도했다.
2. `launchd`를 통해 실행했을 때 `Operation not permitted`가 발생했다.
3. 외부 볼륨의 스크립트 접근이 보안 정책에 의해 차단되는 것으로 판단했다.

### 4. 스크립트 위치 변경

1. 스크립트를 `~/.local/libexec/screen_log.sh`로 옮겼다.
2. 같은 구조에서 다시 실행을 시도했다.
3. `launchd`와 shell script 실행 자체는 정상화되었음을 확인했다.

### 5. `screencapture` 동작 분석

1. 터미널에서 직접 `screencapture -x file.jpg`를 실행해 정상 동작을 확인했다.
2. 같은 캡처를 `launchd` 경유로 실행했을 때 `could not create image from display`가 발생했다.
3. `launchctl asuser`, `launchctl bsexec loginwindow`, bash wrapper 제거를 각각 시도했지만 모두 동일하게 실패했다.

## 결과 상세

- 기대한 결과: 월요일부터 금요일까지 `09:00-18:00` 동안 30분 간격으로 화면이 자동 캡처되어 저장되기를 기대했다.
- 실제 결과: `launchd`와 shell script는 동작했지만, 실제 GUI 화면 캡처 단계인 `screencapture`에서 실패했다.
- 문제 또는 실패 원인 후보: 현재 macOS의 `TCC / Screen Recording` 권한 및 실행 컨텍스트 제약 때문에 `launchd` 하위 프로세스가 디스플레이 이미지를 생성하지 못하는 것으로 보인다.
- 다음 시도 아이디어: `launchd` 단독 구조 대신 사용자 세션과 더 밀접한 앱 기반 접근, 권한이 명확한 별도 실행 주체, 또는 다른 캡처 방식이 필요한지 검토한다.
