## 6주차 (Week 6)

---

### 오늘 배운 내용 (What I Learned)

- Dockerfile
- 레이어와 캐시
- 배포

### 주요 단어 (Key Terms)

- **Dockerfile**: 이미지를 만드는 레시피

### 내 이미지 주소

`ghcr.io/hikicrash/guestbook:v2`

### 친구 이미지를 실행한 결과

![친구 이미지 실행 결과](https://github.com/user-attachments/assets/9be6847d-5b43-4d48-b3dc-0edd29b7ef75)

### Dockerfile의 각 줄이 하는 일

```dockerfile
FROM python:3.12-slim
# 파이썬이 준비된 이미지를 기반으로 시작한다.

WORKDIR /app
# 컨테이너에서 사용할 디렉터리의 경로를 설정한다.

COPY requirements.txt .
# 파일을 복사한다.

RUN pip install --no-cache-dir -r requirements.txt
# txt파일에 적힌 라이브러리를 설치한다.

COPY . .
# /app으로 현재 디렉터리의 폴더와 파일을 전부 복사한다.

RUN useradd -m appuser
# 컨테이너에서 사용할 계정을 만든다.

USER appuser
# 실행 사용자를 변경한다.

ENV APP_TITLE="InhaTC DevOps 방명록" \
    THEME_COLOR="#0054A6"
# 환경 변수를 설정한다.

EXPOSE 5000
# 포트 정보를 지정한다.

CMD ["python", "app.py"]
# 컨테이너가 시작할 때 기본으로 실행하는 명령어를 설정한다.
```

### 빌드 캐시가 동작한 로그 (CACHED)

![빌드 캐시가 동작한 로그](https://github.com/user-attachments/assets/4bc56001-c221-4dd0-bc74-d83f50173fed)

### 설정을 넣는 세 가지 방법 (코드 / ENV / -e)

- **코드**: `app.py`에서 조작, 코드에 기본값을 직접 작성
- **ENV**: Dockerfile에서 조작, 이미지 빌드 시 기본 환경 변수 설정
- **`-e`**: `docker run` 명령어로 조작, 컨테이너 실행 시 환경 변수 주입
