<div align="center">

### Java / Spring Backend Developer

**요청과 데이터의 흐름을 이해하고, 문제를 끝까지 해결하는 백엔드 개발자입니다.**

Spring 기반 REST API와 데이터 처리, WebSocket 실시간 통신 기능을 구현했습니다.  
단순히 기능을 완성하는 데 그치지 않고 **동작 원리와 데이터 일관성**을 고민합니다.

[![Notion Portfolio](https://img.shields.io/badge/Notion-Portfolio-000000?style=flat-square&logo=notion&logoColor=white)](https://placid-literature-646.notion.site/3e1f533a052381e8ba3ef68215b6f743)
[![GitHub](https://img.shields.io/badge/GitHub-plkj1032-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/plkj1032)

</div>

---

## 🛠 Tech Stack

### Backend · Project

![Java 17 / 21](https://img.shields.io/badge/Java_17%20%2F%2021-007396?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Spring MVC](https://img.shields.io/badge/Spring_MVC-6DB33F?style=flat-square&logo=spring&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white)
![Spring Data JPA](https://img.shields.io/badge/Spring_Data_JPA-6DB33F?style=flat-square)
![MyBatis](https://img.shields.io/badge/MyBatis-BE3939?style=flat-square)
![WebSocket](https://img.shields.io/badge/WebSocket-010101?style=flat-square)
![STOMP](https://img.shields.io/badge/STOMP-6A5ACD?style=flat-square)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)

- Java/Spring 기반 REST API, Controller → Service → Mapper/Repository 처리 흐름 구현
- JPA·MyBatis를 활용한 데이터 조회·저장, 트랜잭션 및 서비스 정책 처리
- WebSocket/STOMP 실시간 채팅과 Redis Pub/Sub 서버 간 이벤트 전달

### Database · Project

![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white)

- MySQL 기반 관계형 데이터 관리와 SQL 조회·저장
- Redis Pub/Sub으로 실시간 이벤트 전달, MySQL에 채팅 기록 영속화
- Flyway를 이용한 DB 스키마 변경 관리

### Infrastructure & Collaboration

![AWS EC2](https://img.shields.io/badge/AWS_EC2-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)

- **Project:** AWS EC2 기반 서비스 배포·환경 설정 및 Git/GitHub PR 협업
- **Practice:** Linux, Docker, Nginx, VPC·Subnet·Routing 등 서버·네트워크 실습

---

## 📂 Portfolio

📚 **[Notion | 상세 개발 포트폴리오](https://placid-literature-646.notion.site/3e1f533a052381e8ba3ef68215b6f743)**  
프로젝트 소개, 시연 영상, 개인 담당 기능 및 트러블슈팅을 정리했습니다.

---

## 🚀 Main Projects

### 🌿 [Mood&Move | 감정 기록과 행동 추천·재측정](https://github.com/plkj1032/mood-and-move)

> 감정 기록 → 행동 추천 → 실행 → 기분 재측정 → 캘린더·통계로 이어지는 서비스

**2026.09 ~ 2026.10 | 3인 팀 프로젝트**  
`Java 21` `Spring Boot` `JPA` `MySQL` `Flyway`

**직접 담당한 기능**
- 사용자별 하루 1회 일기 작성 정책과 작성 가능 상태 관리
- 추천 행동 실행(`STARTED`) 및 기분 재측정 후 완료(`COMPLETED`) 처리
- 관련 상태와 점수가 함께 반영되도록 트랜잭션 처리
- 월간 감정 캘린더·행동 효과 통계 및 위치 기반 장소 조회 연동

**설계 관점:** 화면의 입력 제한만 믿지 않고 서버의 일기 작성 정책을 검증했으며, 행동 완료와 재측정 결과가 서로 어긋나지 않도록 데이터 처리 단위를 고려했습니다.

🎬 [팀 전체 시연 영상](https://youtu.be/KhvVEx4mxlc) · [Notion 상세보기](https://placid-literature-646.notion.site/Mood-Move-404f533a052381a289dcc8732985a530?source=copy_link)

---

### 🚇 [MeetBack | 모임 관리와 실시간 채팅](https://github.com/plkj1032/meetback)

> 모임 생성·참여, 장소 투표·최종 확정과 실시간 채팅을 지원하는 모임 서비스

**2026.08.18 ~ 2026.09.02 | 5인 팀 프로젝트**  
`Java 17` `Spring Boot / MVC` `MyBatis` `MySQL` `WebSocket/STOMP` `Redis Pub/Sub`

**직접 담당한 기능**
- 모임 생성·참여와 장소 투표·최종 확정 기능
- STOMP/WebSocket 채팅 및 참가자 접속 상태(Presence) 관리
- Redis Pub/Sub을 이용한 다중 애플리케이션 인스턴스 간 실시간 이벤트 전달

**트러블슈팅:** 애플리케이션 인스턴스별로 관리되는 WebSocket 연결 때문에 이벤트가 다른 서버의 사용자에게 자동 전파되지 않는 문제를 경험했습니다. Redis Pub/Sub으로 서버 간 이벤트를 전달하고, MySQL은 채팅 기록 저장용으로 구분했습니다.

🎬 [MeetBack 시연 영상](https://youtu.be/kyOFVK_VOP8) · [Notion 상세보기](https://placid-literature-646.notion.site/MeetBack-3e1f533a052381649546dc5ab2dac5e7?source=copy_link)

---

### 🔒 [SPOILOCK | 시청 진행률 기반 스포일러 방지 커뮤니티](https://github.com/plkj1032/spoilock)

> 드라마 시청 진행률에 맞춰 스포일러 노출을 제한하는 커뮤니티 서비스

**2026.10.19 ~ 2026.11.16 예정 | 3인 팀 프로젝트 · 개발 진행 중**  
`Java 21` `Spring Boot` `Spring Security` `JPA` `MySQL` `JWT` `AWS EC2`

**담당 개발 범위**
- 회원가입·로그인 및 JWT 기반 인증
- 드라마·에피소드·사용자 시청 진행률 API
- 홈 화면, 채팅 연결 및 AWS EC2 배포 환경 연동

현재 개발 중인 프로젝트로, 완료·검증한 기능에 맞춰 내용을 계속 갱신하고 있습니다.

[Notion 상세보기](https://www.notion.so/404f533a0523813d9ba5cdd2c8c15513)

---

## 💻 Personal Project

**[Java JSP/Servlet Board](https://github.com/plkj1032/java-jsp-PostBoard)**  
Spring 사용 이전에 Java 웹 동작 원리를 이해하기 위해 만든 게시판입니다.  
JSP/Servlet, JDBC, HttpSession 로그인, 게시글 CRUD 및 검색·페이징을 학습했습니다.

---

## 🔧 How I Solve Problems

**1. 요청과 이벤트의 흐름을 나누어 분석합니다.**  
MeetBack에서 WebSocket 연결과 Redis Pub/Sub의 역할을 구분해 다중 서버 간 이벤트 전달을 구현했습니다.

**2. 데이터의 일관성을 함께 고려합니다.**  
Mood&Move에서 일기 작성 정책과 행동 실행·재측정 상태를 서버 검증 및 트랜잭션으로 처리했습니다.

**3. 수정 후 동작을 확인합니다.**  
재현 조건과 처리 흐름을 확인하고 문제를 수정한 뒤 동일한 상황에서 결과를 다시 검증하려고 합니다.

---

<details>
<summary><strong>Previous Experience</strong></summary>

임베디드 QA (2022.08 ~ 2024.11)  
Camera·Wi-Fi·LAN 기능 검증 및 정상 SDK와 제품 설정 비교를 통한 LAN 장애 원인 분석·해결 경험이 있습니다.

</details>

---

<div align="center">

**기능 구현부터 결과 검증까지 고민하는 백엔드 개발자**

[📚 Notion Portfolio](https://placid-literature-646.notion.site/3e1f533a052381e8ba3ef68215b6f743)

</div>
