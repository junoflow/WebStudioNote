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
- primary key : 고유한
