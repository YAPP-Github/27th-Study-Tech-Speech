# Android Notification

## 학습 자료 링크
https://velog.io/@victoryu/Android-Notification

## 학습 요약
1. Notification 기본 표시 및 관리
  - 표시 방식: 알림은 상태바(Status Bar), 알림창(Notification Drawer), 팝업(Heads-up), 잠금 화면, 앱 아이콘 배지 등 다양한 형태로 사용자에게 노출된다.
  - 삼성 기기에서는 '알림 카테고리 관리' 메뉴를 직접 활성화해야만 개별 알림 채널에 대한 상세 설정(활성화/비활성화)이 가능하다.

2. Samsung One UI 8 및 Android 16 특이 사항 
  - 기존 가이드와 달리 One UI 8 버전부터는 잠금 화면에서도 팝업(Heads-up) 형태의 알림 표시를 지원한다.
  - setSilent 메서드 무시: One UI 8에서는 알림 채널의 중요도가 '긴급(Urgent)'인 경우, 개발자가 코드로 설정한 setSilent 무음 처리가 무시되고 팝업 알림이 강제로 나타난다.
  - 삼성 One UI의 알림 배지는 AOSP와 달리 알림의 상세 내용 확인보다는 단순 숫자 표기 기능에 집중되어 있다.

3. Android 16 자동 그룹화(Auto-grouped)
  - Android 16부터는 앱이 별도의 요약(Summary) 알림을 생성하지 않더라도 시스템이 스스로 알림을 그룹화한다.
  - 자식 알림이 없거나 그 수가 매우 적은 경우, 화면의 효율적 활용을 위해 자동으로 그룹화가 적용된다.

---

**학습 날짜**: 2025-12-26 
**작성자**: 류태웅