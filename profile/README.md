## PINGPONG

### 프로젝트 소개
- 중앙정보기술인재개발원 프로젝트 평가 - 대상 수상 🏆
- MSA 기반의 그룹웨어 프로젝트 입니다.
- Spring Cloud를 활용하였습니다.
- 개발 기간 : 2024.09.24 ~ 10.18
- URL : https://pingpong-works.com
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
      <td align='center'><img width="100" alt="image" src="https://github.com/user-attachments/assets/a0153d6c-1b8f-44be-aadd-9bcf7ae1f2ff"></td>
      <td align='center'><img width="120" alt="image" src="https://github.com/pingpong-works/.github/blob/main/assets/yang.jpeg?raw=true"></td>
      <td align='center'><img width="100" alt="image" src="https://github.com/user-attachments/assets/eeca2938-2795-4e78-88bc-cde8fd9a8982"></td>
      <td align='center'><img width="100" alt="image" src="https://github.com/pingpong-works/.github/blob/main/assets/lee.jpg?raw=true"></td>
    </tr>
    <tr>
      <td align="center" width="150"><a href="https://github.com/quokkavely">@quokkavely</a></td>
      <td align="center" width="150"><a href="https://github.com/HJk29">@HJk29</a></td>
      <td align="center" width="150"><a href="https://github.com/Lifesheep1">@Lifesheep1</a></td>
      <td align="center" width="150"><a href="https://github.com/coding-Rhino">@coding-Rhino</a></td>
      <td align="center" width="150"><a href="https://github.com/gwanghui97">@gwanghui97</a></td>
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
| <img src="https://github.com/user-attachments/assets/e0d19bc9-9abd-41ce-b392-16b5becd49ba" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/3ffc9d43-187a-4b4b-bf5b-60ee59858391" width="370" height="200"/> |

| 관리자 페이지 | 부서 생성 |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/007cb3e2-20aa-475f-bd88-9ead7472a9c1" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/36aef486-65d4-42ea-8ecb-158f3e769bce" width="370" height="200"/> |

|  직원 생성  | 직원정보 수정 |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/8e8d5198-5bb7-493e-9e3e-46d5ab3d18d3" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/7ee974f8-a7f0-4181-8bda-5a1f391dc7bf" width="370" height="200"/> |

| 부서별 직원조회 | 내 정보 수정 |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/06b12ee2-6f51-427b-8abb-71f6ee500e1a" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/7ee974f8-a7f0-4181-8bda-5a1f391dc7bf" width="370" height="200"/> |

| 메일 작성 | 받은메일함 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 보낸 메일함 | 휴지통 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 게시글 작성 | 게시판 조회 |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/411e812e-b7fd-40cf-bc46-31055d03e9b9" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/46fc724b-44a3-4c60-83e9-5b6266383852" width="370" height="200"/> |

| 게시글 조회, 수정, 삭제 | 게시글 댓글 작성, 수정, 삭제 |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/c112b0b4-330b-43b4-9a19-6c956af7e885" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/1fcee90c-dce5-4501-8833-40525496311b" width="370" height="200"/> |

| 자원-차량관리 | 자원-회의실 관리 |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/edd40f63-4d69-412c-9a41-d58c94285023" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/dd287292-f488-4beb-9df6-00ac55ff307b" width="370" height="200"/> |

| 일정(자원 예약) 등록 | 일정(자원 예약) 조회, 수정, 삭제 |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/e67d0140-c529-42b7-b468-45468dcf1a4e" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/707e2f86-c304-482b-8c33-2ab2a6ee2d17" width="370" height="200"/> |

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

| 채팅 | 알림-전자결재 알림  |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/d31c4b23-0316-4358-9537-9295ae5a7b88" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/5e60637f-9aea-407f-a597-9dd8e18e904e" width="370" height="200"/> |

| 알림-승인자 알림 | 알림-일정 알림  |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/6ebafea4-534a-43ea-aed1-581c7b807b97" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/e562e877-1407-4796-a3d8-d2492022459d" width="370" height="200"/> |

| 알림-차량예약 알림 |
|:------------------:|
| <img src="https://github.com/user-attachments/assets/a31b6fa3-21f9-45f7-840b-eaec9fdaf627" width="370" height="200"/> |


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
[ Security, 직원 기능, 관리자 기능 ]

> ### Security [BE]

- Spring Security와 JWT를 사용해 사용자 인증 정보를 안전하게 관리
- Redis를 활용해 세션 관리를 최적화하여 시스템의 성능 향상

