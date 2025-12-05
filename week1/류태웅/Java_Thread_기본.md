# Java Thread 기본

## 학습 자료 링크
https://velog.io/@victoryu/Java-Thread-Basics

## 학습 세 줄 요약
1. Thread는 하나의 프로세스 내에서 동시에 실행되는 독립적인 실행 흐름으로, 메모리와 자원을 공유하며 GUI 반응성 향상, 멀티코어 활용, 비동기 처리 등의 이점을 제공한다.
   <br><br>
2. Java에서 Thread.start()를 호출하면 JVM이 새로운 Thread를 생성하고 내부적으로 run() 메서드를 실행시키며, 이 과정은 Java 레벨의 start0() → JVM_StartThread → Thread::start → os::start_thread를 거쳐 실제 OS Thread가 생성된다.
   <br><br>
3. 멀티 Thread 환경에서는 여러 Thread가 공유 데이터에 접근할 때 반드시 synchronized나 volatile을 사용하여 동기화해야 하며, 그렇지 않으면 데이터 불일치나 race condition이 발생할 수 있다.

---

**학습 날짜**: 2025-12-06  
**작성자**: 류태웅
