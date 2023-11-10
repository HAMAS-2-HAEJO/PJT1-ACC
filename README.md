# 모빌리티 임베디드 SW스쿨 2차 프로젝트 - 1

Matlab Simulink를 이용하여 고속도로 자율주행을 위한 고도화된 ACC(Adaptive Cruise Control) 기능 개발

## 프로젝트 배경

- 프로젝트는 차량 도메인에서 SW개발의 Human Error을 줄이고, 코드 탑재 이전 
가상환경에서의 시뮬레이션이 용이한 모델 기반 개발 과정을 익히는데 중점
- 서로 요구사항을 전달하고 협상하는 과정을 거치며 V 모델 프로세스에 대해서 익힘.

## 프로젝트 필요성

- 기존 ACC 기능은 전방 차량의 속도와 관계없이 차량의 거리에 따라 고정된 속도로 동작된다는 한계를 가짐. ACC의 고도화를 통해 원하는 속도로 주행하며, 전방 차량 거리에 따른 유동적 감속 시스템의 구현 필요.
- 한국도로공사에 따르면, 최근 5년간 발생한 여름 장마철(6~8월) 빗길 교통사고 치사율은 맑은날 대비 약 5배 높은 수치를 보임.
- 또한, 도로의 종류에 따른 치사율은 고속도로가 일반도로보다 4배 이상의 수치를 보임.
- 우천 시 평소보다 시야 확보에 어려운 상황에서 차간 거리와 감속 정도를 보다 증가시켜 안전을 확보하는 기술의 필요.

## 주요기능
- 가변저항을 이용한 차량의 속도 조절 시스템의 구축.
- 빗물 감지 센서를 이용한 우천 감지시 차량 안전거리 증가 및 감속 정도 변경 시스템의 개발.
- 우천 정도에 따른 가변 속도 와이퍼 시스템의 개발.
- 후진 및 Brake 시스템의 구축.
  
---
## 프로젝트 결과
> 모델 설계 + 요구사항
>
<img src="https://github.com/HAMAS-2-HAEJO/PJT1-ACC/assets/87352996/e5370fbe-2f2d-4fa9-ae86-f53b109f5104.png" width="400" height="200"/>
<img src="https://github.com/HAMAS-2-HAEJO/PJT1-ACC/assets/87352996/7a9f0488-ab25-445e-9b26-4dfc349043c1.png" width="400" height="200"/>
<img src="https://github.com/HAMAS-2-HAEJO/PJT1-ACC/assets/87352996/3d62ddbc-1672-4384-9895-e8bc6c2d8aec.png" width="400" height="200"/>
<img src="https://github.com/HAMAS-2-HAEJO/PJT1-ACC/assets/87352996/d864bffc-dd02-4cb3-8090-741fa58c43ce.png" width="400" height="200"/>



## 프로젝트 산출물 요약

| 폴더 | 상세내용 |
| --- | --- |
| Requirements | 전달받은 요구사항에 대한 명세과정 |
| Test | 단위테스트 - 통합테스트 - 시스템 및 인수테스트 수행과정 |
| Unit | 단위 모듈 설계 및 구현 파일 |
| integrated | 기능별 통합 및 최종 통합 파일 정리 |

---
## 환경구축


1. Matlab 설치 ( R2022b 이상 ) 
    - Simulink 관련 패키지 추가 설치
2. Add on → 검색 창에 “Simulink Support Package for Arduino Hardware” 검색 후 설치
    - 모델기반 아두이노 제어관련 모듈 다운로드 과정
3. Add on → 검색 창에 “DSP System Toolbox:” 설치
    - 모델 설계 중, delay 관련 함수 사용을 위한 패키지

## Simulink 모델 환경 설정


1. Simulink 모델 파일 실행 ( .slx )
2. 상단 Tool바에서 모델링 → 모델설정
    
    <img src="https://github.com/HAMAS-2-HAEJO/PJT1-ACC/assets/87352996/84b8ae50-b6df-4146-a2e8-344e0a989a14.png" width="600" height="150"/>

3. 구성 파라미터 - 솔버 설정
    
    <img src="https://github.com/HAMAS-2-HAEJO/PJT1-ACC/assets/87352996/90ca1f13-beac-4605-9ce3-1479dcb639ee.png" width="600" height="400"/>

4. 구성 파라미터 - 하드웨어 구현 설정
    
    <img src="https://github.com/HAMAS-2-HAEJO/PJT1-ACC/assets/87352996/fe31c183-4081-452d-87f4-4a7fbcfd3b1b.png" width="600" height="400"/>

---

## 프로젝트 개발환경


| S/W 개발환경 | 상세내용 |
| --- | --- |
| IDE | Matlab 및 Simulink |
| 개발도구 | Simulink |
| 개발언어 | C, Matlab |
| 기타사항 | Support Package for Arduino Hardware 사용 |

| H/W 구성장비 | 상세내용 |
| --- | --- |
| 개발 보드 | - Arduino Mega 2560 R3 |
| 추가 모듈 | - Easy Module Shield V1, Arduino Motor Shield Rev3 |
| 사용 센서 | 초음파(HR-SR04), DC모터, 빗물감지센서, 가변저항, LED, 부저, 스위치 |
| 기타사항 |  |

| 프로젝트 | 관리환경 |
| --- | --- |
| 형상관리 | Git |
| 의사소통관리 | Notion, 카카오톡 |
| 기타사항 |  |
