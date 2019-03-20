# 190320
# 3 - Python, Flask (2)

## 외부서버 접속하기
### SSH (Secure SHell)
- 서버에 접속을 한다 = 엄청 위험한 얘기, 돌아다니는 패킷을 가로채서(패킷 스미핑) 악용할 수 있다
- 패킷 보호를 위해 강력한 인증과 암호화를 이용하는데, 그게 SHell.
- $ ssh junoflow@54.180.96.144 password 1234
- if __name__ == '__main__':
    app.run(host='0.0.0.0',port=5002, debug=True)
- 기본포트는 5000. 근데 다 그걸로 들어오면 망함. 그래서 포트를 배정해준다.

## venv
### 독립된 python 환경을 만들어 놓기
- 왜? 복수의 패키지를 사용하는 경우가 자주 발생하는데, 그냥 막 깔아버리면 다른 버전의 패키지들끼리 영향을 주면서 망할 수 있다.
- 그래서, 다른 버전의 무언가를 돌릴 때 사용한다

## Flask
### app.route('/')
내가 쓸 서버의 최상단 루트
### app.route('/variable/<input_strings')
<>안에 있는 건 변수다.
### app.route('/counter')
if not os.path.exists(filename) : os는 파일관리 할 때 사용하는 파이썬 패키지. filename 이름의 파일이 있는지 확인해주세요.

## RESTful API
### API란?
- 어떤 정보를 가지고 싶을 때, 서버에 요청해서 받아올 수 있는 무언가
- 현대의 웹은 API 호출을 많이 하려고 하고 있다. -> SPA(Single Page Application)
- 옛날에는 필요할 때마다 하나하나 불러내야했다면, 현대에는 한꺼번에 다 불러오고 부분적으로 서버에서 가져온다. 그게 현대의 API
### HTTP
- 통신 규약
- 브라우저로 서버에 무언가를 요청할 때, 서버한테 무얼 원하는지 HTTP request를 전달(뭘 원하는지, 무슨 브라우져인지, 누구인지 등등...)
- 그걸 읽어서 서버가 잘 처리해서 브라우저한테 줘야하는데, 그게 HTTP response(뭘 보낼건지, 무슨 프로토콜로 줄건지...) 브라우저가 그걸 잘 해석해서 우리한테 보여준다.
- HTTP Method : GET POST PUT DELETE
- 서버가 처리하는 건 크게 접속한 주소, 어떤 HTTP Method인지
