## 7주차 (Week 7)

---

### 오늘 배운 내용 (What I Learned)

- 도커 컴포즈

### 주요 단어 (Key Terms)

- **도커 컴포즈(docker compose)**: 독립된 컨테이너들이 함께 동작하도록 구성 및 관리하는 도구

---

### docker compose ps 결과 (healthy 포함)

![docker compose ps 결과 (healthy 포함)](https://github.com/user-attachments/assets/7c63496a-9955-41c7-b333-429bff12622a)

### scale 후 각 웹 컨테이너 호스트명(컨테이너 ID)이 바뀐 화면 결과 (캡처)

![scale 후 웹 컨테이너 호스트명 변경 결과 1](https://github.com/user-attachments/assets/25b7f554-bf63-4104-8ba4-f352cf38943e)

![scale 후 웹 컨테이너 호스트명 변경 결과 2](https://github.com/user-attachments/assets/d3ad40b2-b817-4c20-a09e-0bf34786405c)

---

### down 후 up과 down -v 후 up 차이 비교

- **down 후 up을 하면** 컨테이너와 네트워크는 삭제되었다가 다시 생성되지만, 볼륨에 저장된 데이터는 유지되므로 방명록 글이 살아 있다.

- **down -v 후 up을 하면** 컨테이너와 네트워크뿐만 아니라 볼륨까지 삭제되므로, 저장된 데이터도 사라져 방명록 글이 없어진다.

---

### .env를 Git에 올리지 않는 이유 적어보기

비밀번호, API 키 같은 민감한 정보의 보안
