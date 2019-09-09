# Common issue

[TOC]



`2019.09.09`

> ISSUE #1 

## OEM USB 드라이버 설치(w-pad usb-driver)



Windows 7 이상 버전에서 처음 Android USB 드라이버를 설치하려면:

1. Android 구동 기기를 컴퓨터의 USB 포트에 연결합니다.
2. 바탕화면 또는 Windows 탐색기에서 **Computer**를 마우스 오른쪽 버튼으로 클릭한 다음 **Manage**를 선택합니다.
3. 왼쪽 창에서 **Devices**를 선택합니다.
4. 오른쪽 창에서 **Other device**를 찾아 펼칩니다.
5. 기기 이름(예: **Nexus S**)을 마우스 오른쪽 버튼으로 클릭한 다음 **Update Driver Software**를 선택합니다. 이렇게 하면 하드웨어 업데이트 마법사가 시작됩니다.
6. **Browse my computer for driver software**를 선택하고 **Next**를 클릭합니다.
7. **Browse**를 클릭한 다음 UDB 드라이버 폴더를 찾습니다. (Google USB 드라이버는 `<sdk>\extras\google\usb_driver\`에 있습니다.)
8. **Next**를 클릭하여 드라이버를 설치합니다.



- https://developer.android.com/studio/run/oem-usb?hl=ko (참조)

![](D:\___down\1567989902.png)





`2019.08.12`

## android.enableAapt2



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

















