# [2019.05.26] Effective Java 3/E 스터디 진행 - 6주차
참석자: Delf, Doy, Hee, Nesoy
## 주제
- [**아이템 70.**](../chapter10/item70.md) 복구할 수 있는 상황에는 검사 예외를, 프로그래밍 오류에는 런타임 예외를 사용하라 
- [**아이템 71.**](../chapter10/item71.md) 필요 없는 검사 예외 사용은 피하라 
- [**아이템 72.**](../chapter10/item72.md) 표준 예외를 사용하라 
- [**아이템 73.**](../chapter10/item73.md) 추상화 수준에 맞는 예외를 던지라 
- [**아이템 74.**](../chapter10/item74.md) 메서드가 던지는 모든 예외를 문서화하라 
- [**아이템 75.**](../chapter10/item75.md) 예외의 상세 메시지에 실패 관련 정보를 담으라 

## 아이템 분담
- Delf: 72, 73
- Doy: 70, 71
- Hee: 74, 75
- Nesoy: 70, 71

## 주요 이슈

#### item 72
- 예외를 상속하여 직접 구현한 커스텀 예외(클래스)에 대하여
  - 표준 예외를 확장하는 것은 좋으나, 부담이 될 수 있다.
    - 예외도 직렬화가 가능하고, 직렬화는 부담이 되기 때문?