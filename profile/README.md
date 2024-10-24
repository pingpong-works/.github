## PINGPONG

### 프로젝트 소개
- 중앙정보기술인재개발원 프로젝트 평가 - 대상 수상 🏆
- MSA 기반 그룹웨어 프로젝트 입니다.
- Spring Cloud를 활용하였습니다.
- 개발 기간 : 2024.09.24 ~ 10.18
- URL : https://pingpong-works.com (배포 x)
<br>

### 구성원
<table>
  <tbody>
    <tr width='100%'>
      <th align="center" width='20%'>박혜지</th>
      <th align="center" width='20%'>김준하</th>
      <th align="center" width='20%'>양수명</th>
      <th align="center" width='20%'>방승욱</th>
      <th align="center" width='20%'>이광희</th>
    </tr>
    <tr>
      <td align="center"><img width="100" alt="image" src="https://github.com/user-attachments/assets/51d6b43d-0e95-4f44-a19a-8ff4a44ae0d3"></td>
      <td align='center'><img width="100" alt="image" src=""></td>
      <td align='center'><img width="120" alt="image" src=""></td>
      <td align='center'><img width="100" alt="image" src=""></td>
      <td align='center'><img width="100" alt="image" src=""></td>
    </tr>
    <tr>
      <td width="150"><a href="https://github.com/quokkavely">@quokkavely</a></td>
      <td width="150"><a href="https://github.com/HJk29">@HJk29</a></td>
      <td width="150"><a href="https://github.com/Lifesheep1">@Lifesheep1</a></td>
      <td width="150"><a href="https://github.com/coding-Rhino">@coding-Rhino</a></td>
      <td width="150"><a href="https://github.com/gwanghui97">@gwanghui97</a></td>
    </tr>  
  </tbody>
</table>
<br>

### 프로젝트 아키텍쳐

<img src="https://github.com/pingpong-works/.github/blob/main/assets/architecture.png?raw=true" alt="Project pingpong_wireframe" width="600">
<br>

- Front-end : 클라이언트의 요청이 들어오면 API Gateway에서 로드밸런서에서 Round Robin 방식으로 순서대로 Front Application 에 보내지게 됩니다.
Front Application 은 필요한 요청을 API Gateway 를 통해 처리합니다.
프론트엔드는 Thymeleaf, HTML, CSS, Javascript로 구현되어 있으며, 사용자 인증 및 권한 관리를 위해 Spring Security와 JWT를 사용합니다.


- API - Gateway : API Gateway는 Spring Cloud Gateway를 이용하여 구현되었으며, 클라이언트의 요청을 받아 해당 요청을 처리할 서비스로 라우팅합니다.
또한 Spring Cloud Netflix Eureka Client를 사용하여 유레카 서버로부터 서비스 인스턴스 정보를 검색하고, JWT를 활용하여 인증된 요청만을 허용합니다.
Access 토큰이 만료된 경우, Refresh 토큰과 비교를 통해 요청을 Auth 서버로 보내 토큰 재발급을 받고, 원래 요청을 수행하도록 구현하였습니다.


- Eureka : Eureka 서버는 Spring Cloud Netflix Eureka를 통해 서비스들의 인스턴스 정보를 등록하고 관리합니다. 이를 통해 서비스 디스커버리 및 로드 밸런싱이 가능하며, Gateway는 유레카 서버를 통해 서비스의 위치를 동적으로 찾을 수 있습니다.

<br>

### 개발환경
 - 개발도구: Intellij IDEA
 - 언어: Java 11 Open JDK
 - 빌드도구: Gradle
 - 개발
    - Spring Framework: 5.3
    - Spring Boot: 2.7.0
    - Spring Cloud
      - Spring Cloud Gateway
      - Spring Cloud Netflix(Eureka Server)
      - Spring Cloud OpenFeign
    - Spring Data
      - Spring Data JPA
      - Spring Data Redis
    - Spring Security
    - JPA
      - QueryDsl
 - 데이터베이스
    - MySQL
    - Redis
    - Postgresql
    - Mongo
 - ERD
    - DB Diagram
 - 프론트 개발 환경 및 언어
    - 언어:
      - HTML
      - CSS
      - JavaScript
    - 라이브러리 및 프레임워크:
      - React
      - React Query
      - Zustand
      - React Bootstrap 5
      - Axios
 - 형상관리 및 이슈관리
    - GitHub
 - 기타
   - Slack

