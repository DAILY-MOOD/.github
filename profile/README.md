# 📘 DAILY MOOD
  
**DAILY MOOD**는 단순한 일기 관리 앱을 넘어, 사용자의 감정을 기록하고 분석하여 **사회적 약자(청소년, 노약자, 장애인 등)의 정서적 돌봄**을 지원하는 서비스입니다.  
<br/>

<img width="1908" height="1068" alt="image" src="https://github.com/user-attachments/assets/8bd86d93-1499-4a97-b510-08e0753cc3e3" />
<br/>
<br/>

- 🔍 **감정 기록 & 추적** : 작성된 일기를 바탕으로 감정 분석을 수행해 사용자의 정서 상태를 파악합니다.  
- ❤️‍🩹 **심리적 지원 가능성** : 일정 기간 부정적 감정 패턴이 지속적으로 감지되면, 상담 지원이나 커뮤니티 연계와 같은 확장 서비스를 고려할 수 있습니다.  
- 🤝 **산학 협력 프로젝트** : 전북대학교 hello world 팀이 LG U+와 함께 진행한 산학 협력 캡스톤 프로젝트의 결과물로, 인공지능 기술을 활용해 사회적 약자의 생활 개선을 돕는 것을 목표로 합니다.  
<br/>  
<br/>
  
## ✅ 주요 기능
### 프론트엔드 (Flutter)
- **회원 인증**
  - 로그인 / 로그아웃
  - 신규 가입 지원
- **일기 관리**
  - 일기 작성, 수정, 삭제
  - 작성된 일기 목록 조회
- **데이터 분석**
  - 텍스트 기반 감정 분석(분석 서비스 연동)
- **멀티플랫폼 지원**
  - Android, iOS, Web, Desktop(macOS, Windows, Linux)
<br/>

### 백엔드 (Django + DRF)
- **사용자 관리**
  - 회원가입 (Register API)
  - 로그인 (JWT 토큰 기반 인증)
- **일기 데이터 관리**
  - 일기 작성(Create), 조회(Read), 수정(Update), 삭제(Delete)  
- **REST API 제공**
  - Flutter 앱과 통신 가능한 JSON API 엔드포인트 제공
<br/>  
<br/>  
  
## ✅ 기술 스택
### 프론트엔드
- Flutter (Dart)
- SQLite
- REST API 연동
<br/>

### 백엔드
- Django
- Django REST Framework
- SQLite
<br/>

<img width="1900" height="1065" alt="image" src="https://github.com/user-attachments/assets/28df6f5d-94b2-4afe-9741-64b3a14eaa30" />
<br/>  
<br/> 
  
## ✅ 프로젝트 구조
```
/diary-main (Frontend - Flutter)
  ├── lib/
  │   ├── main.dart                 # 앱 진입점
  │   ├── screens/                  # 로그인, 메인, 일기 화면
  │   └── services/                 # Auth, Diary, Analysis API 연동

/backend-main (Backend - Django)
  ├── models.py       # Diary 모델 정의
  ├── views.py        # 회원가입/로그인, Diary CRUD API
  ├── serializer.py   # User, Diary 직렬화
  ├── urls.py         # 엔드포인트 라우팅
  └── setting.py      # Django 프로젝트 설정
```
<br/>  
<br/>
  
## ✅ 실행 방법
### 프론트엔드
```bash
cd diary-main
flutter pub get
flutter run
```
<br/>

### 백엔드
```bash
cd backend-main
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```
<br/>
<br/>
