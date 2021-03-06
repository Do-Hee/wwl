# [item 45] 스트림은 주의해서 사용하라 
### 사전 조사 
- 스트림
  - 데이터 원소의 유한 혹은 무한 시퀀스(일련의 연속적인 사건들)를 의미
  - 컬렉션, 배열, 파일, 정규표현식 패턴 매처, 난수 생성기, 다른 스트림 
  - 스트림 안의 데이터 원소들은 객체 참조나 기본 타입 값 (int, long, double - 세 가지)
  - 재사용 불가 

- 스트림 파이프라인
  - 이 원소들로 수행하는 연산 단계를 표현하는 개념 
  - 여러 개의 스트림이 연결되어 있는 구조 
   ```java
   emps.stream().filter(x -> x.getSalary()>100).count();
      // 스트림생성       중개연산(스트림 변환)     종단연산(스트림 사용)
   ```
  - [중간, 종단 연산의 예](https://m.blog.naver.com/PostView.nhn?blogId=spdlqjdudghl&logNo=220757598355&proxyReferer=https%3A%2F%2Fwww.google.com%2F)
  - 중간 연산(intermediate operation)
    - 모두 한 스트림을 다른 스트림으로 변환
    - 지연 연산(Lazy Evaluation)을 한다.
     ```java
      Stream<String> a = names.stream().filter(x -> x.contains("o")).map(x-> x.concat("s"));
      a.forEach(x -> System.out.println(x));
     ```
      - 위와 같은 코드가 있으면 위에 filter와 map 함수는 미리 계산하고 있지 않고 있다가 forEach와 같은 최종연산이 적용될 때 중개 연산도 실행된다.
      - 이로써 얻는 장점은 미리 계산하면서 두 번 순회하는 짓을 안할 수 있게 된다는 점이다.
      - [https://jeong-pro.tistory.com/165](https://jeong-pro.tistory.com/165)
  - 플루언트 인터페이스
    - 메소드 체이닝을 지원하는 디자인 패턴
    - 가독성 높은 객체지향 API 구현 가능

- `computeIfAbsent()`
 ```java
  default V computeIfAbsent(K key,
          Function<? super K, ? extends V> mappingFunction) {
    Objects.requireNonNull(mappingFunction);
    V v;
    if ((v = get(key)) == null) {
        V newValue;
        if ((newValue = mappingFunction.apply(key)) != null) {
            put(key, newValue);
            return newValue;
        }
    }

    return v;
  }
 ```
  - 각 키에 다수의 값을 매핑하는 맵을 쉽게 구현 가능

- 스트링으로 처리하기 어려운 경우
  - Ex) 한 데이터가 파이프라인의 여러 단계를 통과할 때 이 데이터릐 각 단계에서의 값들에 동시에 접근하기는 어려운 경우 
  - 스트림 파이프라인은 일단 한 값을 다른 값에 매핑하고 나면 원래의 값은 잃는 구조 

-   [Fluent API](https://zetawiki.com/wiki/%ED%94%8C%EB%A3%A8%EC%96%B8%ED%8A%B8_%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4,_%EB%A9%94%EC%86%8C%EB%93%9C_%EC%B2%B4%EC%9D%B4%EB%8B%9D)
    -   메소드 체이닝을 지원하는 디자인 패턴
    -   가독성 높은 객체지향 API 구현 가능

```java
class Person {
	private String name;
	private int age;

	public Person setName(String name) {
		this.name = name;
		return this;
	}

	public Person setAge(int age) {
		this.age = age;
		return this;
	}

	public void introduce() {
		System.out.println("Hello, my name is " + name + " and I am " + age + " years old.");
	}

	public static void main(String[] args) {
		Person person = new Person();
		person.setName("Peter").setAge(21).introduce();
		// Hello, my name is Peter and I am 21 years old.
	}
}
```

-   [Lazy Evaluation](https://knight76.tistory.com/entry/%ED%8E%8C-lazy-evaluation%EB%8A%90%EA%B8%8B%ED%95%9C-%EA%B3%84%EC%82%B0%EB%B2%95%EC%97%90-%EB%8C%80%ED%95%9C-%EC%A2%8B%EC%9D%80-%EC%84%A4%EB%AA%85-%EA%B7%B8%EB%A6%BC-%EC%9E%90%EB%A3%8C)


---

### 스터디 요약 
- 

---

> :leftwards_arrow_with_hook:[EffectiveJava3E](/EffectiveJava3E/README.md)

