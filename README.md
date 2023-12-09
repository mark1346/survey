# 객관식 설문지 프로젝트
김영한 JPA 강의 듣고, 학습을 위해 진행한 프로젝트입니다. 
객관식 설문지를 위한 DB와 Restful API설계가 목표입니다.
설문지 답변 별로 점수가 존재하고, 총점을 확인할 수 있게 설계했습니다. 

## 버전정보
- Java 17
- Spring Boot 3.1.5
- JPA
- H2 DB 2.2.224
## 애플리케이션 아키텍쳐
<img src = "https://github.com/mark1346/survey/assets/54796278/678f2a20-aaf0-45d3-b1f3-55f9ac210241" width="500">
- 계층형 구조 사용

## 데이터베이스 설계
<img src="https://github.com/mark1346/survey/assets/54796278/57b606bb-1390-4133-8da0-6bc1185eb767" alt="ERD" width="500" height="auto">

## 연관관계
### Survey(설문지)

- 여러 Questions 가질 수 있음

### Question(문항)

- 여러 Options 가질 수 있음

### Option(선택지)

- 여러 설문자에 의해 여러 답변에 선택될 수 있음

### Choice(답변)

- 하나의 선택지만 고를 수 있음

### User

- 문항 당 하나의 답변을 골라 여러 답변을 가질 수 있음

## API
- JavaDoc으로 정리됨
- Survey, Question, Option, Choice, User에 대한 CRUD