- 사용자 권한에 따라 일반 직원은 기본 정보만, 관리자는 모든 민감한 정보와 관리 기능에 접근할 수 있도록 설정

- 로그인하지 않은 사용자가 특정 페이지에 접근하려고 할 때, 로그인 페이지로 자동으로 리다이렉트되도록 라우팅 기능 구현

- Redis를 사용하여 세션 정보를 캐싱하고, JWT 토큰의 유효성을 검증하여 비정상적인 접근 시 즉시 차단할 수 있도록 설정

> ### 직원 기능 [BE, FE]
- 로그인/로그아웃
    - 관리자가 발급한 이메일과 초기 비밀번호를 통해 직원들이 바로 로그인/로그아웃할 수 있도록 구현

- 주소록
    - 회사 내부 직원의 연락처와 활동 상태를 손쉽게 조회할 수 있도록 주소록 페이지 구현
    - 로그인 상태를 기반으로 실시간으로 활동 상태를 확인 가능
    - 부서별 필터링 기능을 추가해  효율적으로 필요한 직원의 정보 조회

- 마이페이지
    - 개인 프로필 정보 조회 기능
    - 내 정보 수정 기능 
    - 사용자가 주기적으로 비밀번호를 변경할 수 있도록 하여 보안을 강화.

> ### 관리자 기능 [BE, FE]
- 부서 관리
    - 부서 생성 및 삭제
    - 부서 목록과 각 부서의 직원 수를 조회하도록 구현

- 직원 관리
    - 직원 정보 수정(이름, 이메일, 부서, 직급)
    - 퇴사자 계정 삭제
- 주소록
    - 일반 직원들이 조회할 수 있는 정보 외에도, 관리자는 직원 단일 조회 시 추가적인 민감한 정보를 확인할 수 있도록 구현


> ### 그 외
- 메인 페이지에서 사용자가 속한 부서의 직원들이 현재 활동 중인지, 비활동 중인지 빠르게 확인할 수 있는 목록을 구현.

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
[게시판, 일정(자원 예약), 자원 관리, AWS S3]

> ### 게시판
- QueryDSL을 활용하여 게시물의 키워드, 카테고리를 동시에 검색할 수 있어 사용자에게 원하는 정보를 제공
- 게시물 정렬 기능을 통해 사용자에게 다양한 방식으로 게시물을 탐색할 수 있는 옵션을 제공
- 페이지네이션을 통해 게시물 로딩 시 성능을 최적화를 하여 사용자에게 쾌적한 사용 환경을 제공

> ### 일정(자원 예약)
- 부서별 일정을 관리할 수 있도록 캘린더를 부서 단위로 나누고, 부서가 사라지면 해당 부서의 일정 데이터도 자동으로 삭제되도록 설정
- 월별, 주별, 일별로 일정을 볼 수 있도록 다양한 뷰를 제공하여 사용자가 일정을 쉽게 파악할 수 있게 구현
- 일정 등록 시 자원 예약도 가능하도록 하되, 이미 예약된 시간과 겹칠 경우 예약이 불가능하도록 구현
- 현재 시간 이후의 일정은 일정 페이지의 Events 항목에 시간순으로 표시되어, 급한 일정을 확인 할 수 있음

> ### 자원관리
- 차량 등록 시 이미지와 해당 이미지의 설명을 함께 저장할 수 있도록, Map 구조를 활용한 엔티티 필드를 구현

> ### AWS S3
- 서비스에서 필요한 이미지 파일을 AWS S3에 저장하여, 파일 관리를 효율적으로 하고 사용자에게 안정적인 파일 접근성을 제공
- POST나 PATCH 요청을 통해 이미지가 추가 변경 되는 경우 요청 시 S3에 해당 이미지를 추가하거나 삭제하여 S3 저장소 최적화

> ### 그 외
- 직원 정보 수정 시 sideBar도 수정된 내용으로 렌더링되게 구현
- 메인 페이지의 게시판, 캘린더 추가

## 이광희
[Chat, Gateway, Eureka]

> ### Chat [FE, BE]

### BE

- Apache Kafka
  - 분산형 스트리밍 플랫폼으로, 대규모 데이터 흐름을 처리하고 실시간으로 이벤트를 관리
  - 데이터를 특정 토픽으로 구분하여 메시지를 게시하고 구독할 수 있어, 다양한 이벤트 소스를 효과적으로 관리
  - 채팅 메시지를 디스크에 지속적으로 기록하여, 시스템 장애 발생 시에도 메시지 손실을 방지

