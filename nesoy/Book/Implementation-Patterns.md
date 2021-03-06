## Chapter 1. 소개
- 생각을 하며 프로그래밍하는 것
    - 특정 메소드의 이름을 왜 그렇게 지었는지, 어떤 기능이 왜 특정 객체에 있어야 하는지..
    - 내가 어떤 생각을 하고 있는지 살펴볼 수 있는 여유를 갖는 것.
- 다름 사람들의 중요성을 인정하는 것
- 다른 사람의 존재도 내 존재만큼 중요하다는 생각을 한 후, 생각을 실천으로

### 구성
![No Image](/nesoy/Images/Implementation-Patterns/1.png)

- 소개
    - 커뮤니케이션을 돕는 코드의 중요성, 패턴의 기본 철학
- 클래스
    - 왜, 어떻게 클래스를 생성해야 하는지, 클래스에서 어떤 식으로 로직을 표현해야 하는가?
- 상태
    - 상태를 저장하고 읽어오는 데 관한 패턴
- 행위
    - 로직, alternative path를 표현하는 패턴
- 메소드
    - 여러분의 코드를 읽을 사람은 여러분이 작성한 메소드와 메소드 이름을 보며 어떤 생각을 할 것인가?
- 컬렉션
    - 컬렉션을 선정하고 사용하는 데 관한 패턴
- 발전하는 프레임워크
    - 어떤 식으로 패턴을 변화시켜 사용해야 하는가?




## Chapter 2. 패턴
- 새로 짜는 경우보다 기존 프로그램을 읽는 경우가 많음.
- 완성은 없다. 유지보수 비용이 훨씬 크다.
- 같은 문제에 대한 다른 해결책도 함께 봐야한다. 특정 상황에서 특정 패턴을 사용하는 이유를 알게 되면 문제 해결 능력을 기를 수 있다.
- 패턴은 절대적인 진리가 아니므로, 사람의 의사 결정을 돕는 도구 정도로 생각하는 것이 좋다.



## Chapter 3. 프로그래밍 이론

### 가치
- 훌륭한 프로그래밍에 있어 공통적인 가치
    - 커뮤니케이션, 단순성, 유연성

#### 커뮤니케이션
- 타인을 고려해서 프로그램을 작성하게 되면?
    - 내 코드는 좀더 이해하기 쉽고 깔끔해지며
    - 더 효율적이 되고 생각은 명확해진다.
    - 새로운 관점에서 코드를 바라보게 되고, 스트레스가 줄어들며 읽기 쉬운 코드가 작성된다.
- [Literate Programming](http://www.literateprogramming.com/knuthweb.pdf)

#### 단순성
- 복잡도를 낮추면 프로그램을 읽고 사용하고 수정하는 사람들이 프로그램을 훨씬 빨리 이해할 수 있다.
- 복잡도가 과다하게 높아지면 소프트웨어가 제대로 동작하지 않게 되며, 차후에 소프트웨어 수정도 어려워져서 소프트웨어 가치가 떨어진다.
- 프로그램을 최대한 단순화하라. 의미 없는 코드는 모두 제거하라. 설계시에도 과도한 요소는 모두 빼고, 요구 사항을 분석해서 꼭 필요한 사항만을 뽑아내라.
    - 과도한 단순화가 커뮤니케이션을 저해하는 경우도 있다.
