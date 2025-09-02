---
title: "SQL First"
date: 2025-09-02
draft: false
tags: ["MySQL", "DB"]
categories: ["Database"]
---

# 🤓 **MySQL 이란**

MySQL은 1995년 오라클이 개발한 데이터베이스 관리 시스템으로 오픈 소스 관계형 데이터베이스 관리 시스템(RDBMS)입니다.
주로 데이터 저장 및 관리에 매우 효과적인 언어입니다. 특징과 용도는 다음과 같습니다.

- **특징**: 빠른 성능, 안전성, 다양한 OS 지원, SQL 표준 준수
- **용도**: 웹 애플리케이션, 데이터 분석, 모바일 애플리케이션 DB, 게임 개발 등

---

# 🤓 **설치 및 세팅법(Windows 기준)**

1. [MySQL 공식 사이트](https://dev.mysql.com/downloads/installer/)에서 다운
2. 설치 시 **MySQL Server**와 **MySQL Workbench** 선택
3. 루트 및 계정 비밀번호 설정
4. 설치 중 데이터베이스 설정 가능

   - **비밀번호 설정**: MySQL root 사용자 비밀번호
   - **기본 설정**: 서버 포트(기본값: 3306)와 인증 방식 설정
   - **서비스 설정**: MySQL 서버를 Windows 서비스로 실행할 수 있도록 설정

5. 명령 프롬프트에서 MySQL 접속 확인

```bash
mysql -u root -p
```

6. 데이터베이스 및 테이블 생성 예시

```sql
 CREATE DATABASE testdb;
 USE testdb;

 CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(100)
 )
```

```sql
INSERT INTO users (name, email) VALUES('mason', 'mason@example.com')
```

7. 데이터 베이스 조회하기

다음 명령어로 데이터 베이스를 조회해 봅시다

```sql
SELECT * FROM users;
```
