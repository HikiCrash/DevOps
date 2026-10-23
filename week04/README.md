## 4주차 (Week 4)

---

### 오늘 배운 내용 (What I Learned)

- 자동화 기초
- 프로세스와 백업
- Git 협업 (Pr, Merge, Confilct)
- 네트워크 기본 개념
- 웹 서버 띄우기

---

### 주요 단어 (Key Terms)

- **IP 주소 (IP address)**

  네트워크에서 장치를 식별하기 위한 주소

- **NAT (Network Address Translation)**

  사설 IP 주소와 공인 IP 주소를 변환하여 네트워크 간 통신을 가능하게 하는 기술

- **DNS (Domain Name System)**

  도메인 이름에 대응하는 IP 주소를 찾는 역할, DNS = 도메인 이름 → IP 주소

---

### 주요 코드 (Key Code)

- **`tar`**

  여러 파일을 하나의 아카이브로 묶는 도구

  - `-tzf`: 내용 확인
  - `-xzf`: 압축 해제
  - `-czf`: 압축 생성
  - `-C`: 작업할 디렉터리 지정 (change directory)

- **`diff -rq`**

  다르면, A and B differ 등으로 표시됨

  - `echo $?` 입력 시, `1` 출력
  - `0`: 같음
  - `1`: 다름
  - `2`: 오류

- **`diff -ru A B`**

  다른 내용을 `-`와 `+`로 보여줌

