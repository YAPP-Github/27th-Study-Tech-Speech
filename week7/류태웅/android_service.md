# Android Service

## 학습 링크
https://velog.io/@victoryu/Android-Service

## 요약
Service의 세 종류

1. Background Service (= Started Service)
startService()를 호출하여 시작되며 onStartCommand() 메서드가 호출된다.
호출한 구성 요소와 독립적인 수명 주기를 가지며, 작업 완료 후 stopSelf() 또는 stopService()로 중단해야 한다.
Intent를 통해 데이터를 전달받아 순차적으로 처리하는 방식으로 사용된다.

2. Foreground Service
사용자에게 알리는 notification을 표시하면서 실행되는 서비스이다.
백그라운드 실행 제한이 엄격한 최신 Android 버전에서 사용된다.
음악 재생, GPS 추적 등 사용자가 인식해야 하는 작업에 사용된다.

3. Bound Service
bindService()를 호출하여 바인딩되며, 클라이언트-서버 인터페이스를 제공한다.
클라이언트가 바인딩을 해제할 때까지 실행되며, 양방향 통신이 가능하다.
서비스와의 상호작용이 필요한 경우에 사용된다.

---

**학습 날짜**: 2026-01-18
**작성자**: 류태웅