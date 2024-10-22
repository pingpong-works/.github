## PINGPONG

### 프로젝트 소개
- MSA 기반 그룹웨어 프로젝트 입니다.
- Spring Cloud를 활용하였습니다.
- 개발 기간 : 2024.09.24 ~ 10.18
- URL : https://pingpong-works.com (배포x)
<br>

### 구성원
<table>
  <tbody>
    <tr width='100%'>
      <th align="center" width='10%'>박혜지</th>
      <th align="center" width='17%'>김준하</th>
      <th align="center" width='14%'>양수명</th>
      <th align="center" width='17%'>방승욱</th>
      <th align="center" width='19%'>이광희</th>
    </tr>
    <tr>
      <td align="center"><img width="100" alt="image" src=""></td>
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

### 개발언어

<img src="https://img.shields.io/badge/java-007396?style=for-the-badge&logo=java&logoColor=white">
<img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"/>

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


### [ERD](https://dbdiagram.io/d/Copy-of-Untitled-Diagram-6701a9a8fb079c7ebd7469db)
<img src ="https://github.com/user-attachments/assets/6ab844f1-fcb8-480d-90b9-62a2bf8189f8" width=1713 alt="image" />

<br>

### [Kanban Board](https://github.com/orgs/pingpong-works/projects/1)
Github Kanban
- Github의 Project 기능 중 Kanban 보드를 활용하여 프로젝트를 관리했습니다.
- Todo, InProgress, Done 의 열로 작업을 구분해 현재 작업 상황을 실시간으로 확인할 수 있도록 했습니다.

<img width="1713" alt="image" src="https://github.com/user-attachments/assets/a513b853-54ef-483d-ad7d-bbf2518e924d">
<br>

### 🔍서비스 구현 내용

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
| <img src="" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/14cacd65-015c-4a6c-b892-45e80a06780c" width="370" height="200"/> |

| 근태관리 | 전자결재 템플릿 생성 |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/29844864-f028-4af4-986b-1092bbad5924" width="370" height="200"/> | <img src="https://github.com/user-attachments/assets/ccec61b7-db39-41a0-938f-06b72d1e4eaa" width="370" height="200"/> |

| 전자결재 템플릿 수정 | 전자결재 템플릿 삭제 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 전자결재 조회 | 전자결재 삭제 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 전자결재 작성1 | 전자결재 작성2 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 전자결재 승인 | 전자결재 반려 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 알림-전자결재 알림 | 알림-승인자 알림  |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 알림-일정 알림 | 알림-차량예약 알림  |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |


### 구성원 별 담당 내용

## 박혜지
[알림, 전자결재, 근태관리]


---
<br/>

## 김준하
[직원, 관리자, Spring Security]


---
<br/>

## 양수명
[메일 서버 구축, 메일 송수신, 데이터 관리]

---
<br/>

## 방승욱
[게시판, 일정, 자원 예약]

    
---
<br/>

## 이광희
[Gateway, Eureka]


---
<br>

## 개발 문서

### 요구사항 정의서
[pingpong-요구사항 정의서](https://docs.google.com/spreadsheets/d/1Wm1eB2oXyVdstC47ynx7sx1UHRXSIlatq2_O8U7ozU0/edit?gid=0#gid=0)

### API 명세서
[pingpong-API명세서](https://docs.google.com/spreadsheets/d/1O87LmWl6mkqLLtPM1yqOCbKzsnxeVUi8hP7bycf31d8/edit?gid=646885922#gid=646885922)

## 발표자료
[pingpong-발표자료](https://www.figma.com/deck/0jZrRSnrXrvnOk94DKPGYI/Untitled?node-id=64-634&node-type=slide&t=Plz2XXgwsm0JlVMd-1&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1)



## 프로젝트 회고


### 박혜지
> 

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
