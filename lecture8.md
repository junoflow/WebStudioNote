# 190415
# 8 - Javascript

## Layout 제작
### margin과 padding
- margin은 element들 간의 간격, padding은 자식 element 간의 간격
- 위 오른쪽 아래 왼쪽 순서로 네 개 숫자로 할 수 있음 0 0 16px 0 -> 아래에만 16px
- 0 auto : 가운데 정렬

## javascript란
### javascript
- 동적으로 content를 다룰 수 있음
- 이벤트(click, scroll, hover)를 다룰 수 있음
- asynchronous network 통신 : API 서버로부터 데이터를 가져옴
- C언어에서 영감을 받았다고 한다

## javascript를 써보자
### variable, type, list, dictionary
- var에 문제가 많아서 let과 const를 쓰게 되었다.
- let과 const 모두 재선언 불가, let 수정가능하고, const는 수정 불가
```
let a = 1
let a = 7 (불가능)
a = 7 (가능)
const b = 7
b = 9 (불가능)
```
### function
- 함수 자체를 변수로 쓸 수도 있다.
- arrow function을 잘 쓰는 방법
  - 원래 : (parameter1. ... , paremeterN) => {statement}
  - (parameter, ... , parameterN) => expression
  - ex
  ```
  (a,b) => {
     return a+b
  }
  
  (a,b) => a+b

## javascript를 적용해보자
### fetch
- 비동기통신 : 오래 걸리는 호출을 할 때 서버와 브라우저 사이에 뭘 만들어서 그걸 거쳐 호출하는 거 -> 안그러면 멈추니까
- promise를 반환
### promise
- callback 함수 : 끝나면 실행되는 함수
- console.log = print
### cors
- cors 처리를 해줘야함
- 두 줄로 가능. 그거 쓰면 된다.
### POST method
- stringify : 직렬화(문자열로 바꾸는 거 = json.dump)
### article fetch 후 보여주기
- parse : 역직렬화(=json.loads)
- 동적으로 삽입 : 순회하며 만든다
