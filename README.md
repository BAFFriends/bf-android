# 🌟 AI 기반 장애인 취업 지원 플랫폼 - BAFF

> 장애인의 성공적인 취업을 위한 맞춤형 채용 정보 제공 플랫폼

## 📱 프로젝트 소개

이 프로젝트는 8th umc hackathon 에서 시작한 프로젝트로, 장애인의 취업 기회를 확대하고 맞춤형 채용 정보를 제공하는 Android 애플리케이션입니다. <br>
사용자의 장애 유형, 희망 직종, 근무 조건 등을 고려하여 개인화된 채용 공고를 추천하고, <br>
간편한 지원 프로세스를 통해 장애인의 취업 성공률을 높이는 것을 목표로 합니다.

## 🗓️ 기간

2025.07.05 ~ 2025.07.06 (무박 2일)

## 🏅 수상
UMC 8th Hackathon 대상

## ✨ 주요 기능

### 🏠 홈 화면
- **개인화된 채용 공고 추천**: 사용자 프로필 기반 맞춤형 채용 정보 제공
- **스와이프 인터페이스**: 카드 형태의 직관적인 채용 공고 탐색
- **즉시 지원**: 관심 있는 채용 공고에 바로 지원 가능

### 📋 채용 공고 목록
- **다양한 필터링 옵션**:
  - 장애 유형별 필터 (지체, 뇌병변, 시각, 청각, 언어, 안면, 신장, 심장, 간, 호흡기, 장루·요루, 뇌전증, 정신, 발달장애 등)
  - 지역별 필터 (전국 시·도 단위)
  - 고용 형태 (정규직, 계약직, 인턴, 프리랜서, 아르바이트 등)
  - 급여 범위 및 근무 시간
  - 학력 및 경력 조건
- **프로필 기반 추천**: 개인 정보를 바탕으로 한 스마트 추천 시스템

### 👤 마이페이지
- **이력서 관리**: 개인 정보, 장애 유형, 희망 조건 등 상세 프로필 작성
- **지원 내역 관리**: 지원한 채용 공고 현황 확인
- **설정 관리**: 앱 환경 설정 및 개인 정보 수정

### 🔍 검색 기능
- **통합 검색**: 채용 공고 제목, 회사명, 직무 등 다양한 조건으로 검색
- **검색 기록 관리**: 최근 검색어 저장 및 관리

### 📝 채용 지원
- **간편 지원**: 미리 작성된 이력서 정보를 활용한 원클릭 지원
- **지원 사유 및 메시지**: 개인화된 지원 메시지 작성
- **지원 결과 관리**: 지원 현황 및 결과 확인

## 🛠 기술 스택

### Android
- **Kotlin**: 주 개발 언어
- **Jetpack Compose**: 현대적인 UI 개발 프레임워크
- **Material Design 3**: 구글의 최신 디자인 시스템

### Architecture & Libraries
- **MVVM Pattern**: 관심사 분리를 통한 유지보수성 향상
- **Hilt**: 의존성 주입 프레임워크
- **Retrofit**: REST API 통신
- **Navigation Component**: 화면 간 네비게이션 관리
- **StateFlow & LiveData**: 반응형 데이터 처리

### UI/UX
- **Custom Design System**: 접근성을 고려한 맞춤형 디자인 컴포넌트
- **Pretendard Font**: 가독성 높은 한국어 폰트
- **Responsive Design**: 다양한 화면 크기 대응

## 🏗 프로젝트 구조

```
app/src/main/java/umc/hackathon/
├── core/                      # 핵심 공통 모듈
│   ├── component/            # 재사용 가능한 UI 컴포넌트
│   ├── designsystem/         # 디자인 시스템 (색상, 폰트, 테마)
│   ├── navigation/           # 네비게이션 관련
│   └── ui/                   # 공통 UI 유틸리티
├── data/                     # 데이터 레이어
│   ├── datasource/          # 데이터 소스 (로컬/원격)
│   ├── network/             # 네트워크 API
│   └── repository/          # 데이터 저장소
├── domain/                  # 비즈니스 로직
├── model/                   # 데이터 모델
├── presentation/            # 프레젠테이션 레이어
│   └── ui/                  # 화면별 UI 구성
│       ├── main/            # 메인 화면들
│       ├── home/            # 홈 화면
│       ├── jobpost/         # 채용 공고 관련
│       ├── mypage/          # 마이페이지
│       ├── search/          # 검색 기능
│       └── apply/           # 지원 관련
└── di/                      # 의존성 주입 모듈
```

## 📸 스크린샷

### 주요 화면

<div align="center">
  <img src="https://github.com/user-attachments/assets/f6731a00-d0ad-4753-babc-f56a4e8eb637" width="200" alt="홈 화면"/>
  <img src="https://github.com/user-attachments/assets/f9832512-8c92-4e55-bd20-ff9f183c5ee0" width="200" alt="채용 공고 목록"/>
  <img src="https://github.com/user-attachments/assets/0a028454-f9d2-4d2c-a974-13b5036de7bf" width="200" alt="마이 페이지"/>
</div>

<div align="center">
  <strong>홈 화면</strong> | <strong>채용 공고 목록</strong> | <strong>마이 페이지</strong>
</div>

세부 뎁스 페이지는 데모 영상에서 확인하실 수 있어요.

### [데모](https://youtu.be/l3YTwNZOLt8?si=RkAHxWBAi7Sj6AnN)
![데모 비디오](https://img.youtube.com/vi/l3YTwNZOLt8/0.jpg)


## 👥 개발자

| 역할 | 이름 | GitHub |
|------|------|--------|
| Android Developer | 김강현 | [@keem-hyun](https://github.com/keem-hyun) |
| Android Developer | 김경록 | [@gomsang](https://github.com/gomsang) |
| Android Developer | 손주완 | [@vvan2](https://github.com/vvan2) |
