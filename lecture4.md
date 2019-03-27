# 190327
# 4 - flask, restful

## 서버에 접속하자
### ssh junoflow@54.180.96.144

## 지난 과제 리뷰
### 코드적으로 예쁘게 만들기
-     filename = 'users.json' : 파일 이름이 바뀌는 걸 대비하여 변수로 만듦
-     def get_users(self):
        users = []
        if os.path.exists(self.filename):
            with open(self.filename, 'r') as fp:
                users = json.loads(fp.read())
        return users

반복되는 거라 함수로 따로 빼버렸다. users = self.get_users()로 사용.

## 유저 리스트에 id 부여하기
### id
- 일반적으로 1부터 시작하여 증가하는 순으로 부여
### 실습1 : 기존 api에 id 부여하기
- 5. 새로운 유저를 추가할 때, id를 마지막 유저의 아이디 + 1로 주고 새로 저장
