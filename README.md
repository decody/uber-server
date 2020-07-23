# uber-server
A part of server in Uber clone practice from Nomad Coder


### 설치 
```hash
yarn add typescript ts-node nodemon --dev
```

tsconfig.json: 타입스크립트 설정
tslint.json: 타입스크립트 linter를 설정

github 코드에서 해당 설정 복사

```hash
yarn add tsline-config-prettier --dev
```

package.json에 서버 실행 scripts 추가 

`yarn dev`로 실행

### GraphQL Yoga
graphQL로 개발환경을 만들어주는 create-react-app 같은 것

설치
```hash
yarn add graphql-yoga
```

### Middleware 설치
미들웨어는 앱의 연결이나 요청들을 다루는 방식을 수정하는 것

모든 요청을 콘솔에 로깅(기록)하는 미들웨어를 만들고 싶을 때, Logger 미들웨어를 설치함

helmet: 보안 미들웨어
morgan
cors

```hash
yarn add helmet morgan cors
yarn add @types/helmet @types/morgan @types/cors
```

### app.ts 설치
어플리케이션 설정

### api 폴더 생성해서 
예제 파일로 `sayHello.graphql`과 `sayHello.resolvers.ts` 파일을 쌍으로 생성

### schema 파일 생성
```hash
yarn add graphql-tools merge-graphql-schemas
```
api 폴더 내의 *.graphql과 *.resolvers.*을 path 모듈을 이용하여 모든 schema를 가져옴

graphql의 쿼리는 `localhost:8000/playground`에서 확인가능


graphql-to-typescript와 gql-merge 패키지 dev로 설치
```hash
yarn add graphql-to-typescript add gql-merge --dev
```
types 폴더 생성
d.ts 파일은 타입스크립트가 type 정의 파일이라고 인식함. d는 definition

```hash
yarn add babel-runtime --dev
```

모든 graphql 파일을 받아서 하나로 합치고 그 graphql 파일을 typescript로 바꿈
타입스크립트의 리턴값과 graphql의 리턴값을 동기화할 수 있다.