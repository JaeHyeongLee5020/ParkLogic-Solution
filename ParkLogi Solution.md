# 🅿️ ParkLogi Solution

**ParkLogi Solution**은 스마트 주차 예약, AI 기반 범죄 감지, Firebase 연동 기능을 포함한 모바일·웹 통합 스마트 주차 관리 시스템입니다.

---

## 📱 주요 기능 (Android 앱)

- **실시간 주차 예약**
  - 주차장 선택 (PL장안대, PL협성대, PL수원대)
  - 공간 선택 및 예약 처리
  - 당일 예약 수에 따라 잔여 공간 실시간 계산
- **Firebase 연동**
  - 사용자 인증 (Authentication)
  - 예약 및 감지 데이터 실시간 저장 (Realtime Database)
- **Android APP UI 구성**
  - 내 정보 / 주차 예약 / 내 예약 정보 / 커뮤니티 / 시간 구매 / 로그아웃
- **실시간 알림 기능**
  - 사고 감지 시 Android 상태바에 알림 전송
- **첫 실행 애니메이션 및 사용자 안내 메시지**

---

## 🧠 AI 기반 범죄 감지 기능

- **감지 범주**
  - `nomal`, `smoking`, `assault`, `propertyDamage`, `wasteDumping`, `threat`, `thief`
- **학습 데이터**
  - mp4 영상 → 프레임 추출 → 커스텀 CNN 학습
- **결과 처리**
  - `nomal` 제외한 범주만 Firebase 저장
  - 동일 상황 10회 연속 감지 시만 저장
  - Firebase 경로:  
    `situation/{사용자명}/{yyyy-mm-dd}/{hh:mm:ss} → 상황명`

---

## 🌐 웹/관리자 페이지 기능 


- **JSP + Bootstrap UI 구성**

---

## 📁 외부 리소스

- **Google Drive 프로젝트 전체**  
  [🔗 프로젝트 다운로드](https://drive.google.com/file/d/1CeVgqceX2L2qFteHeXAozK5evTUvmVsp/view)

---

## 🛠️ 사용 기술 스택

| 구성 요소         | 기술                                       |
|------------------|--------------------------------------------|
| **프론트엔드**   | Android (Java, XML), Bootstrap (웹)        |
| **백엔드**       | Spring Boot, JSP, Thymeleaf                |
| **DB 및 연동**   | Firebase Authentication, Realtime Database |
| **AI 모델링**    | Python, TensorFlow, OpenCV                 |
| **기타 도구**    | Gradle, GitHub, Google Drive               |

---

## 📌 프로젝트 목적

> 안전하고 편리한 주차 경험을 제공하며, 실시간 범죄 감지를 통해 사용자와 관리자 모두에게 필요한 정보를 즉시 전달하는 통합형 스마트 주차 솔루션 개발

---

