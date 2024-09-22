# 대구르르 - DAEfree
## 서비스 요약
**무더위 쉼터 정보 제공 서비스(DAEfree)** - 대구 무더위 쉼터 정보 제공 및 현재 위치 기반 인근 쉼터 안내, 쉼터 이용자 커뮤니티 제공   
![KakaoTalk_20240922_000753663](https://github.com/user-attachments/assets/10779e3f-6020-4fe5-8121-12e2b66a5e7f)

## 레포지토리 링크
**FE 레포지토리** : https://github.com/Daegurrr/Daegurrr_Frontend

**BE 레포지토리** : https://github.com/Daegurrr/Daegurrr_backend

## 주제 구분
-	S타입 대구 시내의 환경 문제를 해결하고 지속가능한 발전을 지원하는 서비스 

## 팀원 소개
**대구르르**
| 권수현 | 김규회 | 김현민 | 채정민 |
| :-----: | :-----: | :-----: | :-----: |
| [<img src="https://github.com/kwonssshyeon.png" width="100px">](https://github.com/kwonssshyeon) | [<img src="https://github.com/KimKyuHoi.png" width="100px">](https://github.com/KimKyuHoi) | [<img src="https://github.com/ZZAEMMIN.png" width="100px">](https://github.com/ZZAEMMIN) | [<img src="https://github.com/chaejm55.png" width="100px">](https://github.com/chaejm55) | 
| 백엔드 | 프론트엔드 | 디자인 | 백엔드 | 

## 시연 영상
[![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white)](https://youtu.be/dOZQivC8648)


## 서비스 소개
### 서비스 개요
무더위에 지친 대구 시민을 위해 무더위 쉼터의 정보를 실시간으로 알려주는 서비스이다.
사용자는 간단한 과정으로 무더위를 피할 수 있다.
또한, 커뮤니티를 통해 쉼터에서 서로 도움을 주고 받으며 대구 시민 사이에 유대감과 커뮤니티를 형성할 수 있다.



### 타서비스와의 차별점
서비스 타겟층인 무더위 취약계층 중 많은 비율로 디지털 기기의 사용이 익숙하지 못하다. 하지만 기존 비슷한 서비스는 사용하기 너무 복잡해 이 사람들이 이용할 수 있을 것이라 기대하기 어려웠다. 
따라서 우리 서비스는 무더위 쉼터 정보 제공의 접근성 개선 및 커뮤니티 형성 집중했다.

기타 지도 앱에서는 무더위 쉼터 정보를 제공하지 않는다. 또한 비슷한 서비스로 “안전디딤돌” 이라는 서비스가 있지만, 직접 사용해본 결과 4번의 클릭이 필요할 정도로 접근성이 좋지 않음을 느꼈다.  그래서 우리 서비스는 단 한번의 클릭으로 무더위에 지친 사용자에 가장 필요한 정보를 제공해줄 수 있고, 쉼터에서 무더위를 함께 이겨낼 커뮤니티 형성 기능에서도 기존 서비스와 차별점이 있다.

### 구현 내용 및 결과물
**API명세**

[<img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=Swagger&logoColor=black">](http://43.203.25.171:8080/api-docs)

<br/>

**구현 화면**

1. 무더위 쉼터 지도 페이지
    - 지도를 통해 현재 위치 부근의 무더위 쉼터 정보를 자세하게 제공한다.
    - 무더위 쉼터 종류를 통해 검색하는 것도 가능하다.
      <img src="https://github.com/user-attachments/assets/b6145ee2-8b3d-4e8f-9a8c-a2f5083e91bf" height="500"/>
2. 무더위 쉼터 커뮤니티 페이지
    - 무더위 쉼터에 관한 정보를 주고 받을 수 있다.
    - 무더위 쉼터 이용자 사이에 도움을 주고 받을 수 있다.
      <img src="https://github.com/user-attachments/assets/ebd29c24-c88b-4777-8d7b-808df3c86dbe" height="500"/>

### 구현 방식
어떤 언어와 프레임워크를 사용했는지, 만약 배포를 진행했다면 환경은 어떤지 등을 기재
1. 프론트엔드
    - React
    - axios, styled-components, zustand, framer-motion
    - 카카오 지도 API 사용
2. 백엔드
    - Java, Spring
    - AWS EC2에 Docker를 사용해 배포, DB로 RDS 사용
    - 공공 데이터 API, Spring Scheduler로 매일 데이터 수집, 카카오 oauth 사용
3. 디자인
    - Figma
    - Adobe Illustrator

## 향후 개선 혹은 발전 방안
**'DAEfree'가 웹 친화적인 UI라는 점에서 사용자 접근성과 사용편의성, 지속성을 고려하여 향후 개선 및 발전 방안을 도출했다.**

**첫째, 모바일 서비스와 반응형 UI 개발**

향후 사용자 위치 기반으로 모바일 서비스를 개발하여 경로를 따라 가까운 무더위 쉼터로 이동할 수 있도록 할 예정이다. 이는 사용성을 확대하여 소프트웨어의 활용성을 높일 수 있을 것이다.

접근성과 사용성 향상을 위해 모바일 서비스 개발뿐만 아니라 반응형 UI로 디자인하여 다양한 디바이스에서 사용자가 손쉽게 소프트웨어를 사용할 수 있도록 의도한다.

**둘째, 쉼터의 특이사항·공지사항을 업데이트하는 관리 시스템 구축**

쉼터 운영자·관리자가 쉼터의 특이사항·공지사항 등을 실시간으로 업데이트 할 수 있는 관리 시스템을 구축할 예정이다. 적극적인 서비스 관리를 통해 사용자 편의성을 높이고 명절·공휴일 운영여부 등 쉼터에 대한 구체적인 정보를 알 수 있도록 할 것이다.

**셋째, 대구시와 협력하여 지속적인 사용을 유도**

대구시 지자체와 협력하여 쉼터에서 냉방 서비스, 음료 제공, 건강 체크 등의 부가 서비스를 제공하고 봉사자나 서비스 제공자에게 대구시 훈장 또는 표창장 등의 인센티브를  제공하여 성취감을 고취시켜 소프트웨어의 지속적인 사용을 유도한다. 이는 폭염 대응을 위한 대구시만의 체계적인 시스템을 구축할 수 있으며 지속 가능한 발전에 기여할 가능성이 있다.
