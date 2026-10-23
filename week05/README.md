## 5주차 (Week 5)

---

### 오늘 배운 내용 (What I Learned)

- 하이퍼바이저(VM) 방식 vs 컨테이너 방식
- 이미지 vs 컨테이너
- 프로그램 vs 프로세스
- GitHub 이슈 기반 작업 흐름

### 주요 단어 (Key Terms)

- **Docker**: 애플리케이션을 개발(develop), 배포(ship), 실행(run)하기 위한 오픈 플랫폼, 서로 다른 환경에서도 비교적 동일하게 실행할 수 있도록 도와주는 플랫폼
- **Image**: 컨테이너를 만들기 위한 읽기 전용 템플릿
- **Container**: 이미지로부터 생성된 인스턴스
- **Dockerfile**: 이미지를 어떻게 만들지 작성하는 파일
- **Registry**: 이미지를 저장 및 공유하는 곳, ex) Docker Hub

### 주요 코드 (Key Code)

- **`docker ps`**: 실행 중인 컨테이너 출력
  - `-a`: 모든 컨테이너 출력
- **`docker images`**: 내려받은 이미지 목록 보기
- **`docker logs <컨테이너명>`**: 로그 보기
  - `-f`: 실시간으로 확인
- **`docker stop <컨테이너명>`**: 정지
- **`docker start <컨테이너명>`**: 실행
- **`docker rm <컨테이너명>`**: 삭제
  - `-f`: 실행 중이어도 삭제

### Issue부터 Merge까지의 과정 요약

`Issue → Branch → 기록 → Commit/Push → PR → Merge → Issue Close`

### curl 실행 결과

- **실행 명령어**: `curl http://localhost:8091`
  - **결과**:
    ```html
    <h1>Welcome to nginx1</h1>
    ```

- **실행 명령어**: `curl http://localhost:8092`
  - **결과**:
    ```html
    <h1>Welcome to nginx2</h1>
    ```

- **실행 명령어**: `curl http://localhost:8093`
  - **결과**:
    ```html
    <h1>Welcome to nginx3</h1>
    ```
