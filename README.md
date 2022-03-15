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


  >ObjectMapper.readValue( arg, type )
  arg: 변환대상
  type: 대상을 어떤 타입으로 변환할것인지 명시한다. JavaClass 혹은 Class객체, TypeReference객체가 올 수 있다.
  ex)mapper.readValue(arg, ArrayList.class);
  mapper.readValue(arg, new ArrayList<HashMap<String, String>>().getClass())
  mapper.readValue(arg, new TypeReference<ArrayList<HashMap<String, String>>>(){})




- TypeReference
- 제이쿼리 ajax 로딩바 
> $.ajaxSetUp에서 한번에 할수 있다.
> 
> 
>
### 2022.03.11
- mybatis SelectKey return값 1이 나오는 이유
  [참고링크](https://velog.io/@ctp102/mybatis-selectKey-return%EA%B0%92%EC%9D%B4-1%EC%9D%B4-%EA%B3%84%EC%86%8D-%EB%82%98%EC%98%A4%EB%8A%94-%EC%9D%B4%EC%9C%A0)

### 2022.03.15
