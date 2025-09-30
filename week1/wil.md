1. Spring Boot 애플리케이션을 실행하고, 브라우저에 localhost:8080 을 입력했을 때 나오는 Whitelabel Error Page 스크린샷
<img width="845" height="961" alt="스크린샷 2025-09-30 오후 5 50 30" src="https://github.com/user-attachments/assets/15a71c57-36a0-4914-9266-fe29cde78612" />

---
2. 작성한 온라인 쇼핑몰 프로젝트 API 명세서
### 상품(Product)
- POST   /products
- GET    /products
- GET    /products/{productId}
- PATCH  /products/{productId}
- DELETE /products/{productId}

### 주문(Order)
- POST   /orders
- GET    /orders
- GET    /orders/{orderId}
- POST   /orders/{orderId}/cancel

---

3. 강의 내용 정리

## **📌 1주차 주제: 웹, HTTP, REST API**


### **1️⃣ 웹과 인터넷**

- **인터넷**: 전 세계 기기들이 연결된 네트워크
- **웹(Web)**: 인터넷 위에서 동작하는 대표 서비스
- **클라이언트-서버 모델**
    - 클라이언트: 요청(request) 전송, 응답(response) 수신
    - 서버: 요청 처리 후 응답 반환

---

### **2️⃣ URL 구조**

http://www.example.com:5883/category/food.html?topic=pizza&size=large

- **Scheme**: 통신 규칙 (http, https)
- **Host**: 서버 주소 (도메인/IP)
- **Port**: 서버 포트 (기본은 생략 가능)
- **Path**: 서버 내 리소스 경로
- **Query**: 추가 데이터 (key=value 형식)

---

### **3️⃣ HTTP (HyperText Transfer Protocol)**

- **특징**
    - 무상태성(Stateless): 서버는 요청 상태를 저장하지 않음
    - 비연결성(Connectionless): 요청-응답 후 연결 종료
- **HTTP 요청 구조**
    - Start line (메서드, 경로, 버전)
    - Headers (부가 정보)
    - Body (데이터)
- **주요 메서드**
    - GET: 조회
    - POST: 생성
    - PUT: 전체 수정 (없으면 생성)
    - PATCH: 부분 수정
    - DELETE: 삭제
- **주요 상태 코드**
    - 200 OK: 요청 성공
    - 201 Created: 생성 성공
    - 400 Bad Request: 잘못된 요청
    - 404 Not Found: 리소스 없음
    - 500 Internal Server Error: 서버 내부 오류

---

### **4️⃣ 프론트엔드 & 백엔드**

- **프론트엔드**: 사용자 인터페이스(UI), 화면 개발
- **백엔드**: 데이터 처리, 비즈니스 로직, DB 관리
- **데이터베이스(DB)**
    - 방대한 데이터를 영구적/안전하게 관리
    - DBMS 예시: MySQL, PostgreSQL, MongoDB

---

### **5️⃣ API와 REST API**

- **API (Application Programming Interface)**
    - 프로그램 간 통신 규칙
- **REST (Representational State Transfer)**
    - 자원(Resource): URI로 식별
    - 행위(Verb): HTTP 메서드로 정의
    - 표현(Representation): JSON 등으로 전달
- **REST API 예시**
    - 회원 등록: POST /members
    - 회원 목록 조회: GET /members
    - 회원 상세 조회: GET /members/{id}
    - 회원 수정: PATCH /members/{id}
    - 회원 삭제: DELETE /members/{id}

---

### **6️⃣ Spring & Spring Boot**

- **Spring Framework**
    - 자바 기반 백엔드 프레임워크
    - 객체지향 특성을 살려 엔터프라이즈 앱 개발 지원
- **Spring Boot**
    - 복잡한 설정 없이 스프링을 쉽게 사용 가능
    - 빠른 개발 & 실행 환경 제공
