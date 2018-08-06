# 실용주의 프로그래머
#### 자신의 기술에 관심과 애정을 가져라.
#### 자신의 일에 대해 생각하면서 일하라.
#### 어설픈 변명을 만들지 말고 대안을 제시하라.
#### 깨진 창문을 내버려두지 말자.
- 발견하자마자 바로 고쳐라.
#### 변화의 촉매가 되라
- 허락을 얻는 것보다 용서를 구하는 것이 쉽다.
#### 큰 그림을 기억하라.
#### 품질을 요구사항으로 만들어라.
- 자신이 한 것을 비판적인 눈으로 보기 위해 늘 뒤로 물러서서 보자.
- 완벽해지기란 불가능하다.
#### 지식 포트폴리오에 주기적으로 투자하라.
- 주기적으로 노력하는 습관
- 다양한 분야에 투자할 것.
- 보수적인 투자. 위험성이 큰 투자. 보상이 높은 사이에서 균형을 잘 맞춘다.
- 주기적으로 재검토하고 재조정해야 한다.
- 목표
    - 매년 새로운 언어를 최소 하나를 배우기.
    - 기술 서적을 분기마다 한 권씩 읽기.
    - 비 기술 서적도 읽기
    - 수업을 듣거나 지역 사용자 모임에 참여하기
    - 다른 환경에서 실험해보기.
    - 흐름을 놓치지 말기.
#### 읽고 듣는 것을 비판적으로 분석하라.
- 읽거나 듣는 것에 대해 비판적으로 생각하는 것.
- 누군가 좋은 자리를 차지하려고 돈을 지불했을 수 있다.
#### 무엇을 말하는가와 어떻게 말하는가 모두 중요하다.
- WISDOM
    - What - 무엇을 배우길 원하는가?
    - Interest - 말하려는 것에서 그들이 관심 있어 하는 건 무엇인가?
    - Sophisticated - 얼마나 소양이 있는가?
    - Detail - 어느 정도의 구체적인 내용을 원하는가?
    - Owe - 누가 정보를 소유하길 원하는가?
    - Motivate - 그들이 경청하도록 동기를 주려면 어떻게 해야 할까?

#### DRY - Don't Repeat Yourself
- 낮은 차원의 지식은 그것이 속하는 코드에 두고 주석은 다른 높은 차원의 설명을 위해 아껴두자.
- 돌아가는 길이 지름길이다.
    - 지금 당장 몇 초를 절약할 수 있을지라도, 나중에는 몇 시간을 잃게 될런지 모른다.

#### 재사용하기 쉽게 만들라.
- 재사용이 쉽지 않다면 사람들은 사용하지 않을 것이다. 실패한다면 지식 중복의 위험을 각오해야 한다.

#### 관련 없는 것들 간에 서로 영향이 없도록 하라.
- 직교적인 시스템을 만들자.
- 변화가 Localize되서 개발 시간과 테스트 시간이 줄어든다.
- 감연된 코드는 격리된다.
- 시스템이 잘 깨어지지 않는다.
- 코드의 결합도를 줄여라
    - Write Shy Code
    - Law of Demeter
- 전역 데이터를 피하라.
    - 싱글톤 객체를 전역 데이터의 일종으로 사용하지 말자. 불필요한 링크를 제거하자.
- 유사한 함수를 피하라.
- 항상 자신이 작성하는 코드를 항상 비판적으로 검토해 보는 습관을 기르자.


#### 최종 결정이란 없다.
> 당신이 가진 생각이 딱 하나밖에 없다면, 그것만큼 위험한 것은 없다.
- 여러분의 코드는 몇 가지 가능한 미래를 지원할 수 있는가?
- 어떤 미래가 일어날 가능성이 높을까? 그 미래가 닥쳤을 때, 이를 지원하는 것이 얼마나 어려울까?


#### 목표물을 찾기 위해 예광탄을 써라
- 예광탄 코드는 나중에 버리려고 만드는 것이 아니다.
    - 재사용한다. 완전한 기능이 들어있지 않을 뿐.
    - 필요하다면 조정도 할 수 있다.
