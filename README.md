# 🚀 프로젝트명 (Project Name)

> **한 줄 소개:** 프로젝트의 핵심 가치나 목적을 어필하는 한 줄 설명 (예: 사용자 맞춤형 맛집 추천 서비스)  
> **개발 기간:** YYYY.MM.DD ~ YYYY.MM.DD (O주)  
> **참여 인원:** 개인 프로젝트 or 팀 프로젝트 (O명)

<br>

## 1. 📖 프로젝트 소개
* **기획 배경:** 왜 이 프로젝트를 만들게 되었는지, 어떤 문제를 해결하고자 했는지 간략히 작성합니다.
* **목표:** 이 프로젝트를 통해 달성하고자 했던 기술적/비즈니스적 목표를 명시합니다.

<br>

## 2. 🛠 기술 스택 (Tech Stack)
### Backend
* Java 17
* Spring Boot 3.x
* Spring Data JPA / QueryDSL
* Spring Security (JWT)

### Database
* MySQL 8.x
* Redis (캐싱, 세션 관리)

### Infrastructure
* AWS EC2 / RDS / S3
* Docker / Github Actions (CI/CD)

<br>

## 3. ✨ 핵심 기능 (Key Features)
포트폴리오에서 가장 강조하고 싶은 기능 위주로 작성합니다. (gif나 캡처 이미지를 활용하면 좋습니다.)
* **기능명 1 (예: 소셜 로그인 및 JWT 인증)**
  * OAuth 2.0을 활용한 카카오/구글 로그인 구현
  * Access Token과 Refresh Token을 활용한 보안 강화
* **기능명 2 (예: 실시간 채팅)**
  * WebSocket과 STOMP를 활용한 1:1 실시간 채팅 기능 구현
* **기능명 3 (예: 상품 검색 및 필터링)**
  * QueryDSL을 활용한 동적 쿼리 작성 및 페이징 처리 성능 최적화

<br>

## 4. 🏗 아키텍처 및 ERD (Architecture & ERD)
시스템 구조와 데이터베이스 설계 모델을 시각적인 자료로 보여줍니다.

* **시스템 아키텍처 (System Architecture)**
  * `[시스템 아키텍처 이미지 삽입]` (예: 클라이언트 -> Nginx -> Spring Boot -> DB 등)
* **ERD (Entity Relationship Diagram)**
  * `[ERD 이미지 삽입]` (예: ERDCloud 링크나 캡처본)

<br>

## 5. 🔥 트러블 슈팅 (Troubleshooting)
**취업 포트폴리오에서 가장 중요한 항목**입니다. 개발 중 마주한 문제와 이를 어떻게 논리적으로 해결했는지 작성합니다.

* **문제 1: 대량 데이터 조회 시 N+1 문제 및 성능 저하**
  * **상황:** 메인 페이지에서 100건의 게시글 조회 시 댓글 목록까지 가져오며 101번의 쿼리가 발생 (응답 시간 1.5초).
  * **해결 방안:** Fetch Join을 사용하여 게시글과 댓글을 한 번의 쿼리로 조회. 데이터가 많아질 것을 대비해 페이징 처리 적용.
  * **결과:** 쿼리 수를 1개로 줄이고, 응답 시간을 0.2초로 약 **86% 개선**.
* **문제 2: (예: 동시성 이슈, 메모리 누수, CI/CD 배포 자동화 삽질기 등)**
  * [여기에 작성 또는 기술 블로그 링크 첨부]

<br>

## 6. 🚀 실행 방법 (Getting Started)
프로젝트를 로컬 환경에서 실행해 볼 수 있는 방법을 안내합니다.

```bash
# 1. 저장소 클론
$ git clone https://github.com/username/project.git

# 2. 디렉토리 이동
$ cd project

# 3. 환경 변수 설정 (application.yml 등 설정 방법 기재)
# ex) application-local.yml 파일에 DB 정보 입력

# 4. 빌드 및 실행
$ ./gradlew build
$ java -jar build/libs/project-0.0.1-SNAPSHOT.jar
```
