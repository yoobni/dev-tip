# React
자바스크립트 라이브러리

### About React
페이스북에서 개발한 유저인터페이스 라이브러리.
Virtual Dom 이라는 개념을 사용하여, 상태의 변화에 따라 선택적으로 유저인터페이스를 렌더링.

### Virtual DOM
실제 DOM에 접근하지 않고, 추상화된 자바스크립트의 객체를 사용함.
Virtual DOM을 사용한다고 무조건 빠른것은 아님.

##### Virtual DOM 동작 방법
- 데이터 업데이트 시, 전체 UI를 Virtual DOM에 리렌더링
- 기존의 Virtual DOM과 현재의 Virtual DOM을 비교
- 바뀐 부분에만 실제 DOM 적용

### Lib

- open-color : Useful color library
- prop-types : Use to define 'PropTypes'
- react-icons : Import icons to SVG
- react-onclickoutside : Help outside click library
- react-transition-group : Help CSS animaion
- shortid : Create unique id
- styled-components : Defind CSS in Javascript file
- axios : Http client
- react-addons-update : Immutability helper(when use to change redux's store)
- react-router : Client side router
- react-timeago : Calculate time
- redux : FLUX structure
- react-redux : React & Redux helper
- redux-thunk : Redux middleware to help return function in redux's 'action creator' when using asynchronous call

### Memo

- Presentational component

Presentational component only charge 'view'
It has dom element, styles, container or component
Doen't has redux store permission
It wrote functional component and if has state or LifeCycle

- Redux

The state of the redux is done by the reducer.
Reducer changes the state: according to 'dispatch' function's action object of type.
