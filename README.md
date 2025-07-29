# 📁 Project Setup

프로젝트 기본 셋팅 정보를 정리한 문서입니다.

---

## ✅ 개발 환경

- **Java**: 17
- **Spring Boot**: 3.5.3
- **Build Tool**: Gradle (Groovy DSL)

---

## 🗄️ 데이터베이스

- **DBMS**: MySQL
- **Driver**: `com.mysql:mysql-connector-j`

---

## 🔐 보안

- **Spring Security**
- **JWT** (`io.jsonwebtoken:jjwt`)

---

## 🧩 ORM & 쿼리

- **JPA (Jakarta Persistence API)**
- **QueryDSL 5.x**
    - `QClass`는 `src/main/generated` 디렉토리에서 관리

---

## 🎨 템플릿 엔진

- **Thymeleaf**

---

## 🔧 유틸리티

- **Lombok**
    - `compileOnly` 및 `annotationProcessor`로 설정
- **DevTools**
    - 핫리로딩 지원

---

## 🧪 테스트

- **JUnit 5**
- **Spring Boot Test**
- **Spring Security Test**

---

## 📂 기타 설정

- `QClass`(QueryDSL) 클래스는 다음 경로에 생성됨:  `src/main/generated`
- 빌드 시 자동 생성되며, `clean` 태스크로 자동 삭제 처리 설정됨

---

## 💡 비고

- Spring Boot 3.x부터는 모든 `javax` API가 `jakarta`로 변경되었으므로,
  QueryDSL 및 JPA 설정은 모두 `jakarta.*` 기반으로 구성되어 있음.