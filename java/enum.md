## 💡 Enum

#### Enum이란?
- Enum은 열거형이라고 불리며, 서로 연관된 상수들의 집합을 의미한다.
#### Enum의 장점
- 코드가 단순해지며, 가독성이 좋다.
- 인스턴스 생성과 상속을 방지하여 상수값의 타입 안정성 보장
- 키워드 enum을 사용하기 때문에 구현의 의도가 열거임을 분명하게 알 수 있다.
- 허용 가능한 값들을 제한할수 있다.

### Enum 예제
```java
public class EnumExam {
	// 기존에 상수를 정의하는 방법
	public static final String MALE = "MALE";
	public static final String FEMALE = "FEMALE";

	public static void main(String[] args) {
		String gender1;
		gender1 = EnumExample.MALE;
		gender1 = EnumExample.FEMALE;
		// MALE, FEMALE이 아닌 상수 값이 할당 될 때 //컴파일시 에러가 나지 않음. -> 문제점 발생.
		gender1 = "boy";  
		Gender gender2;
		gender2 = Gender.MALE;
		gender2 = Gender.FEMAL;
		// 컴파일 시 의도하지 않는 상수 값을 체크할 수 있음.
		// Enum으로 정의한 상수값만 할당 받을 수 있음.
		gender2 = "boy";
	}
}

// enum class를 이용해 Gender라는 새로운 상수들의 타입을 정의한다.
enum Gender { 
	MALE,
	FEMAL; 
}

```
- 상수를 사용하면 우리가 기대하지 않는 상수값이 들어왔을 때를 대비 할 수 없다.
- 즉 컴파일시 우리가 기대하지 않은 상수값의 할당을 사전에 체크 할 수 있다.



### 참고문서 
[우아한블로그](https://rangken.github.io/blog/2015/effective-java-5/)