<br>

### 개발언어
<span>
<img src="https://img.shields.io/badge/java-007396?style=for-the-badge&logo=java&logoColor=white">
<img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"/>
</span>

### 사용도구

<span>
  <img src="https://img.shields.io/badge/spring boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white">
  <img src="https://img.shields.io/badge/spring cloud-6DB33F?style=for-the-badge&logo=spring&logoColor=white">
  <img src="https://img.shields.io/badge/spring eureka-6DB33F?style=for-the-badge&logo=spring&logoColor=white">
  <img src="https://img.shields.io/badge/spring security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white">
  <img src="https://img.shields.io/badge/spring Data JPA-6DB33F?style=for-the-badge&logo=spring&logoColor=white">
  <img src="https://img.shields.io/badge/spring Data Redis-6DB33F?style=for-the-badge&logo=spring&logoColor=white">
  <br>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=MySQL&logoColor=white">
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=Redis&logoColor=white">
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=MongoDB&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=PostgreSQL&logoColor=white"/>
  <br>

  ### Messaging

  <span>
  <img src="https://img.shields.io/badge/Apache%20Kafka-231F20?style=for-the-badge&logo=ApacheKafka&logoColor=white"/>
  <img src="https://img.shields.io/badge/WebSocket-4D4D4D?style=for-the-badge&logo=websocket&logoColor=white"/>
  </span>

  <br>
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=React&logoColor=white">
  <img src="https://img.shields.io/badge/React_Query-FF4154?style=for-the-badge&logo=ReactQuery&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=Docker&logoColor=white"/>
  <br>
  <img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white"/>
</span>

### etc

<span>
  <img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white"/>
  <img src="https://img.shields.io/badge/css3-1572B6?style=for-the-badge&logo=css3&logoColor=white"/>
  <img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=white"/>
  <img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white"/>
  <img src="https://img.shields.io/badge/Gradle-02303A?style=for-the-badge&logo=Gradle&logoColor=white"/>
  <br>
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
  <img src="https://img.shields.io/badge/Github-181717?style=for-the-badge&logo=github&logoColor=white"/>
  <img src="https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=Slack&logoColor=white">
  
</span>
<br>

----
</br>

### [ERD](https://dbdiagram.io/d/Copy-of-Untitled-Diagram-6701a9a8fb079c7ebd7469db)
<img src ="https://github.com/user-attachments/assets/6ab844f1-fcb8-480d-90b9-62a2bf8189f8" width=1713 alt="image" />

<br>
<br>

----
</br>

### [Kanban Board](https://github.com/orgs/pingpong-works/projects/1)
Github Kanban
- Github의 Project 기능 중 Kanban 보드를 활용하여 프로젝트를 관리했습니다.
- Todo, InProgress, Done 의 열로 작업을 구분해 현재 작업 상황을 실시간으로 확인할 수 있도록 했습니다.

<img width="1713" alt="image" src="https://github.com/user-attachments/assets/a513b853-54ef-483d-ad7d-bbf2518e924d">

<br>
<br>


## 🔍서비스 구현 내용

### 🕹주요 기능

| 로그인 | 메인페이지 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 관리자 페이지 | 부서 생성 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

|  직원 생성  | 직원정보 수정 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 부서별 직원조회 | 내 정보 수정 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 메일 작성 | 받은메일함 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 보낸 메일함 | 휴지통 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 게시판 작성 | 게시판 조회 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 게시글 조회 | 게시글 댓글 작성 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 게시글 수정/삭제 | 자원-차량관리 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 자원-회의실 관리 | 일정 등록 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 일정 조회 | 채팅 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/d31c4b23-0316-4358-9537-9295ae5a7b88" width="370" height="200"/> |

| 근태관리 | 전자결재 템플릿 생성 |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/9f82f44a-8eb1-4a2c-bf21-2827ed10be0d" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/0601d246-480e-4bbf-ac7e-5985616e615f" width="370" height="200"/> |

| 전자결재 템플릿 수정 | 전자결재 템플릿 삭제 |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/f9bcffc7-1d31-41b1-8300-311b190fed47" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/195c03f2-e936-4f02-902d-96ffb2732825" width="370" height="200"/> |

