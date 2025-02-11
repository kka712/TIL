# Git 기본 개념

## 분산버전 관리 시스템
- 클라이언트와 서버 모두가 똑같은 데이터를 유지하여 버전을 관리하는 시스템

## 파일의 세가지 상태

![areas](../assets/areas.png)

- 영역
    - working directory : 작성하고 있는 코드, 파일
    - staging area : add 명령어로 무대위로 올라간 파일들
    - git directory (repository) : commit 명령어로 찍힌 스냅샷들을 저장

## 파일의 라이프사이클
![lifecycle](../assets/lifecycle.png)

Tracked(관리대상임), Untracked(관리대상이 아님)
- Tracked 파일 : 이미 스냅샷에 포함돼 있던 파일이다. Tracked 파일은 또 Unmodified(수정하지 않음)와 Modified(수정함) 그리고 Staged(커밋으로 저장소에 기록할) 상태 중 하나이다. 간단히 말하자면 Git이 알고 있는 파일이라는 것이다.

그리고 나머지 파일은 모두 Untracked 파일이다. Untracked 파일은 워킹 디렉토리에 있는 파일 중 스냅샷에도 Staging Area에도 포함되지 않은 파일이다.