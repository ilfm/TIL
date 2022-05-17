# TIL
Today I Learned / 배운 것 기록하기

### 2022.03.02


- javax.servlet.jsp.jsptagexception no message found under code



- PostgreSQL 테이블 좌우로 합치기
  https://greendreamtrre.tistory.com/683
  
- 마이바티스 시퀀스 넣기
```
<selectKey keyProperty="newSeq" resultType="int" order="BEFORE">
  
</selectKey>
```

### 2022.03.04
- readValue
  JSON타입의 값을 맵 형태로 변환aadmin

```
  ObjectMapper.readValue( arg, type )
  arg: 변환대상
  type: 대상을 어떤 타입으로 변환할것인지 명시한다.
  JavaClass 혹은 Class객체, TypeReference객체가 올 수 있다.
    ex)mapper.readValue(arg, ArrayList.class);  
  mapper.readValue(arg, new ArrayList<HashMap<String, String>>().getClass())  
  mapper.readValue(arg, new TypeReference<ArrayList<HashMap<String, String>>>(){})
```




- TypeReference
- 제이쿼리 ajax 로딩바
```
  $.ajaxSetUp에서 한번에 할수 있다.
 ```

### 2022.03.11
- mybatis SelectKey return값 1이 나오는 이유
  [참고링크](https://velog.io/@ctp102/mybatis-selectKey-return%EA%B0%92%EC%9D%B4-1%EC%9D%B4-%EA%B3%84%EC%86%8D-%EB%82%98%EC%98%A4%EB%8A%94-%EC%9D%B4%EC%9C%A0)
- Spring @ResponseBody

### 2022.03.15
- postgresql 소숫점 2자리
- postgresql 나누기 할때는 자료형 numeric 바보같이 소수점까지 필요한데 integer로 했음.
- spring c: forEach spring form:select

### 2022.03.16
- JPA 정의 

### 2022.03.17
- dbever primary key 추가 
- insert 한번에 넣는게 빠르다. 결국 해결 못함. 
- https://dev.dwer.kr/2020/04/mysql-bulk-inserting.html
- https://d2.naver.com/helloworld/1155

### 2022.03.18
- 오라클 level
- [postgresql-document](https://www.postgresql.org/files/documentation/pdf/10/postgresql-10-A4.pdf)
- 함수안에서 for문 돌리던거   
  generate_series 함수 사용해서 계산하는 쿼리 만들어서   
  insert 해줬더니 엄청 빨라졌다.

### 2022.03.29
- limit
- abs 절대값 
### 2022.05.05
```
Elements in iteration expect to have 'v-bind:key' directives  vue/require-v-for-key
```
- v-bind:key v-for을 사용할때는 v-bind:key 속성을 추가해줘야한다.


### 2022.05.16
-export import {} 중괄호 의미
```
  자바스크립트
  export import {} 중괄호 의미
  export { vue };
  export const Vue =3;
  export default vue;
  default가 붙어 있지 않은 변수는 다 괄호를 붙여야한다.  
```
- vuex
1. state
2. getters
3. mutations

### 2022.05.17
- axios (액시오스)
- : 뷰에서 권고하는 Promise 기반의 HTTP 통신 라이브러리

- 액시오스 응답제어
- .then
- : 비동기 통신이 성공했을 경우, .then()은 콜백을 인자로 받아 결과값을 처리할수 있다.
- .catch
- : .catch를 통해 오류를 처리한다.

- 액시오스 http 요청 메서드 종류
1. axios.get(url[,conpig)
   : 서버에서 데이터를 가져올 때 사용하는 메서드
     두 번째 파라미터 config 객체에는 헤더(header),응답초과시간(timeout),인자값등의
     요청 값을 같이 넘길 수 있다.
2. axios.post(url[,data[,config]])
   : 서버에서 데이터를 새로 생설할떄 사용하는 메서드 
3. axios.pust(url[,data[,config]])
   : 특정 데이터를 수정할 때 요청하는 메서드 put은 새로운 리소스를 생성하거나
     이미 존재하는 데이터를 대체할 때 사용됩니다. post와의 다른점은 post는 여러번
     호출할 경우, 새로운 데이터가 지속적으로 추가됩니다. 반면 put은 한번 요청하거나 
     여러 번 지속적으로 요청해도 결과값이 동일하다
4. axios.delete(url[,data[,config]])
   : 특정 데이터나 값을 삭제할때 요청하는 메서드