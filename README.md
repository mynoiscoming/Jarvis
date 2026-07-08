# 🤖 JARVIS AI Assistant

**대화형 홀로그램 인터페이스를 갖춘 AI 비서 시스템**

## ✨ 기능

### 🔐 사용자 인증
- **회원가입**: 새로운 프로필 생성 (최대 4명)
- **로그인**: 이메일과 비밀번호로 안전하게 접속
- **로컬스토리지 저장**: 브라우저에 자동 저장

### 🎯 할 일 관리
- 자비스에게 "~을 목록에 추가해줘" 명령으로 작업 추가
- 체크박스로 완료한 작업 삭제
- 실시간 동기화

### 🎤 음성 인식 & TTS
- 브라우저 기본 음성 합성 기능
- 자비스의 한영 혼합 대화
- 명령어 인식:
  - "안녕" / "hello" → 인사말
  - "이름" / "who are you" → 자기소개
  - "고마워" / "thank you" → 감사 인사

### 🌌 홀로그램 애니메이션
- Canvas 기반 미래형 그래픽
- 실시간 입자 효과
- 음성 재생 시 홀로그램 반응

## 🚀 사용 방법

### 1️⃣ 회원가입
1. "새 프로필 생성하기" 클릭
2. 사용자 이름, 이메일, 비밀번호 입력
3. "프로필 생성" 클릭

### 2️⃣ 로그인
1. 이메일과 비밀번호 입력
2. "접속하기" 클릭
3. JARVIS 시스템 접근

### 3️⃣ 명령어 사용
```
예시 명령어:
- "안녕하세요"
- "이름이 뭐예요?"
- "할 일을 추가해줘"
- "오늘 공부하기 목록에 추가해줘"
```

## 📁 파일 구조

```
Jarvis/
├── index.html      # 메인 애플리케이션
└── README.md       # 프로젝트 설명
```

## 🌐 배포 (GitHub Pages)

이 프로젝트는 GitHub Pages에서 자동으로 배포됩니다:

🔗 **사이트 주소**: https://mynoiscoming.github.io/Jarvis/

### 배포 설정
1. GitHub 저장소의 **Settings** → **Pages**
2. **Source**를 `main` 또는 기본 브랜치로 설정
3. 자동으로 배포 완료!

## 💾 데이터 저장

- 모든 사용자 데이터는 **브라우저 LocalStorage**에 저장됩니다
- 새 탭/창에서도 동일한 데이터에 접근 가능
- 브라우저 캐시 삭제 시 데이터 소실

## 🛠️ 기술 스택

- **Frontend**: HTML5, CSS3, JavaScript (Vanilla)
- **Data Storage**: LocalStorage API
- **Audio**: Web Speech API (TTS)
- **Graphics**: Canvas API
- **Hosting**: GitHub Pages

## 📱 지원 환경

- ✅ Chrome/Edge (음성 합성 완벽 지원)
- ✅ Firefox (음성 합성 부분 지원)
- ✅ Safari (음성 합성 부분 지원)
- ✅ 모바일 브라우저 (제한적)

## 🎨 커스터마이징

### 색상 변경
`index.html` 파일의 CSS 변수를 수정:
```css
:root {
    --neon-blue: #00f3ff;  /* 기본 색상 변경 */
    --bg-color: #0a0f1d;   /* 배경색 변경 */
}
```

### 자비스 응답 추가
`handleAuth()` 함수의 command 처리 부분에 새로운 조건 추가:
```javascript
} else if (command.includes("커스텀 명령어")) {
    jarvisSpeak("응답 메시지");
}
```

## 📝 라이선스

자유롭게 사용, 수정, 배포 가능합니다.

## 👨‍💻 개발자

**mynoiscoming** - JARVIS AI Assistant Creator

---

**마지막 업데이트**: 2024년
