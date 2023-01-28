# cleancode_study_repo
#### 클린코드 공부 저장소
>##### 추천 책
- effect java
- clean code
- refactoring

>##### 소트웍스 앤솔러지 책에서 다루고 있는 내용으로 객체지향 프로그래밍을 잘 하기 위한 9가지 원칙
- 규칙 1: 한 메서드에 오직 한 단계의 들여쓰기(indent)만 한다.
- 규칙 2: else 예약어를 쓰지 않는다.
- 규칙 3: 모든 원시값과 문자열을 포장한다.
- 규칙 4: 한 줄에 점을 하나만 찍는다.
- 규칙 5: 줄여쓰지 않는다(축약 금지).
- 규칙 6: 모든 엔티티를 작게 유지한다.
- 규칙 7: 3개 이상의 인스턴스 변수를 가진 클래스를 쓰지 않는다.
- 규칙 8: 일급 콜렉션을 쓴다.
- 규칙 9: 게터/세터/프로퍼티를 쓰지 않는다.

>##### 경험할 객체지향 생활 체조 원칙
- 규칙 1: 한 메서드에 오직 한 단계의 들여쓰기만 한다.
- 규칙 2: else 예약어를 쓰지 않는다.
- 규칙 3: 모든 원시값과 문자열을 포장한다.
- 규칙 5: 줄여쓰지 않는다(축약 금지).
- 규칙 8: 일급 콜렉션을 쓴다.

- 규칙 4: 한 줄에 점을 하나만 찍는다.
- Clean Code 가이드의 디미터 법칙을 지키는 것을 의미한다.
- 규칙 6: 모든 엔티티를 작게 유지한다.
- 규칙 7: 3개 이상의 인스턴스 변수를 가진 클래스를 쓰지 않는다.
- 규칙 9: 게터/세터/프로퍼티를 쓰지 않는다.


# 책임주도설계
- 프로그래밍의 팩임을 갖고 책임을 수행할 적절한 객체르 찾아 책임을 할당하는 방식으로 협력을 설계하는 방법
>##### 책임이란 ?
- 객체이 의해 정의되는 응집도 있는 행위의 집합으로,
- 객체가 유지해야 하는 정보와 수행할 수 있는 행동 에 대해 개략적으로 서술한 문장이다.
- 객체가 '무엇을 알고 있는가'와 ' 무엇을 할 수 있는가' 로 구성된다.

>##### 하는것
- 객체를 생성하거나 계산을 수행하는 등의 스스로 하는 것
- 다른 객체의 행동을 시작시키는 것
- 다른 객체의 활동을 제어하고 저절하는 것

>##### 아는것 
- 사적인 정보에 관해 아는 것
- 관련된 객체에 대해 아는 것
- 자신이 유도하거나 계싼할 수 있는 것에 관해 아는 것

 
 >##### PR 피드백 관련 정리
 - [AssertJ](https://www.baeldung.com/introduction-to-assertj)
 - [AssertJ Exception Assertions](https://www.baeldung.com/assertj-exception-assertion)
 - [오라클 자바 튜토리얼](https://docs.oracle.com/javase/tutorial/java/index.html)
 - [클래스 상수](https://djkeh.github.io/articles/Why-should-final-member-variables-be-conventionally-static-in-Java-kor/)
 - [클린코드 관련 깃헙 블로그](http://amazingguni.github.io/blog/)
 - [캡슐화](https://javacpro.tistory.com/31)
 - [무인자 제네릭 자료형](https://itstory.tk/entry/%EC%9D%B4%ED%8E%99%ED%8B%B0%EB%B8%8C-%EC%9E%90%EB%B0%94-%EA%B7%9C%EC%B9%9923-%EC%83%88-%EC%BD%94%EB%93%9C%EC%97%90%EB%8A%94-%EB%AC%B4%EC%9D%B8%EC%9E%90-%EC%A0%9C%EB%84%A4%EB%A6%AD-%EC%9E%90%EB%A3%8C%ED%98%95%EC%9D%84-%EC%82%AC%EC%9A%A9%ED%95%98%EC%A7%80-%EB%A7%88%EB%9D%BC)
 
 - [자바 코드컨벤션 (en)](https://google.github.io/styleguide/javaguide.html)
 - [자바 코드컨벤션 (kr)](https://myeonguni.tistory.com/1596)
 
 - [@ParameterizedTest](https://www.baeldung.com/parameterized-tests-junit-5) 
 - [@NullAndEmptySource](https://www.baeldung.com/junit-5)
 
 - [enum](https://woowabros.github.io/tools/2017/07/10/java-enum-uses.html)
 - [enum cache]( https://pjh3749.tistory.com/279)
 
 - [optional](https://www.baeldung.com/java-optional) 