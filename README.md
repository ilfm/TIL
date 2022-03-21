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
  JSON타입의 값을 맵 형태로 변환

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

### 2022.03.21
