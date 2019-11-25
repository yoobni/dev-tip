# Node JS

Server Side JS

### Lib
- babel-cli : Help babel in console(ES6 transplie)
- nodemon : Restart server when file modify in development environment
- cross-env : Set environment value in Window/Linux/OSX
- express : NodeJS web framework
- body-parser : Use parsing JSON in HTTP request


#### Memo

module import -> createServer -> read file -> writeHead end(JSON.stringy(err)) or end(data)
http.request(option, function) -> handleResponse
블로킹 I/O의 지연회피를 위해 event callback 사용
event module import -> event object -> eventEmitter(이벤트를 발생시키는 모든 객체)
접속시 이벤트가 존재(내장된 이벤트도 존재)
ReadEvalPringLoop(code testing, deverging) like python interpreter
non-blocking
옵저버패턴


TDD
* 정확한 프로그래밍 목적을 디자인 단계에서 반드시 미리 정의해야만 하고 또 무엇을 미리 정의해야한다.
* 개발하는 과정에서 Test Script를 작성하고 코드를 Refactoring 했다는 점이 중요하다.
* 
