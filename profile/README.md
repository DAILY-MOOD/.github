# 캘린더 일기장 (Calendar Diary)

## 소개
캘린더 일기장은 Flutter로 개발된 모바일 앱으로, 날짜별로 일기를 작성하고 관리할 수 있는 애플리케이션입니다. Material Design 3를 적용한 모던한 UI와 직관적인 사용자 경험을 제공합니다.

## 주요 기능
- 📅 캘린더 기반 일기 관리
  - 월별 캘린더 보기
  - 일기 작성된 날짜 마커 표시
  - 연/월 빠른 선택
- ✍️ 일기 작성 및 관리
  - 일기 작성/수정/삭제
  - 실시간 저장
- 📚 일기 목록
  - 전체 일기 목록 보기
  - 최신순 정렬
  - 날짜별 필터링
- 🔒 사용자 관리
  - 회원가입/로그인
  - 토큰 기반 인증

## 기술 스택
### Frontend
- Flutter 3.0+
- Dart 2.17+
- Material Design 3
- table_calendar
- intl (다국어 지원)

### Backend
- Django REST Framework
- SQLite3
- Token Authentication

## 화면 구성

### 1. 메인 캘린더 화면
- 월별 캘린더 표시
- 일기 작성된 날짜 마커 표시
- 연/월 선택 기능

### 2. 일기 작성/수정 화면
- 일기 작성 및 수정
- 일기 삭제 기능
- 날짜별 일기 관리

### 3. 일기 목록 화면
- 작성된 일기 목록 표시
- 최신순 정렬
- 일기 내용 미리보기

## UI/UX 특징
- Material Design 3 적용
- 커스텀 테마 설정
- 반응형 디자인
- 한국어 지원

## 설치 방법

### 1. Flutter 개발 환경 설정
- Flutter SDK 설치
- Android Studio 또는 VS Code 설치
- 필요한 플러그인 설치

### 2. 프로젝트 클론
git clone [repository-url]
cd calendar-diary

### 3. 의존성 설치
flutter pub get

### 4. 서버 설정
1. Python 및 Django 설치<br>
pip install django djangorestframework django-cors-headers

2. 데이터베이스 마이그레이션<br>
python manage.py migrate

3. 서버 실행<br>
python manage.py runserver

4. 앱 실행<br>
flutter run

> **참고**: 앱을 실행하기 전에 반드시 Django 서버가 실행 중이어야 합니다.

## 시스템 요구사항
- Flutter 3.0 이상
- Dart 2.17 이상
- Python 3.8 이상
- Django 4.0 이상
- Android 5.0 이상 또는 iOS 11.0 이상
