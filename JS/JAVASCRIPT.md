# JavaScript

JavaScript develop tip
<br />

##### Js history
 - JavaScript는 google의 V8엔진을 기반으로 동작한다
 - C++로 만들어졌다
 - 95년에 처음 만들어졌다
 - 스크립트 언어이다
 - 표준 내장 객체 및 메소드가 존재하는 다중패러다임 동적언어 이다
 - numbers는 이중정밀도 64비트형식 IEEE 754값으로 정의된다
 - 빈도가 낮은 함수는 함수 내부에 내장하는 방법이 좋다(은 편이다)
 - 가비지 컬랙트를 하는 언어
 - DOM은 Document, Object Model로 JS node개체의 계층화된 트리
 - DOM은 HTML, XML 문서의 프로그래밍 API다, 브라우저 내에서 작동하고 존재한다, 웹페이지 로드 후 브라우저가 DOM페이지를 만든다

#### ES6

- Tagged Template Literals

Use '${Js expression}' between backquote, pass function argument
```JS
    let foo = 5;
    let bar = 10;
    // Result : foo + bar is 15
    console.log(`foo + bar is ${foo + bar}`);
```

#### BOM
 - Browser Object Model
 - Browser element 를 객체화
 - DOM은 웹 페이지 내용 제어
 - 웹 브라우저의 창이나 프레임을 추상화 -> 프로그래밍적으로 제어
 - location 는 문서 위치 control
 - navigator 는 객체 프로퍼티 열람
 - event.preventDefault();
 - Ajax는 Asynchronous JavaScript and XML
 - XMLHttpRequest
 - JSON(JavaScript Object Notation)의 약자로 JavaScript에서 객체를 만들 때 사용하는 표현식
