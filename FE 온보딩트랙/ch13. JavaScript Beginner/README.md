### 1. JavaScript 소개

- 웹문서가 브라우저마다 다르게 동작함 → `표준화 작업`
- EX6 버전 사용(ECMAScript 2015)
- Web API + ECMAScript = JavaScript
- 리액트, 뷰, 앵귤러/ 익스프레스/ 일렉트

### 2. script 태그 사용

- `<script src="파일명.js"></script>`  <body>태그 안에 넣어줄 것
- <body> 태그 내의 위치에 따라 자바스크립트 출력 위치도 달라짐
    - (원하는 위치에 넣어주면 됨)
- 일반적으로는 <body>태그의 **가장 마지막 부분**
    - (html파일보다 다소 무거운 js파일을 먼저 로드해버리면 기존에 진행되던 html파싱작업이 멈출 수도 있기 때문)
- js파일을 <head>태그에 넣으면 페이지 로딩이 느려짐
    
    `document.write("<p>JavaScript는 재밌어:)</p>");`
    

### 3. 변수주석

- 변수: 데이터를 담아 놓기 위해 이름표를 붙여놓은 공간
- `var 변수명 = 할당 값;`
- 사용할 수 없는 변수명: 한글, 숫자로 시작하는 문자형태, 공백/특수문자/마침표
- `예약어` : 프로그래밍 언어 자체적으로 사용할 단어 혹은 키워드 => 변수x
- 자바스크립트 키워드 라고 치면 사용할 수 없는 단어 알려준다…
- 자바스크립트 예약어 참고할만한 좋은 사이트
    
    [JavaScript Reserved Words](https://www.w3schools.com/js/js_reserved.asp)
    
- **변수명(식별자)**
    
    
  > 1️⃣ **CamelCase**
    
  - 시작 문자는 소문자, 나머지 단어의 첫글자들은 대문자로 쓰는 방식
    
  - `ex) var sendEmailDate`
    
    
  > 2️⃣ **snake_case**
    
  - 문자 전체가 소문자, 단어와 단어 사이는 언더바(_)로 이어줌
  - `ex) var send_email_date`  
  - 보통 CamelCase방식 사용 (상수는 snake_case를 사용하기도 함)
  - 명명방식은 통일하는게 좋음! 
  
  <br>

- 주석(comments)

    - *// 1. 싱글라인 주석 //*
    - /* 2. 멀티라인 주석 */
        
        ```jsx
        /*
        	이런식으로
        	여러 줄 작성
        */
        ```
        

### 4~6. 자료형

1. **기본형** (단순형, 원시형)
    
    ```kotlin
    1. number
    2. string
    3. boolean
    4. undefined
    5. null
    6. synbol
    ```
    
2. **참조형, 객체**(Object)
- 자바스크립트는 정수(int), 실수 구분 없음