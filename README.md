# GraphQL
GraphQL로 영화 API 만들기 _nomadcoders


### GraphQL?
GraphQL은 하나의 Specification이다.
아이디어를 각각의 프로그래밍 언어를 통해 구현하는 것이다.
QL은 Query Language를 뜻한다.


### REST의 단점
1. Overfetching : 현재 필요한 정보 이외의 당장 필요없는 데이터까지 fetch받는 경우

2. Underfetching : 애플리케이션 시작할 때 데이터를 받기 위해 많은 요청을 함



### GraphiQL 실습
https://graphql.org/swapi-graphql/
GraphQL에서 제공해주는 api 실습 페이지이며 스타워즈와 관련된 데이터로 실습해볼 수 있다.
오른쪽에 Docs를 누르면 Documentation Explorer가 나타나며 호출할수 있는 데이터와 받을 수 있는 데이터가 정리되어있다.

### Apollo Server 설치 및 설정
Apollo Server는 Node.js 미들웨어이다. API 서버를 호출하기 전에 앞에서 api 요청을 받아 처리한 후 서버에게 전달해준다.


폴더 생성
`mkdir tweetql`

vscode 폴더 오픈
`code tweetql`

node repository 세팅
`npm init -y`

apollo-server와 graphql을 설치
`npm install apollo-server graphql`

nodemon 설치
`npm install nodemon -D`



#### GraphQL의 query
GET// query은 읽기 전용으로 데이터를 가져오기 위한 메서드이다. 
query를 사용하는 경우는 데이터가 변화될 필요 없이 단순한 조회가 필요할 때이다. 예를 들어 View를 그리기 위한 정보 혹은 유저 정보를 가져오기 위한 경우에 사용한다.


#### Mutation
POST, PUT, DELETE//  request 같은 것들은 Mutation Type
 mutation은 데이터를 변경한 후 가져오기 위한 메서드이다
즉, 서버 혹은 Database 등에 변경 작업(POST, PUT, DELETE)이 일어나는 것들은 Mutation에 입력되어야 한다.