| 전자결재 타입조회 | 전자결재 삭제 |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/fdbfc5c1-6e51-46bd-aa06-2d49b6729736" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/78bd91e3-fdbe-4b48-a700-b25eb74e45ba" width="370" height="200"/> |

| 전자결재 작성 후 제출 | 전자결재 작성 후 임시저장 |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/a5d5c490-8ff2-4a06-b400-9f128c79eb77" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/4758be32-ee56-459e-a3d5-3fcee1fcc2eb" width="370" height="200"/> |

| 전자결재 다시작성 | 전자결재 상태별 조회 |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/886834c2-58f6-49dd-81c7-106d5ef79dee" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/4a9a14ec-4d7a-4d92-a00f-8f3b97d2f532" width="370" height="200"/> |

| 전자결재 승인 | 전자결재 반려 |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/d7f9ef96-481c-4b63-9027-d11740457919" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/dd526818-4d46-46a2-b24a-466222a3ec4d" width="370" height="200"/> |

| 알림-전자결재 알림 | 알림-승인자 알림  |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/5e60637f-9aea-407f-a597-9dd8e18e904e" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/6ebafea4-534a-43ea-aed1-581c7b807b97" width="370" height="200"/> |

| 알림-일정 알림 | 알림-차량예약 알림  |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/e562e877-1407-4796-a3d8-d2492022459d" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/a31b6fa3-21f9-45f7-840b-eaec9fdaf627" width="370" height="200"/> |

<br>
<br>

## 구성원 별 담당 내용
팀의 모든 구성원은 프로젝트 초기부터 설계 작업에 적극적으로 참여했으며, 특히 사용자 요구사항 정의서, API 명세서, ERD 설계 등 핵심적인 아키텍처 설계를 함께 논의하고 결정함으로써 프로젝트의 기틀을 다졌습니다. 이를 통해 전체적인 개발 방향을 명확히 설정하고, 팀원 간의 협업을 원활하게 이끌 수 있는 기반을 마련했습니다.

각자의 담당 영역에서 전문성을 발휘해 구현을 진행했으며, 설계 과정에서 나온 다양한 아이디어와 피드백을 반영하여 프로젝트의 완성도를 높이는 데 기여했습니다.

## 박혜지
[알림, 전자결재, 근태관리]

> ### 알림
- Kafka와 SSE를 활용해 MSA 환경에서 통합된 알림 시스템을 구축
- 다양한 서비스에서 발생하는 알림 이벤트(전자결재 요청, 전자결재 상태, 공지사항, 자원 예약 등)를 지원하도록 설계
- Kafka 프로듀서-컨슈머 구조를 사용해 알림 메시지를 발행하고, Kafka 토픽을 통해 여러 서비스에서 메시지를 수신하도록 구현
- 알림 조회 API에서 읽지 않은 알림과 읽은 알림을 필터링할 수 있는 기능을 추가했으며, 사용자가 알림을 읽음 처리할 수 있도록 업데이트 API를 개발
- Spring Scheduler를 통해 30일이 지난 읽은 알림을 자동으로 삭제하는 기능을 구현하여 데이터 관리 효율성을 높임
- 알림 토글 패널을 개발하여 읽지 않은 알림을 강조 표시하고, 사용자가 알림을 클릭하면 관련된 페이지로 이동하도록 구현
- 알림의 읽음/안읽음을 구분할 수 있게 UI를 추가하여 사용자의 편의성을 높임
- axios를 사용해 알림 데이터의 CRUD 요청을 처리

