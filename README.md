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

