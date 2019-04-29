# 190429 : 상근님 생일파티
# 9 - React

## React
### A javascript library for building UI
- Facebook에서 만듦 : 믿고 쓴다
- 원래 라이브러리 이용할 때 설치할 게 짱많다 -> 하지만, Create-React-App을 이용한 쉬운 개발환경 setup
- Component 단위 개발 : 이것 때문에 깔끔한 코드가 나온다. 코드를 다른 데에서 재사용 하기 용이
- Virtual DOM을 이용한 높은 성능
- Production level third-party libraries
  - 우리는 ant design을 쓴다.
  - 이것만 써도 꽤 괜찮은 웹사이트를 만들 수 있다.
- Unidirectional data flow : 데이터가 한 방향으로 흐른다
- HTML과 javascript를 합쳐 놓은 듯한 jsx 문법을 사용
### Component 단위 개발
- 웹사이트들은 결국 Component의 집합이다.
- Component 단위 개발의 장점 : component 하나를 잘 짜놓으면 다른 페이지에서 또 쓸 수 있다
- 그렇지만, 순수 html code를 따로따로 만들어서 합쳐준다는 건 매우 복잡한 일이다.
  - 만드는 것도 어렵고, 만들더라도 합쳐주는 것도 어렵다.
- React는 이걸 쉽게 해주는 라이브러리다.
### Virtual DOM
- DOM : html 코드와 브라우저가 보여주는 화면 사이에 있는 무언가
- DOM manipulation : DOM을 수정하는 것, 엄청 느리다.
  - 무언가 변했으면, DOM tree를 다시 만들고, render tree를 확인해서 변경될 node를 계산해서 layout을 수정하고 repaint
  - render tree확인하고 node를 계산해서 layout을 수정하고 repaint 하는 연산을 최소화해야 성능이 올라간다
  - 가상의 DOM을 만들어 계산하고 실제 DOM 연산을 최소화 -> Virtual DOM
### Undirectional Data Flow
- 디버깅이 쉽다는 장점

## Create-React-App
### One command로 React app 생성해주는 Tool
- 