> ### 전자결재
- 문서 템플릿 생성 기능을 개발해 다양한 양식의 문서를 작성할 수 있도록 했고, 커스텀 필드를 통해 템플릿의 유연성을 높임
- QueryDSL을 활용해 전자결재 문서의 검색 기능을 구현 : 결재 상태, 제출일, 작성자 등을 기준으로 검색할 수 있도록 함
- 결재 라인 설정과 문서 제출, 승인, 반려 처리 API를 구현하여 전자결재의 전반적인 워크플로우를 구축
- 결재 문서의 승인권자 또는 최종 승인 /반려 상태에 따라 Kafka를 이용해 알림 이벤트를 트리거하도록 설정
- 임시저장 기능을 구현하여 작성 중인 문서를 임시로 저장할 수 있고 임시 저장된 문서는 언제든지 불러와 수정 후 제출 할 수 있도록 구현
- 전자결재 문서 작성 페이지를 개발하여, 템플릿 선택 시 커스텀 필드가 동적으로 생성되도록 구현
- 문서 제출 시 결재 라인 설정과 상태 변경에 따른 UI 업데이트 로직을 추가해, 제출 이후에는 문서를 수정할 수 없도록 제한
- 결재 상태에 따라 버튼과 UI 요소가 동적으로 변경되도록 상태 관리 로직을 최적화
- 관리자 페이지에서 문서 템플릿을 생성하여 다양한 양식의 문서를 생성할 수 있으며 템플릿을 수정할 때마다 새로운 버전이 생성되도록 하여 이전 버전의 템플릿도 유지할 수 있도록 구현
- visible 설정을 통해 활성화된 템플릿만 직원이 볼 수 있도록 했으며, 비활성화된 템플릿은 목록에서 제외되도록 처리
- 사용자 입력 값을 검증하고 저장하는 로직을 추가해 클라이언트 측 유효성 검사를 강화
  
> ### 근태관리
- IP 기반 출근 확인 기능을 도입해 사내 네트워크 내에서만 출근, 퇴근 기록을 등록할 수 있도록 구현
- 근무 시간 통계 계산 로직을 개발해 일별, 주별, 월별 근무 시간 통계 데이터를 제공
- 전체 직원의 출퇴근 기록과 근무 시간을 관리자가 조회할 수 있는 API도 추가
- 내 정보 페이지에서 사용자가 출/퇴근 시간과 근무 시간과 쉽게 확인할 수 있도록 했고, 시각화된 차트를 통해 근무 시간 통계를 제공

> ### 그외
- mainpage와 sidebar 구성 및 전반적인 css 수정
- cors 설정 추가(core, alarm, chat -api)
- 채팅방 정보 업데이트 기능 강화 및 kafka 설정 수정
- LocalDateTime 역직렬화 기능 추가

---
<br/>

## 김준하
[직원, 관리자, Spring Security]

> ### Security

> ### 직원 관리

---
<br/>

## 양수명
[메일 서버 구축, 메일 송수신, 데이터 관리]

> ### 메일 서버 구축
- hmail

> ### 메일 송수신
-
-

---
<br/>

## 방승욱
[게시판, 일정, 자원 예약]

> ### 게시판
-

> ### 일정
-


> ### 자원관리
-

> ### 자원예약
-
    
---
<br/>

## 이광희
[Gateway, Eureka, chat]


---
<br>
<br>

## 📃개발 문서

### 요구사항 정의서
[pingpong-요구사항 정의서](https://docs.google.com/spreadsheets/d/1Wm1eB2oXyVdstC47ynx7sx1UHRXSIlatq2_O8U7ozU0/edit?gid=0#gid=0)

### API 명세서
[pingpong-API명세서](https://docs.google.com/spreadsheets/d/1O87LmWl6mkqLLtPM1yqOCbKzsnxeVUi8hP7bycf31d8/edit?gid=646885922#gid=646885922)

## 발표자료
[pingpong-발표자료](https://www.figma.com/deck/0jZrRSnrXrvnOk94DKPGYI/Untitled?node-id=64-634&node-type=slide&t=Plz2XXgwsm0JlVMd-1&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1)

<br>
<br>

## 프로젝트 회고


### 박혜지
> 마이크로 서비스 아키텍처를 도입하여 도전적인 목표를 설정함으로써 실무에서 요구되는 다양한 기술을 경험하고 기술적 역량을 크게 향상시킬 수 있었습니다. 프로젝트 진행 중 어려운 상황에서도 묵묵히 자신의 역할을 수행해준 팀원들 덕분에 완성도 높은 결과물을 도출할 수 있었습니다. 팀과 함께 성장하는 소중한 경험을 쌓았으며, 앞으로도 이러한 경험을 바탕으로 적극적으로 도전할 수 있는 발판이 되었다고 생각합니다.

<br>

### 김준하
> 

<br>

### 양수명

<br>

### 방승욱
> 

<br>

### 이광희
> 

<br>
