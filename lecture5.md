# 190403
# 5 - RDBMS

## RDBMS
### 관계형 모델을 기반으로 하는 데이터베이스 관리 시스템
### DB 안에 여러 테이블이 있고, 테이블은 column과 row로 이루어진다.
### why?
- 데이터 삽입, 수정, 삭제, 검색 등의 성능이 빠름 -> B-tree 계열
- 안정성(70년대부터 꾸준히 개발, 이용)
- 성능 괜찮은 무료 오픈소스 다수

### 단점
- 유사도 query 안됨 (70% 유사도 같은 거)
- 설치가 번거로움, resource 많이 씀, SQL 알아야 함

### SQL
- RDBMS 할 때 쓰는 언어

### ORM
- python으로 만들면 SQL로 바꿔주는 거
- python은 class 기반이고, RDBMS는 table 기반이라 mapping이 되지 않음

### python ORM Library
- ORM 중 유명한 게 SQLAlchemy -> Flask에서 쓰기 쉽게 만든 게 Flask-sqlalchemy


- primary_key=True : 탐색을 할 때, 하나라도 indexing이 되어야 빠르기 때문에 이걸 쓴다. 이건 각 요소가 unique하다는 게 보장될 때만 가능.
  (RDB는 binary tree로 indexing을 해서 속도가 빠르다)
- 왜 다 indexing하지 않나? : 인덱싱을 하면 그 관계가 따로 저장되기 때문에 저장공간을 많이 차지, 삽입/수정/삭제 때 무조건 탐색해야하기 때문에 오히려 더 느려질 수도 있다.
  
  
- db.string(300) : 300자 이내로 제한할거임
- __init__ : 생성자. class를 호출할 때마다 나오는 거?
- db = SQLAlchemy()에서 괄호 안에 아무것도 없다. 그래서 만들 때 아무 변수도 가지고 있지 않은데
- db.init_app(app) : app.config에 접근해서 자료를 가져오는 거...라고 치자
- User.query.all() : User class에 있는 걸 다 가져와라
- filter_by(email=email).first() : db에 있는 email과 지금 입력한 email을 비교해서 같은 것 중 첫 번째(filter_by는 하나를 찾든 여러개를 찾든 리스트로
  가져오기 때문에 그 중 하나를 가져오기 위해 first가 필요하다)
- RDB에서도 add와 commit이 필요하다
- 
