# Android Process and App Lifecycle

## 학습 자료 링크
https://velog.io/@victoryu/Android-Process-App-Lifecycle

## 학습 세 줄 요약
1. 안드로이드는 앱 프로세스를 직접 제어하지 않고, 컴포넌트 상태(Activity·Service·BroadcastReceiver)와 시스템 메모리 상황을 종합해 프로세스를 생성·유지·종료한다.

2. 실행 중인 구성 요소에 따라 프로세스는 포그라운드 → 가시적 → 서비스 → 캐시된 프로세스 순의 중요도 계층으로 분류되며, 중요도가 낮을수록 메모리 부족 시 먼저 종료 대상이 된다.

3. BroadcastReceiver에서 단순히 스레드만 띄우고 반환하는 것처럼 컴포넌트를 잘못 사용하면, 시스템이 프로세스를 “불필요”하다고 판단해 작업 중에도 종료할 수 있으므로 JobService, 포그라운드 서비스 등 적절한 API로 장기·중요 작업을 위임해야 한다.

---

**학습 날짜**: 2026-01-08
**작성자**: 류태웅