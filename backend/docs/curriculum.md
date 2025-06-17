# 💻 혼부캠 – 실무 중심 통합 개발 커리큘럼 (~ing)

> 혼자서도 실무에 강한 개발자가 되기 위한 15주 통합 루트 – CS, Java, Spring Boot, Linux, Docker, AWS 포함

---

## 🧭 전체 커리큘럼 구성

### ✅ 기본 트랙 (10주)

| 주차      | 영역          | 주제          | 핵심 내용                            | 실습/미니 프로젝트                                   |
| ------- | ----------- | ----------- | -------------------------------- | -------------------------------------------- |
| Week 01 | CS          | 컴퓨터 구조      | CPU, 캐시, 메모리, 버스                 | `jvisualvm`으로 CPU 병목 잡기, Redis 캐시 비교 실험      |
| Week 02 | CS          | 운영체제        | 프로세스, 스레드, 메모리 구조, 시그널           | `htop`, `ps`, `taskset` 실습, StackOverflow 재현 |
| Week 03 | CS          | 데이터베이스      | RDB/NoSQL, 트랜잭션, 인덱스             | `MySQL` + `Redis` 튜닝 비교, `EXPLAIN` 실습        |
| Week 04 | CS          | 컴퓨터 네트워크    | OSI, TCP/IP, DNS, HTTP           | `curl`, `dig`, `wireshark`, NAT 시뮬레이션        |
| Week 05 | CS          | 자료구조        | 배열, 트리, 해시, BFS/DFS              | LRU 캐시 직접 구현, 백준 DFS 문제 병렬 처리 실험             |
| Week 06 | Java        | Java 기초     | 자료형, 제어문, 클래스, 예외                | 미니 ATM 시스템 CLI 버전 만들기                        |
| Week 07 | Java        | 객체지향/컬렉션    | 상속, 추상화, 인터페이스, List/Map         | OOP 기반 도서 관리 시스템 만들기                         |
| Week 08 | Spring Boot | 스프링부트 기초    | 의존성 주입, MVC, Controller, Bean    | 간단한 회원가입 API 구현 프로젝트                         |
| Week 09 | Spring Boot | 스프링보안/DB 연동 | Spring Security, JPA, Validation | 로그인 기능 + DB 연결 API 완성하기                      |
| Week 10 | 통합          | 미니 실전 프로젝트  | CRUD, 에러 처리, 배포 흐름 실습            | 블로그형 미니 서비스 구현 + API 문서화 (Swagger)           |

---

### ✅ 선택 확장 트랙 (Week 11~15)

| 주차      | 영역     | 주제             | 목표                        | 실습 과제                                   |
| ------- | ------ | -------------- | ------------------------- | --------------------------------------- |
| Week 11 | Linux  | 리눅스 기초 및 커널 구조 | 셸, PID, 커널/유저 영역, 시스템 콜   | crontab 설정, 로그 분석 트레이싱                  |
| Week 12 | Docker | 도커 & 컨테이너 구조   | 이미지/컨테이너/볼륨, Compose      | 도커라이징 → Compose 구성 → 배포 실습              |
| Week 13 | AWS    | AWS 기초         | EC2, S3, IAM, VPC 개념      | EC2 인스턴스 띄우고 Spring Boot 배포             |
| Week 14 | DevOps | CI/CD & 배포 구조  | GitHub Actions, 무중단 배포 전략 | GitHub Actions + Docker 이미지 자동 배포       |
| Week 15 | 통합     | 실전 장애 대응 & 면접  | 병목 디버깅, 로그 분석, 기술 면접 대응   | 서버 CPU 100% 상황 디버깅 리포트 작성 + 기술 면접 문답 정리 |

---
## ✅ Week 01 – 컴퓨터 구조

### 🔑 핵심 개념
- CPU, 코어, 스레드, 캐시 (L1/L2/L3), 명령어 사이클
- 메모리 계층 구조: 레지스터 → 캐시 → RAM → 디스크
- 버스: 주소/데이터/제어 버스
- 하이퍼스레딩, 멀티코어, 파이프라이닝, NUMA

### 🔧 실습 과제
- `jvisualvm`을 이용해 CPU 병목 감지
- Redis 캐시를 적용했을 때와 안 했을 때의 응답속도 비교

---

## ✅ Week 02 – 운영체제

### 🔑 핵심 개념
- 프로세스 vs 스레드, PCB, TCB
- 시그널, 시스템 콜, 컨텍스트 스위칭
- 메모리 구조: 스택, 힙, 코드, 데이터 영역
- 페이징, 스와핑, 쓰레싱

### 🔧 실습 과제
- `htop`, `ps`, `taskset` 사용법 익히기
- 재귀 호출로 StackOverflow 재현
- 프로세스 시뮬레이션: sleep + busy loop 조합

---

## ✅ Week 03 – 데이터베이스

### 🔑 핵심 개념
- RDB vs NoSQL, 트랜잭션(ACID), 정규화
- 인덱스 구조(B+ Tree), 커버링 인덱스
- Lock, Deadlock, Isolation Level

### 🔧 실습 과제
- `MySQL`에서 `EXPLAIN`으로 인덱스 효율 확인
- 동일 쿼리에서 인덱스 유무 성능 비교
- Redis vs MySQL 캐시 시나리오 테스트

---

## ✅ Week 04 – 컴퓨터 네트워크

### 🔑 핵심 개념
- OSI 7계층, TCP vs UDP, HTTP 구조
- IP/포트/NAT, DNS 동작 원리
- 3-way handshake, Keep-Alive, TLS 흐름

### 🔧 실습 과제
- `curl -v`, `dig`, `wireshark` 사용해 패킷 분석
- NAT 시뮬레이션: 로컬 서버 포트포워딩 구조 그리기
- HTTP 요청 헤더 분석 및 응답 시뮬레이션

---

## ✅ Week 05 – 자료구조

### 🔑 핵심 개념
- 배열, 연결리스트, 스택, 큐, 트리, 그래프, 힙
- BFS, DFS, 이진탐색, 해시 테이블
- 시간 복잡도(Big-O), 공간 복잡도

### 🔧 실습 과제
- LRU 캐시 직접 구현 (링크드리스트 + 해시맵)
- 백준 DFS 문제 병렬 처리 실험 및 시간 비교
- 우선순위 큐 vs 일반 큐 비교 실험

---