- 프로토타이핑
    - 위험을 수반하는 모든 것이다.

#### 프로토타입을 통해 학습하라
- 무시해도 좋은 세부사항
    - 정확성
    - 완전성
    - 안정성
    - 스타일
- 빠르게 만들고 잠재적 문제 지점을 발견하자.


#### 문제 도메인에 가깝게 프로그래밍하라.
- 더 높은 추상화 수준에서 작업함으로써 사소한 구현의 세부사항들을 무시하고 도메인의 문제들을 푸는 일에만 정신을 집중할 수 있다.


#### 추정을 통해 놀람을 피하라
- 얼마나 정확한 것이 충분히 정확한 것인가?
    - 자신에게 물어봐야 할 첫 번째 질문은 여러분의 답변이 사용될 상황이다.
- 이미 그 일을 해본 사람에게 물어보라는 것이다.
- 그들이 어떻게 문제를 해결했는지 이해하려 노력해보자.
- 상대방이 무엇을 묻고 있는지에 대해 이해하는 것.
- 추정을 하기 전에 미리 생각하는 습관을 기르는 것이 좋다.
- 추정치를 잘못되었더라도 움츠리거나 도망가지 마라. 왜 여러분의 추측과 실제 값이 달라졌는지 원인을 찾아야 한다. 시간을 들여 이를 규명하라. More better than yesterday

#### 코드와 함께 일정도 반복하며 조정하라

#### 지식을 일반 텍스트로 저장하라
- 유닉스 철학
    - 작고 예리한 각각의 도구가 한 가지 일만 잘 하도록 만들자는 철학

#### 명령어 셸의 힘을 사용하라
- 셸 명령은 이해하기 어렵거나 너무 불친절해 보일런지도 모르겠지만, 이것들은 강력하고 간결하다.

#### 하나의 에디터를 잘 사용하라
- 모든 기능을 사용해보자.

#### 언제나 소스코드 관리 시스템을 사용하라.
- 진보라는 것은 변화와는 걸리가 멀고 오히려 기억에 의존한다. 과거를 기억하지 못하는 사람은 과거를 반복할 운명이다.


#### 비난 대신 문제를 해결하라
- 버그가 여러분의 잘못인지 다른 사람의 잘못인지는 그리 중요한 게 아니다. 버그를 해결하는게 중요하다.

#### 디버깅을 할 때 당황하지 마라.
- 가장 속이기 쉬운 사람은 자기 자신이다.
- 표면에 보이는 증상만 고치려는 욕구에 저항하라. 실제 문제는 여러분이 관찰하고 있는 것에서 몇 단계 떨어져 있고, 또 다른 여러 가지와 연관되어 있을 확률이 다분하다.
- 항상 문제의 근본적인 원인을 발견하려고 노력하고, 그 문제의 특정한 증상만 고치려고 하지 말라.
- 버그상황을 재현하도록 노력하자.
- 데이터를 가시화하라
- Tracing
- 고무오리 : 누군가에게 문제를 설명하게 되면 혼자 코드를 살펴 볼 때는 당연히 여기고 지나갈 것을 명시적으로 이야기함으로써 깨달음을 얻게 된다.

#### Select는 망가지지 않았다.
- 발굽 모양을 보면 말부터 생각해야지, 얼룩말부터 생각하지는 말자
- OS는 아마 망가지지 않았을 것이며, Database 또한 괜찮을 것이다.

#### 가정하지 마라. 증명하라
- 왜 이 실패가 더 일찍 발견되지 않았을까 생각해볼 필요가 있다.
- 버그를 미리 잡을 수 있도록 단위 테스트나 다른 테스트를 수정할 필요가 있다.
- 누군가가 잘못 내린 가정의 결과라면 다 같이 토론하라.

#### 텍스트 처리 언어를 하나 익혀라
#### 코드를 작성하는 코드를 작성하라
#### 완벽한 소프트웨어는 만들 수 없다.
- 자기 자신 역시 믿지 않는다.
- 완벽한 코드를 작성할 수 없음을 깨닫고 자신의 실수를 대비해 방어적으로 코드를 짠다.