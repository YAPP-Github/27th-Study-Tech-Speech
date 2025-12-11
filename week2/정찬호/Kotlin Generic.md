### Kotlin Generic
#### [링크](https://medium.com/@chanho680526/kotlin-generic-type-system-699b82c1ebf4)

Kotlin으로 작성된 코드는 Kotlin Compiler에 의해 컴파일되어 Java Byte Code로 변환됩니다. 이 과정에서 제네릭의 타입 정보는 소거(Type Erasure)되어 런타임 시점에 사라지게 됩니다. 
따라서 제네릭은 컴파일 타임의 타입 안전성(Type Safety)을 보장하기 위해 사용됩니다.

이 글에선 크게 다음 내용에 대해 소개합니다.

제네릭의 타입 정보 소거
제네릭엔 왜 참조 타입만 가능한가 ?
