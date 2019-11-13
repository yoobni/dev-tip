# React

JavaScript Frame work

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


1. 책으로만 공부하지말 것. 금방 바뀜
2. 리액트 관련 구글링시에는 무조건 지난 1년이내로 설정(중요)
3. 라이브러리가 잘 안붙는 다면 해당 라이브러리 깃헙 이슈 필히 확인
4. 적용이 잘안되거나 어려움이 있는 라이브러리는 고집하지말고 다른 대안으로 대체

리액트는 프레임워크가 아닌 라이브러리!!
때문에 앱의 규모가 커질수록 필요한 것들이 많기 때문에 러닝커브가 상승합니다.


1. 처음에는 CRA(create react app)을 이용해서 정말 너무나도 간단한 앱을 만든다. 미친듯이 간단한 앱
2. 간단히 만든 앱에 redux를 적용한다
3. 그 앱에 react-redux를 적용한다
4. 이해할때까지 몇번이고 다시 기본앱 => redux => react-redux 사이클을 반복한다.
5. CRA를 버린다. npm run eject 명령어 입력시 CRA 구조가 나오는 데 어마어마합니다.
react boilerplate 라고 검색해서 입맛에 맞는 걸 찾아보기도 하고 직접 따라치고 수만가지 오류를 경험하고,
웹팩에 좌절하며 나만의 보일러 플레이트를 만든다 => 마지막으로 만든 앱을 올린다
6. 비동기를 적용한다 (간단한 api 호출 또는 로컬 데이터) json-server 와 axios가 적용하기 쉽습니다.
7. 비동기 적용시 thunk 적용! 만약 실력이 좋다면 saga!
8. 리팩토링으로 타입을 적용한다. (초보) prop-types => flow => typescript (고수)
9. 서버에 올려본다. express 아니면 서버리스도 괜찮습니다.
10. jest 적용해서 컴포넌트 유닛 테스트

그 외에도 컴포넌트 방식의 CSS, JWT 토근 적용, SEO, SSR 등
