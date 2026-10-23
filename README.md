# 2026-2학기 DevOps

2026-2학기 DevOps 수업에 관한 내용입니다.  
(This repository contains materials for the DevOps course in the second semester of 2026.)

수업에 대한 내용은 각 주차별 폴더의 README.md에서 확인하실 수 있습니다.  
(You can find the course materials in the README.md file in each week's folder.)

---

## 주차별 내용 (Weekly Course Content)

- `[1주차 - 오리엔테이션]`
- `[2주차 - 실습 환경 구축과 버전 관리 기초](test, week02)`
- `[3주차 - 셸 스크립팅](week03)`
- `[4주차 - 자동화와 협업, 네트워크](week04)`
- `[5주차 - 도커](week05)`
- `[6주차 - 도커파일](week06, guestbook)`
- `[7주차 - 도커 컴포즈](week07)`

---

## 리눅스 기본 명령어 (Basic Linux Commands)

### 디렉터리 및 파일 관리

- **`mkdir <디렉터리 이름>`**: 새 디렉터리 만들기 (make directory)
- **`cd <디렉터리 이름>`**: 디렉터리 이동 (change directory)
  - `~`: 홈 디렉터리로
  - `..`: 상위 디렉터리로
  - `-`: 직전 작업하던 디렉터리로
- **`pwd`**: 현재 디렉터리 확인 (print working directory)
- **`ls`**: 파일/폴더 목록 확인 (list)
  - `-a`: 숨김 파일까지 모두 보여주기
- **`rmdir <디렉터리>`**: 빈 디렉터리 삭제 (디렉터리가 비어있을 때만 삭제 가능)
- **`touch <파일>`**: 빈 파일 생성 (create empty file)
- **`echo "내용" > <파일>`**: 파일에 내용 삽입 (insert file contents)
- **`nano <파일>`**: 텍스트 파일 생성 후 작성
- **`cp <원본파일> <복사파일>`**: 파일 복사 (file copy)
- **`mv <파일><파일>`**: 파일 이동 (move file)
- **`rm <파일>`**: 파일 삭제 (delete file)
  - `-rf`: 경고 없이 전부 삭제

### 파일 내용 확인

- **`cat <파일명>`**: 파일 내용 확인 (check file contents)
- **`less <파일명>`**: 긴 파일 내용 보기 (read large file)
- **`head <파일명>`**: 앞 부분만 보기 (read file header)
- **`tail <파일명>`**: 뒷 부분만 보기 (read file tail)

### 권한 및 사용자

- **`chmod <권한> <파일이름>`**: 권한 수정 방법 (chmod: change mode)
- **`whoami`**: 현재 활성화된 사용자명 (user name)

### 시스템 관리

- **`df -h`**: 디스크 사용량 (disk usage)
- **`clear`**: 화면 정리 (clear terminal screen)

### 명령어 기록

- **`history`**: 입력했던 명령어 (display command history)
- **`!<숫자>`**: 히스토리 확인 후, `<숫자>`번째 명령어 실행 (execute `<number>` from command history)
  - `!<숫자>:p`: `<숫자>`번째 명령어 확인
  - `!!`: 바로 직전 명령 다시 실행

