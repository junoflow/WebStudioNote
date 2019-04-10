# 190410
# 7 - HTML, css

## HTML
### HTML
- 웹페이지를 만드는 언어다
### HTML TAG
- <head>와 </head> 사이에는 메타 정보들을 넣음
  - 메타 정보 : title 등
- <body></body>에는 main
- nested 구조 : html 안에 head 안에 title이 있는 계층적 구조
- <meta charset="UTF-8"> : 한글 쓸 때 안 깨지게
- <h1> header : 제목 쓸 떄
- <p> : 평문, 기본 margin을 가지고 있다.
- <img src="주소"> : 주소에 맞는 이미지, 안 닫아도 됨
- <a href="주소"> : 하이퍼링크
- <br /> : enter
- <div> : 엄청 많이 쓴다. 코드 상에서 구분을 위한 도구. div만 이용하면 다 만들 수 있다.
- <from action="서버주소" type="post"> : input 내용들을 모아 어떤 http method를 쓸 건지 정해줄 수 있다.
- <input type="     "> : 미리 정해져있는 게 있다. ex) text, password, submit...
### HTML id attribute
- javascript나 css에서 쓸라고 만든다.
### HTML class attribute
- 비슷한 기능인 애들을 묶어 class로 만들어놓으면 나중에 속성 같은 거 바꿀 때 유용하다

## CSS
### CSS?
- html이 문서라면 css는 그 문서를 꾸미는 것
- head에 <style>로 넣는다
- #은 id, .은 class에 접근
- 만약 충돌하면 (p에서는 12pt 줬는데, class description에서 11pt 줬을 때) : 나중에 쓴 게 기준
