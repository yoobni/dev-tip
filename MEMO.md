# Memo
Memo : About dev blog, site, tips, studying

### Js
- [How to become a great JS devloper](https://boycoding.tistory.com/1?category=915176)


### Project

- Todolist : Like trello
- Eng workbook :
- Customizing Lib : css(with sass), js(browser trick), jQuery
- 삼국지 : Like sd삼국지
- Chatting system : Like kakao talk
- Maple simulater
- resume page
- academy admin page
- discord.js api

### Running Skill
Hard Skill / Soft Skill / Business Skill

##### 'Hard Skills' : Learn by Studying
1. Basic Knowledge
2. Understanding for Product
3. Development Cycle
- Requirements & Analysis
- Design & Modeling
- Implementation
- Test/Release
- Feedback / Update

##### 'Soft Skills' : Learn by Experience
4. Project Management
- Why, What, How
- Cost(Resource) / Time(Schedule) / Scope(Quality)
5. Team Management
- Forming-> Storming-> Norming-> Performing
- Roles around the Team
- Producer, Artist, Designer, Engineer
- Clear role definition, Proper delegation
6. Process (Agile, Zero-Bug)
- Better way to do it, Optimal way
- Development Process
- Ex : Joel Test(Dead Line)
- Project Management Process
- Ex : PMMM
Level 1. initial = Common Language
Level 2. Repeatable = Common Process
Level 3. Defined = Singular Methodology
Level 4. Managed = Benchmarking
Level 5. Optimized = Continuous Improvement

##### 'Business Skills' : Learn from People
7. HR System
- Hiring / Performance Review / Titles(Engineering) / Rewards / Education / Benefits
- Attract -> Develop -> Engage
- SW Engineer Position Ex : Productivity / Professionalism / Teamwork / Knowledge / Functionality / Implementation(Good Code) / Design & Architecture
8. Business Management
- Balanced Scored Ex : Financial / Customer / Internal / Learning & Growth Perspective
9. Vision / Goals / Culture
- Company Level / Team Level / Your Level

---

#### Temp memo

웹 브라우저를 프로그래밍적으로 제어
브라우저가 코드를 해석
웹 브라우저만을 위한 언어가 아님(아니게 변함)
웹 서버로서도 이용(server side Lang)
브라우저가 요청 -> 웹서버 응답
google app script
IDE ( Integrated Development Environment )
coding, debug, complie
크로스 브라우징(CORS)
IDE
코딩 디버그 컴파일 배포 프로그램을 처리하는 환경 소프트웨어

---

### Keyword

React, redux, angular, vue
Find atom, JetBrain
slack api, discord api with node
new server(at academy)

---

### DOM

DOM 자체는 느리지 않음.
DOM에 직접 변화를 주면, 브라우저가 CSS를 연산해 레이아웃을 구성하고(reflow) 웹페이지를 리페인트하느라 느려짐.
짧은 시간안에 여러 reflow는 한번에 처리하지만, 일부 코드는 그렇지 못함.

---

### React Studying
리액트는 프레임워크가 아닌 라이브러리기 때문에 앱의 규모가 커질수록 필요한 것들이 많아지고, 그에 따른 러닝커브가 상승

**공부하는 방법**
1. 책보다는 구글링으로 문제를 해결
2. 라이브러리가 잘 안붙는 다면 해당 라이브러리 깃헙 이슈 필히 확인
3. 적용이 잘안되거나 어려움이 있는 라이브러리는 고집하지말고 다른 대안으로 대체

**공부하는 순서**
1. 처음에는 CRA(create react app)을 이용해서 간단한 앱을 만든다.
2. 간단히 만든 앱에 redux를 적용한다
3. 그 앱에 react-redux를 적용한다
4. 이해할때까지 몇번이고 다시 기본앱 => redux => react-redux 사이클을 반복한다.
5. CRA를 버리고 react boilerplate를 찾아보고 고쳐보고 만들어보기(나만의 보일러 플레이트 만들기).
6. 비동기를 적용(간단한 api 호출 또는 로컬 데이터) json-server와 axios가 적용하기 쉬움
7. 비동기 적용시 thunk 적용 만약 실력이 좋다면 saga
8. 리팩토링으로 타입을 적용한다. (초보) prop-types => flow => typescript (고수)
9. 서버에 올려본다. express 아니면 서버리스도 괜찮습니다.
10. jest 적용해서 컴포넌트 유닛 테스트

그 외에도 컴포넌트 방식의 CSS, JWT 토근 적용, SEO, SSR 등
