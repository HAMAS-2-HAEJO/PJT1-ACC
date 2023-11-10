# 모빌리티 임베디드 SW스쿨 2차 프로젝트 - 1

Matlab Simulink를 통한 Adaptive Cruise Control기능 구현 프로젝트

## 프로젝트 배경 및 필요성


## 프로젝트 소개


## 주요기능

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
