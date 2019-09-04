# Woongjin_my_work_issue
This repository is my issue that occurred when I worked a Woongjin Thinkbig.



2019.08.12



> ISSUE #1

```kotlin
WARNING: The option 'android.enableAapt2' is deprecated and should not be used anymore.
Use 'android.enableAapt2=true' to remove this warning.
It will be removed at the end of 2018..
```

**<#gradle.properties >**

```kotlin
android.enableAapt2=true
```



> ISSUE #2

```kotlin
AAPT2 error: check logs for details
```



그러니까 aapt는 안드로이드 어셋 — 이미지나 문자열 등의 앱 내 리소스를 최적화 된 형태로 변환 하는 역할을 합니다.

따라서 aapt 에러가 났다는 것은 이러한 리소스 처리 부분에서 에러가 발생했다는 것을 의미 합니다.

추가적으로 androidManifest 의 병합 — 여러 모듈 간 병합이나 라이브러리 의존성에 대한 부분에서 에러가 발생 하는 경우에도 aapt 에서 에러가 발생합니다.



[원문 보기](https://toepic.fail/aapt2-error-check-logs-for-details-23d13d6d5f76)









