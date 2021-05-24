# Hello Spring
## 개요
### 배경
현재 국내 기업에서 규모가 되는 기업들은 Java기반 Spring Framework를 많이 사용하고 있다.

사용하는 이유는 크게 두가지 이유로 볼 수 있다.

1. 성능 + 안정성 측면에서 매우 탁월하다. 
   
2. 국내 시장에서 인력풀이 많다.  

### 목적
인프런 강의 [스프링 입문 - 코드로 배우는 스프링 부트, 웹MVC, DB 접근 기술](https://www.inflearn.com/course/%EC%8A%A4%ED%94%84%EB%A7%81-%EC%9E%85%EB%AC%B8-%EC%8A%A4%ED%94%84%EB%A7%81%EB%B6%80%ED%8A%B8) 을 이용하여 spring boot를 이해한다.

## 프로젝트 환경 설정
Spring Boot Project를 쉽게 만들기 위한 툴로 [spring initializer](https://start.spring.io/) 를 사용한다.

### 라이브러리
build.gradle
```
- spring-boot-starter-thymeleaf: 뷰 템플릿엔진
- spring-boot-starter-web: 스프링부트 웹 라이브러리 모음
- spring-boot-starter-test: 테스트 코드 라이브러리로 Junit 사용
```
Dependencies: 라이브러리에 필요한 의존 라이브러리 자동으로 불러옴

### View 환경설정
정적 페이지 
```
src - main - resources - static
```
[Spring Document](https://docs.spring.io/spring-framework/docs/current/reference/html/)

thymeleaf 템플릿 엔진
[thymeleaf](https://www.thymeleaf.org/)

웹브라우저 - 내장 톰캣 서버 - 스프링 컨테이너 - viewResolver - html 변환 - 웹브라우저

스프링 부트 템플릿엔진 기본 viewName 매핑
`resources:templates/`+{viewName}+`.html`

### 빌드하고 실행하기