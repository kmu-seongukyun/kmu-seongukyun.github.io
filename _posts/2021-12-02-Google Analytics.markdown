---
layout: post
title:  "Google Analytics"
date:   2021-12-02
description: Google Analytics란? / Google Analytics의 장단점 / Google Analytics 활용방안 / Githubpage와 Google Analytics 연동 과정
comments: true
---

## Google Analytics란?
현재 구글 마케팅 플랫폼 브랜드 내의 플랫폼으로서, 웹사이트 트래픽을 추적하고 보고하는 구글이 제공하는 웹 애널리틱스 서비스
<br>
<br>

## Google Analytics의 장점
### 1. 무료 서비스
속성당 월간 1,000만 조회수라는 무료 서비스 용량 한도가 있기는 하지만 대다수 사업자들은 도달하기 힘들 만큼 충분히 많은 용량에 해당합니다.
 <br>

### 2. 막강한 기능
무료 서비스임에도 불구하고 제공하는 기능은 에이스카운터, 로거 등 국내 유료 웹로그분석 서비스 못지 않습니다. 못지 않은 게 아니라 사실 더 뛰어나다고 볼 수 있습니다. GA 기능에 대해서는 앞으로 차근차근 다룰 예정입니다만 다양한 목표설정 기능과 향상된 전자상거래 기능, 이벤트 설정과 세그먼트 등의 기능은 국내 유료 솔루션도 제공하지 못하는 깊이 있는 분석을 가능하게 합니다. 특히 측정기준과 측정항목을 조합하여 원하는 데이터를 추출할 수 있도록 하는 맞춤 보고서 기능은 매우 강력한 맞춤 분석 기능을 제공합니다.
<br>

### 3. 사용자 인테페이스 우수
물론 국내 유료 서비스나 네이버 애널리틱스에 비해 사용자 편의가 부족하다는 주장도 있긴 합니다. 하지만 매우 다양한 기능이 제공된다는 점을 감안하면 구글 애널리틱스 보고서는 매우 직관적이고, 사용하기 쉬우며, 분석에도 용이합니다.
<br>
<br>

## Google Analytics의 단점
구글 애널리틱스는 사용하기 어렵다는 얘기도 많습니다. 번역의 한계로 인해 GA에서 사용되는 용어와 개념을 이해하기가 쉽지 않다는 점, 무료로 제공되는 서비스인 만큼 궁금한 사항을 스스로 해결해야 한다는 점 등이 그 이유로 자주 언급됩니다. 하지만 구글 애널리틱스가 어렵다기보다는 웹분석 자체가 쉽지만은 않기 때문이라는 생각이 더 큽니다. 웹분석을 제대로 하기 위해서는 ‘제대로 된 데이터 수집’을 전제로 ‘제대로 된 분석’이 이뤄져야 합니다. 정확한 데이터 수집을 위해서는 웹개발자의 지식이, 의미 있는 분석을 위해서는 마케터의 통찰력이 필요합니다. 이 두가지를 동시에 갖추기는 쉽지 않습니다. 웹분석이 그리고 구글 애널리틱스가 어려울 수밖에 없는 이유입니다.
<br>
<br>

## Google Analytics 활용 방안
전문가 수준의 세팅이 아닌 기본 스크립트 설치만으로도 우리의 잠재고객에 관한 방대한 데이터를 수집할 수 있으며, 이러한 정보를 통해 의외의 인사이트를 얻을 수도 있습니다. 또한 제대로 세팅을 해 놓으면 언제라도 유용하게 사용할 수 있는 데이터가 차곡차곡 쌓이게 됩니다.

## Githubpage와 Google Analytics 연동 과정
### 1. Google Analytics 계정 생성
<img src="/assets/img/GA1.PNG"><img>
<br>

### 2. Google Analytics 속성 설정
<img src="/assets/img/GA2.PNG"><img>
속성 이름, 보고 시간대, 통화 입력
<br>
측정 ID G- 가 아닌 추적 ID UA-를 사용하기 위해 고급 옵션 보기 클릭
<img src="/assets/img/GA3.PNG"><img>
<br>

### 3. Google Analytics 비지니스 설정
<img src="/assets/img/GA4.PNG"><img>
업종 카테고리, 비지니스 규모, 사용 계획 선택 후 만들기 클릭
<br>

### 4. 추적 ID 확인
<img src="/assets/img/GA5.PNG"><img>
추적 ID (UA- 부분) 복사
<br>

### 5. _config.yml에 추적 ID 값 입력
<img src="/assets/img/GA6.PNG"><img>
google_analytics 부분에 복사해온 추적 ID값 붙여넣기
<br>

### 6. Githubpage와 Google Analytics 연동 확인
<img src="/assets/img/GA7.PNG"><img>
Githubpage에 접속했을 때 현재 활성 사용자가 1이 되는 것을 확인!
<br>