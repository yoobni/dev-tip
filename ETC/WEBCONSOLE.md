# Web console

- jQuery형식의 querySelect사용으로 web소스 view가능 ```$(‘#id’)```
- $$(‘.class’) : 클래스명이 class인 모든 태그 배열로 가져옴
- getEventListeners($(‘selector’)) : 엘리먼트의 모든 이벤트를 배열로 표현
- 이벤트 상세보기 : getEventListeners($(‘selector’)).eventName[0].listener
- monitorEvents : 이벤트 발생시 콘솔에 로그
- console.time(‘selector’) : 타이머기능(.timeEnd)
- $_ : 마지막 결과값 찾기(콘솔, 연산가능)
