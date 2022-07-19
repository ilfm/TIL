### 📘 INDEX



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

### 2022.03.29
- limit
- abs 절대값 
### 2022.04.12
```
- 객체 지향의 핵심 
1. 다형성

- 다형성의 실세계 비유
1. 역할과 구현을 분리 
- 역할과 구현으로 세상을 구분하면
단순해지고, 유연해지며 변경도 편리해진다.
장점: 클라이언트는 대상의 역할(인터페이스)만 알면된다.
     클라이언트는 구현 대상의 내부구조를 몰라도된다.
     클라이언트는 구현 대상의 내부구조가 변경되어도 영향 받지 않는다.
     클라이언트는 구현 대상 자체를 변경해도 영향을 받지 않는다.
2. 유연하고 변경 용이하다
- 자동차 - 운전자 
자동차 k3 -> 아반떼로 바꿔도
운전 가능 자동자 역할에만 의존하기 떄문에
클라이언트가 자동자의 구조를 알 필요가 없어
내부적으로 바껴도 상관없어 
역할과 구현으로 했기 때문에 
클라이언트를 바꿀 필요가 없어

자바 언어의 다형성
- 오버라이딩 떠올려보자

다형성의 본질
- 인터페이스를 구현한 객체 인스턴스를 실행 시점에 유연하게 변경할 수 있다.
- 다형성의 본질을 이해하려면 협력이라는 객체사이의 관계에서 시작해야함
- 클라이언트를 변경하지않고, 서버의 구현 기능을 유연하게 변경할 수 있다.



```
### 2022.04.13
```
vue 에서 함수와 메소드 차이
메소드 어딘가에 속해잇는 함수를 메소드라고한다.
화살표 함수는 this가 바인딩 되지않는다.

v-on을 사용해서 이벤트를 받아온다.
예) v-on:click='add'
    @click='add'

componet 
costum tag를 만드는
Vue.component('product',{
    props : ['image','title','discription','avatar']
    template:
      <div>
      
      
      </div>
    });

```





### java
- [enum](https://github.com/ilfm/TIL/blob/master/java/enum.md)
### Spring
 - [spring container](https://github.com/ilfm/TIL/blob/master/spring/spring-container.md)
### Javascript
 - function 
 - Arguments
### 알고리즘
 - [greedy]
