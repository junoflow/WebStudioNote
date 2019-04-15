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

##javascript를 
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
