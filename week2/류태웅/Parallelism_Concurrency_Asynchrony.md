# Parallelism, Concurrency, Asynchrony

## 학습 자료 링크
https://velog.io/@victoryu/Parallelism-Concurrency-Asynchrony

## 학습 세 줄 요약
1. 병렬성(Parallelism)은 단일 작업을 더 빠르게 완료하기 위해 여러 CPU 코어를 활용하는 속도 중심의 문제이며, 스레드는 코어 수에 맞춰 공간적 스케줄링을 담당한다.

2. 동시성(Concurrency)은 외부에서 들어오는 독립된 여러 작업을 제한된 리소스에 효율적으로 처리하는 처리량 중심의 문제이며, 스레드가 많아 시간적 스케줄링이 중요하다.

3. 비동기 프로그래밍은 블로킹을 피하기 위한 논블로킹 기법으로, 콜백, Future/Promise, Rx 등의 한계를 극복하고 동기 코드처럼 작성할 수 있도록 하는 Kotlin 코루틴이 등장했다.

---

**학습 날짜**: 2025-12-10  
**작성자**: 류태웅