- Web Socket
  - 실시간 채팅 기능을 구현하기 위해 WebSocket을 활용하여 클라이언트와 서버 간의 양방향 통신 지원

- MongoDB
  - 비정형 데이터를 효율적으로 저장하고 빠른 조회를 지원하는 MongoDB 사용
  - 실시간으로 주고받은 채팅 메시지를 저장하기 위해 활용

- Postgresql
  - 정적 데이터 특성에 최적화되어 데이터 무결성을 보장하는 Postgresql 사용
  - 유저 정보와 채팅방 정보를 저장하기 위한 관계형 데이터베이스를 활용한 설계

### FE

- 컴포넌트 설계
  - Chat Container, Group Modal 등의 컴포넌트를 조합하여 채팅 기능을 구현

- 상태 관리
  - WebSocket 연결 상태, 메시지 기록, 참가자 데이터 관리

> ### Gateway [BE]

- 클라이언트 요청을 여러 마이크로서비스로 라우팅하여 중앙 집중식 관리
    - API 호출 시 보안 검증을 통해 인증된 사용자만 접근 가능하도록 인증/인가 구현
    - 여러 서비스 인스턴스에 요청을 분산시켜 성능과 안정성을 향상
    - 여러 서비스로부터의 응답을 집계하여 클라이언트에게 단일 응답으로 전달
    - API 요청 및 응답을 모니터링하고 로깅하여 성능 분석 및 문제 해결

> ### Eureka [BE]

- 분산된 서비스 관리를 위한 Service Discovery 기능을 수행하기 위한 Spring Netflix Eureka 서버 설정
    - 클라이언트 애플리케이션이 Eureka 서버에 등록하여 자신의 존재를 알리고, 서비스 정보를 갱신
    - 다른 클라이언트가 필요한 서비스의 정보를 Eureka 서버를 통해 조회
    - 서비스 인스턴스가 실패할 경우 Eureka가 자동으로 해당 인스턴스를 감지하고, 클라이언트에게 최신 정보를 제공
    - Eureka의 Service Registry 에 등록된 각 서비스 정보들을 기반으로 Gateway 에서 라운드 로빈 방식의 로드밸런싱이 이루어지도록 설정


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
> MSA 방식의 개발은 처음이었기 때문에, 서비스 분할과 각 서비스의 역할을 명확히 정의하는 과정에서 많은 도전이 있었습니다. 특히, 개별 서비스들이 어떻게 유기적으로 동작하고 서로 협력해야 하는지를 이해하는 데 시간이 걸렸지만, 팀원들 모두 처음 도전하는 MSA였기에, 함께 공부하고 문제를 해결하는 과정에서 많은 성장을 경험할 수 있었습니다. 덕분에 새로운 개발 방법을 익히면서도, 협력의 힘으로 안정적이고 완성도 높은 결과물을 만들어낼 수 있었습니다. 이번 경험은 앞으로 더욱 도전적인 프로젝트를 수행하는 데 든든한 밑거름이 될 것입니다.

<br>

### 양수명

<br>

### 방승욱
> 어려운 문제에 도전하는 것을 좋아하기에 이번 프로젝트를 통해 많은 성장을 이루며 즐겁게 진행했습니다. 모놀리식 아키텍처와 달리 MSA에서는 각자 본인의 서비스에 집중해 개발할 수 있어 Git 충돌 문제가 적고, 서비스마다 독립적으로 데이터베이스를 설정할 수 있다는 점이 인상 깊었습니다. 팀원들 또한 자신의 서비스를 구현하기 위해 각자의 역할에 최선을 다해 주었고, 덕분에 프로젝트를 성공적으로 마무리할 수 있어 매우 감사하게 생각합니다. 

<br>

### 이광희
> 모놀리식의 아키텍처의 단점을 깨닫고 MSA 기반 프로젝트를 하고 싶어 팀원들에게 제안을 했습니다. 배우고자 하는 의지가 강한 팀원들이였기에 프로젝트 처음부터 공부를 각자 진행하며 서로 배운 내용을 공유하는 방식으로 진행했습니다. MSA 뿐만 아니라 대량의 데이터를 안정적이고 실시간으로 처리할 수 있는 Apache Kafka와 사용하지 않았던 데이터베이스까지 공부하며 적용하느라 고생 많았다고 전하고 싶습니다. 이번 프로젝트 경험을 토대로 실무에 가서 배우지 않고 어려운 기술도 잘 해낼 수 있는 엔지니어가 되었으면 좋겠습니다.

<br>
