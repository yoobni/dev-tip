# CSS

### Memo

[css]
CSS comb사용시 Gzip 압축기 평균 파일 크기를 줄임
text-shadow: 1px 1px 2px black, 0 0 25px blue, 0 0 5px darkblue;
text-shadow: 0 0 3px red;


[tool]
yeoman - 스카폴딩 (임시 뼈대 구축)


Grunt
* 자바스크립트 프로젝트를 위한 테스크 기반의 커맨드 라인 빌드 툴
* 테스크(task)란 무엇인가? 작업의 단위라고 생각하면 되겠다. js, css, html 같은 static 파일들을 하나로 합치고(concat) 압축을 해서 파일 사이즈를 줄이는(minification) 작업들, 테스트, 배포 등등을 각각 하나의 테스크라고 생각하면 쉽다. Grunt는 이런 빈번한 작업들을 사용자가 미리 정의해 놓은대로(Gruntfile.js) 자동으로 빌드해주는 툴이다. 
* Node.js로 만들어져 있다. 따라서 Node.js가 설치 되어 있어야 하고, npm에 등록 되어 있으며 global로 설치 한다.
Bower
* 프론트엔드 컴포넌트 의존성 관리 툴 이다. 쉽게 말해 위에서 Grunt를 설치하기 위해 사용한 npm과 비슷한 것이다.
* 예를 들어, 새로운 프로젝트를 시작하거나 진행하던 프로젝트에 bootstrap3을 설치한다고 했을때 bootstrap 웹사이트에 가서 소스코드를 다운 받고, 프로젝트의 적당한 디렉토리에 복사할 것이다. 하지만 이미 설치 되어 있는 jquery 버전과 bootstrap에 포함된 jquery 버전과 차이에 의한 의존성 관계가 문제 될 수도 있다.
* bower는 이런 상황에서 각종 컴포넌트들의 설치도 간편하게 해주겠지만, 의존성 부분도 말끔하게 관리해준다.
Yeoman
* 일단은 스캐폴딩 기능만 사용해 봤기 때문에 웹 어플리케이션의 기본 구조를 쉽고, 편하게 잡아줄 수 있는 도구로 생각하고 있다.
* Generator 라는 것을 이용해서 개발하려는 프로젝트 종류(webapp, bootstrap, angularjs 등등)에 따라 기본적인 구조를 알아서 잡아준다.
* 내부적으로 Grunt, Bower를 사용하고 있다.


css 삼각형

```
* {
    padding:0;
    background-color:white;
}

button {
    width:84px;
    height:84px;
    border-color:transparent transparent transparent gray;
    border-style:solid solid solid solid;
    border-width:43px 0 43px 84px;
}
