# JVM (Java Virtual Machine)

## 학습 자료 링크
https://velog.io/@victoryu/JVM-Java-Virtual-Machine

## 학습 세 줄 요약
1. JVM은 Java 바이트코드(.class 파일)를 플랫폼에 맞게 해석 및 실행하는 관리형 런타임 환경으로, "Write once, run everywhere"를 실현하며 메모리 관리와 보안 검사 등의 역할을 수행한다.

2. Runtime Data Area는 PC Register(현재 실행 중인 명령어 주소), JVM Stack(지역 변수와 메서드 호출 관리), Heap(객체와 배열 저장), Method Area(클래스 구조와 상수 풀), Native Stack(네이티브 메서드 실행)으로 구성되며, Heap과 Method Area는 모든 스레드가 공유하고 나머지는 스레드별로 독립적으로 생성된다.

3. Heap은 Garbage Collector에 의해 자동으로 메모리가 관리되는 객체 저장 공간이며, Method Area는 클래스별 구조(런타임 상수 풀, 필드/메서드 데이터, 메서드 코드)를 저장하고, 각 영역은 동적 확장이 가능하며 메모리 부족 시 OutOfMemoryError나 StackOverflowError를 발생시킨다.

---

**학습 날짜**: 2025-12-19  
**작성자**: 류태웅