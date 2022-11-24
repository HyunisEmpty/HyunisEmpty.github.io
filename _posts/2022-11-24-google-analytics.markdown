---
layout: post
title:  "Google Analytics"
date:   2022-11-24 13:33:00 +0900
categories: jekyll update
---

## Google Analytics란?
구글 애널리틱스(Google Analytics, GA)는 구글에서 무료로 제공하고 있는 웹분석 서비스입니다.

### GA 회원 가입및 추적 코드 생성
1. [Google Analytics](https://analytics.google.com/analytics/web/)에 접속하여 회원가입을 한다.
2. 데이터 스트림 웹 항목에 본인 블로그 주소를 입력하여 스트림을 추가한다.
3. 위와 같은 과정을 진행하면 **측정 ID**를 확인 가능하다.
  - Google Analytics의 경우 G-XXXXXXXX의 형식을 사용한다.

### 측정 ID
```
# Analytics
analytics:
  provider               : "google-gtag"
                          # false (default), "google", "google-universal", "google-gtag", "custom"
  google:
    tracking_id          : "추적 ID"
    anonymize_ip         : # true, false (default)
```
다음과 같은 _config.yml 파일에 작성합니다.

### 추적 코드
- 스크립트는 생성한 계정 좌측 상단바 가장 하단에 위치한 톱니바퀴모양 설정 > 속성탭 데이터 스트림 > 계정생성할때 생성했던 스크림 을 선택한다. (스트림이 없다면 우측 상단의 스트림 추가 버튼을 눌러 추가하자.)

- 새로운 온페이지 태그 추가 탭의 첫번째 항목 클릭하여 소스코드를 복사한다.

- 태그를 복사한 후 웹사이트의 각 페이지 코드에서 <head> 요소 바로 다음에 붙여넣으세요. Google 태그는 각 페이지에 하나씩만 추가합니다.
