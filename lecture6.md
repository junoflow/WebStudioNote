# 190408
# 6 - Relationship

## Query String
### URI와 QueryString
- ? 기준으로 오른쪽
- &로 구분한다
### 쓰임새
- 자원을 필터링할 수 있다는 것
- api/articles : 모든 게시물들을 보기
- "한 게시물을 누르면, 그 게시물 정보와 댓글 등등을 가져오고 싶다!"
- /api/articles?id=1 : 게시물 정보 불러오기
- /api/comments?article_id=1 : 댓글 불러오기
- /api/likes?article_id=1 : 좋아요 불러오기
- /api/likes?article_id=1&user_id=11 : user_id이 11인 사람이 좋아요를 눌렀는지
- /api/comments?article_id=1 POST : 댓글 달기

## Key. Relationship
### primary key, foreign key
- primary key : row를 고유하게 식별하는 기본 키, 자동부여, indexing해서 검색 빠르다.
- foreign key : 다른 테이블의 기본 키를 가리키는 외래키
- foreign key는 데이터의 참조무결성을 확인할 때 사용됨 -> 한 테이블이 다른 테이블의 자료롤 참조할 때, 참조하는 데이터를 위반하지 않는지 확인
  - ex) article에서 없는 user_id로 post하는 경우. user_id를 삭제했는데 그 user_id로 작성한 글이 artcie에 남아있는 경우 등
- join연산의 최적화를 위해 사용
  -ex) "comment가 3개 이상인 article을 찾아줘" : article에 query를 날릴 건데, comment가 필요하다!
    comment에 존재하는 article_id 키와 article에 있는 id 키를 join해서 찾을 수 있다
