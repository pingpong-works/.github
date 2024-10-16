
## PINGPONG

### 프로젝트 소개
- MSA 기반 그룹웨어 프로젝트 입니다.
- Spring Cloud를 활용하였습니다.
- 
- 개발 기간 : 2024.09.24 ~ 10.18
- URL : https://pingpong-works.com
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

<img src="" alt="Project pingpong_wireframe" width="600">

<br>

- 
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
    - MySQL: 8.0.25
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
  <br>
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=React&logoColor=white">
  <img src="https://img.shields.io/badge/React_Query-FF4154?style=for-the-badge&logo=ReactQuery&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=Docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker_Compose-2496ED?style=for-the-badge&logo=Docker&logoColor=white"/>
  <br>
  <img src="https://img.shields.io/badge/Github Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white"/>
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


### ERD
![image]()
<br>

### [Kanban Board](https://github.com/orgs/pingpong-works/projects/1)
Github Kanban
- Github의 Project 기능 중 Kanban 보드를 활용하여 프로젝트를 관리했습니다.
- Todo, InProgress, Done 의 열로 작업을 구분해 현재 작업 상황을 실시간으로 확인할 수 있도록 했습니다.

<img width="1713" alt="image" src="">
<br>

### 🔍서비스 구현 내용

### 🕹주요 기능

| 랜딩 페이지 | 회원가입 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 로그인 실패 및 성공 | 마이페이지 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

|  게시글 작성  | 댓글 작성 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 게시판 | 메일 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

| 전자결재 | 채팅 |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |

|  예약 | 수락  |
| :---: | :---: |
| <img src="" width="370" height="200"/> | <img src="" width="370" height="200"/> |


### 구성원 별 담당 내용

## 박혜지



---
<br/>

## 김준하



---
<br/>

## 방승욱


---
<br/>

## 양수명


    
---
<br/>

## 이광희



---
<br>

## 개발 문서

### 요구사항 정의서
[pingpong-요구사항 정의서](https://docs.google.com/spreadsheets/d/1Wm1eB2oXyVdstC47ynx7sx1UHRXSIlatq2_O8U7ozU0/edit?gid=0#gid=0)

### API 명세서
[pingpong-API명세서](https://docs.google.com/spreadsheets/d/1O87LmWl6mkqLLtPM1yqOCbKzsnxeVUi8hP7bycf31d8/edit?gid=646885922#gid=646885922)

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
