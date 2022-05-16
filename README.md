# TIL
Today I Learned / 배운 것 기록하기

##22.03.01



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
- Spring @ResponseBody

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