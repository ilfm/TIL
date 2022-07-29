# 👨‍💻 Today I Learned
Today I Learned / 배운 것 기록하기

## 2022.03.02
- javax.servlet.jsp.jsptagexception no message found under code
- PostgreSQL 테이블 좌우로 합치기
  https://greendreamtrre.tistory.com/683
  
- 마이바티스 시퀀스 넣기
```
<selectKey keyProperty="newSeq" resultType="int" order="BEFORE">
  
</selectKey>
```

## 2022.03.04
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

## 2022.03.11
- mybatis SelectKey return값 1이 나오는 이유
  [참고링크](https://velog.io/@ctp102/mybatis-selectKey-return%EA%B0%92%EC%9D%B4-1%EC%9D%B4-%EA%B3%84%EC%86%8D-%EB%82%98%EC%98%A4%EB%8A%94-%EC%9D%B4%EC%9C%A0)
- Spring @ResponseBody

## 2022.03.15
- postgresql 소숫점 2자리
- postgresql 나누기 할때는 자료형 numeric 바보같이 소수점까지 필요한데 integer로 했음.
- spring c: forEach spring form:select

## 2022.03.16
- JPA 정의 

## 2022.03.17
- dbever primary key 추가 
- insert 한번에 넣는게 빠르다. 결국 해결 못함. 
- https://dev.dwer.kr/2020/04/mysql-bulk-inserting.html
- https://d2.naver.com/helloworld/1155

## 2022.03.18
- 오라클 level
- [postgresql-document](https://www.postgresql.org/files/documentation/pdf/10/postgresql-10-A4.pdf)
- 함수안에서 for문 돌리던거   
  generate_series 함수 사용해서 계산하는 쿼리 만들어서   
  insert 해줬더니 엄청 빨라졌다.

## 2022.03.29
- limit
- abs 절대값 
## 2022.05.05
```
Elements in iteration expect to have 'v-bind:key' directives  vue/require-v-for-key
```
- v-bind:key v-for을 사용할때는 v-bind:key 속성을 추가해줘야한다.


## 2022.05.16
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

## 2022.05.17
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


- Promise란?
- : 비동기 함수를 동기 처리하기 위해 고안한 객체


## 22.05.18
### webpack이란?
> 웹팩의 4가지 주요속성
: 웹팩의 빌드(파일변환)과정을 이해하기 위해서 4가지 주요속성을 알고 있어야한다.
1. entry
    - entry 속성은 웹팩에서 웹 자원을 변환하기 위해 필요한 최초진입점이자 자바스크립트 파일 경로 
    - 웹 애플리케이션의 전반적인 구조와 내용이 담겨져 있어야 합니다. 
    - 웹팩이 해당 파일을 가지고 웹 애플리케이션에서 사용되는 모듈들의 연관 관계를 이해하고 분석하기 때문에 애플리케이션을 동작시킬 수 있는 내용들이 담겨져 있어야 합니다.
2. output
    - 웹팩을 돌리고 난 결과물의 파일 경로는 의미한다.
3. loader
   - 로더(Loader)는 웹팩이 웹 애플리케이션을 해석할 때 자바스크립트 파일이 아닌 웹 자원(HTML, CSS, Images, 폰트 등)들을 변환할 수 있도록 도와주는 속성입니다.
4. plugin
   - 플러그인(plugin)은 웹팩의 기본적인 동작에 추가적인 기능을 제공하는 속성입니다. 로더랑 비교하면 로더는 파일을 해석하고 변환하는 과정에 관여하는 반면, 플러그인은 해당 결과물의 형태를 바꾸는 역할을 한다고 보면 됩니다.
 
### enum?
[enum][https://techblog.woowahan.com/2527/]

## 22.05.19
### Assertions
#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;AssertJ란?
- 테스트코드를 작성 할 때 풍부한 문법을 제공하여 테스트 코드를 쉽고 가독성 높게 작성할수 있도록 도와주는 자바라이브러리

> https://assertj.github.io/doc/
> https://pjh3749.tistory.com/241

### @BeforeEach


## 22.05.20
### return문
- 표현식의 평가 결과를 반환한다.
- 함수안에 많이 사용되고 아무 곳이나 사용가능
- 함수안에서 사용될 때 return이 표현식 안쓰면 undefined를 반환한다.
### 빌트인

### 인스턴스의 프리미티브 값

## 22.05.23
### new 연산자
#### new연산자 사용 시 순서
1.새로운 빈 오브젝트 생성
2. this를 새롭게 생성된 오브젝트에 바인딩
3. 새롭게 생성된 오브젝트 프로퍼티에 proto라고 불리는 생성자 함수의 프로토타입 오브젝트를 추가합니다.
4. 함수에서 완성된 오브젝트가 반환될 수 잇도록, return this를 함수의 맨마지막 부분에 추가합니다.

==> 결론적으로 new 연산자를 사용하여 객체를 생성하면 인스턴스가 생성되면서 proto에 프로퍼티와 메소드가 상속된다.
### String
#### length 로 보는 자바스크립트 엔진
```
    "123".length는 어떻게 가능한걸까?
    "123"은 오브젝트가 아니라 프리미티브 값인데
    자바스크립트 엔진이 .length를 만나게 되면 내부에서
    new String("123")를 하게 되며, 생성한 인스턴스의 
    length값인 3을 반환하게 된다. 

```
#### "" vs String() .toString()이 필요한 이유와 js 함수 호출구조
- 다시 듣기 

## 22.05.24
### 자바스크립트 객체
```
    ○ 자바스크립트 오브젝트
       1. 빌트인 오브젝트 
          - 사전에 미리 만들어 놓은 오브젝트
          - ex) Number, String
       2. 네이티브 오브젝트
          - js스펙에서 정의한 오브젝트, 빌트인 오브젝트
          - 애플리케이션의 환경과 관계없이 항상 사용가능하다.
       3. 호스트 오브젝트
          - 네이티브 오브젝트를 제외한 오브젝트 
          - 실행 환경에 따라 정의된 오브젝트(OS,Web browser에 따라 제공 객체가 달라진다.)
        
        ※ 빌트인 오브젝트 좀더 공부하기 __proto__

```
### Spring @DisplayName 
#### context.getBean(beanName ,Type)
#### .class의 의미


## 22.05.25
### function 
####함수형태
  - 함수 선언문
  - 함수 표현식
### Arguments Object
  - 함수 호출 시 , 전달인자들이 배열 형태로 저장된 객체로
    함수 호출시 전달인자와 함께 arguments 객체가 함수 내부로 전달된다.
  - 주로 파라미터가 유동적인 함수 구현 시 사용된다.
  - 유사배열객체로 배열로 변화하려면 Array.prototype.slice.call(arguments);
  - 자바스크립트는 유연한 언어로 함수를 호출할 때 파라미터 형식을 맞추지 않아도 에러가 나지 않는다.

###Spring


### 22.05.26
#### Global , window


#### 싱글톤 패턴, 싱글톤 컨테이너

### 22.05.31
#### 네비게이션 가드 (navigation guard)
- 네비게이션 가드랑 뷰 라우터로 특정 url에 접근할 때 해당 url의 접근을 막는 방법을 말한다.
- 예를들어, 사용자의 인증정보가 없으면 특정 페이지에 접근 하지 못하게 할때 사용하는 기술

#### 네비게이션 가드의 종류
- 애플리케이션 전역에서 동작하는 전역가드
- 특정 url에서만 동작하는 라우터가드
- 라우터 컴포넌트 안에 정의하는 컴포넌트 가드

#### 전역가드
- 전역 가드는 라우터 인스턴스를 참조하는 객체로 설정 할 수 있습니다.
```javascript 

router.beforeEach(function (to,from,next){
    // to : 이동할 url
    // from : 현재 url
    // next : to에서 지정한 url로 이동하기 위해 꼭 호출해야하는 함수
});
```
- router.beforeEach()를 호출하면 모든 라우팅이 대기 상태가 됩니다.
- 원래 url 변경되고 나면 해당 url 따라 화면이 자연스럽게 전환되어야하는데 전역 가드이기 떄문에 화면이 전화되지않음
- 해당 url로 라우팅 하기 위해서 next()를 호출해야한다.

#### 라우터 가드
- 전체 라우팅이 아니라 특정 라우팅에 대해서 가드를 설정하는 방법 
```javascript
var router = new VueRouter({
    routes:[{
        path: '/login',
        component : Login,
        beforeEnter : function (to, from, next){        
            // 로직 추가
        }
    }]
});
```

#### 컴포넌트 가드
- 라우터로 지정된 특정 컴포넌트에 가드를 설정하는 방법은 다음과 같다.
```javascript
const Login ={
    template: '<p>Login Component</p>',
  beforeRouteEnter (to, from, next) {
    // Login 컴포넌트가 화면에 표시되기 전에 수행될 로직
    // Login 컴포넌트는 아직 생성되지 않은 시점
  },
  beforeRouteUpdate (to, from, next) {
    // 화면에 표시된 컴포넌트가 변경될 때 수행될 로직
    // `this`로 Login 컴포넌트를 접근할 수 있음
  },
  beforeRouteLeave (to, from, next) {
    // Login 컴포넌트를 화면에 표시한 url 값이 변경되기 직전의 로직
    // `this`로 Login 컴포넌트를 접근할 수 있음
  }
}


}

```

###22.06.07
#### @EnableWebSecurity
#### @EnableGlobalMethodSecurity

### 22.06.14
#### vue created mounted 차이

### 22.06.24
- 로그인 폼은 사용자가 아이디 패스워드를
  넣고 전송을 하면 전송하기 전에 중간에 
  자바스크립트가 가로챈다.
  

### 22.07.11
- export , export default 차이
  https://shinejaram.tistory.com/41
  https://m.blog.naver.com/gi_balja/221227430979
  

- vue3 setup()
### 22.07.19
- vue watch 객체안에 있는 데이터 감지
  https://codingcoding.tistory.com/337
  
- 자바스크립트 템플릿 리터럴 (template Literal)
```
    백틱(`) 사용  
```

### 22.07.21
- vue ref는 언제 사용할까?
  https://riviere.tistory.com/92
  
  

### 22.07.22
- vue filters
  https://sunny921.github.io/posts/vuejs-filter/

### 22.07.27
 vue project 생성
 https://blog.naver.com/PostView.naver?blogId=hj_kim97&logNo=222458611638
- element-ui 설치
 https://velog.io/@kimy/vuejs-elementUI-%EC%84%A4%EC%B9%98%ED%95%98%EA%B8%B0
 

### 22.07.28
- 전역 properties
https://kr.vuejs.org/v2/cookbook/adding-instance-properties.html
  

### 22.07.29
- vue 뒤로가기
  https://velog.io/@keywookim/B.TIL-05-history%EB%A5%BC-%EC%9D%B4%EC%9A%A9%ED%95%9C-%EC%BB%B4%ED%8F%AC%EB%84%8C%ED%8A%B8-%EC%9D%B4%EB%8F%99%EB%92%A4%EB%A1%9C%EA%B0%80%EA%B8%B0-%EB%93%B1
  지금 프로젝트에서 라우터로 이동하는게 아니라 v-if show 형식이어서  
