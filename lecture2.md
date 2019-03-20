# 190313
# 2 - Python, Flask (1)

## What is Python
### Python은 interpreted programming language
- compiled programming language : compile을 따로 해줘야하는 언어
- interpreted programming language : 한 줄 한 줄 해석하며 실행하는 언어

## Python
### Variable, Type
- Python은 int를 string처럼 처리해서 무한대로 쓸 수 있다
- b[0:3:2] : b에서 0부터 2까지 볼 건데, 2칸씩 뛰어넘으면서 본다.
### Dictionary
- key는 문자 뿐만 아니라 정수도 된다.
- list와 달리, random access를 가능하게 한다.
### For(range)
- for문을 python처럼 쓰면 python-ic하다고 한다 ^^
- range(3) = [0,1,2] 식으로 list를 만들어주는 역할
### For(enumerate)
- For(range)에서는 인덱스를 알 수가 없다
### Function
- Call by reference : 함수 호출 시 인자로 전달되는 변수의 레퍼런스를 전달. 따라서 함수 안에서 인자의 값이 변경되면, 아규먼트로 전달된 객체의 값도 함께 변경된다.
- Call by value : 함수 호출 시 값을 복사해서 사용. 따라서 함수 안에서 인자의 값이 변경되어도, 외부의 변수의 값은 변경되지 않는다.
- call by reference인 변수가 있고(string, list, dictionary...), call by value(int, float...)인 변수도 있다
### File Write
- 문자열만 된다.
- 파일이 없어도 자동으로 만들어준다.

# 190318
# 2 - Python, Flask (1)

## 수업 시간 전
### upstream과 sync를 맞춰야 한다. https://help.github.com/en/articles/syncing-a-fork 참고하기
### git push origin master해야 github에 들어가있다.

## 실습 전
### 브랜치를 만들어야 한다. git checkout -b 숫자-practice-이름
