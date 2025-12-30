# KICK-ON

> 참여형 축구 커뮤니티 플랫폼 (🏆 프로젝트 2등)

[라이브 데모](https://dev.kickon.net/) | [디자인 시안 (Figma)](https://www.figma.com/design/x9wbW2UCBiRpgWwiH1Idgg/kickon-frontend?node-id=0-1&t=5ZTph6WCKxmV5Ewq-1)

## 프로젝트 개요

킥온은 축구 팬들을 위한 통합 플랫폼으로, AI 기반 이적 예측, 실시간 뉴스, 커뮤니티 게시판, 중고 거래 등 다양한 기능을 제공하는 참여형 축구 커뮤니티입니다. 팬 간 소통과 정보 공유를 활성화하며, 진정한 참여형 축구 커뮤니티를 지향합니다.

<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/8bd85549-2085-4c98-a27c-96c321a8b0ae" width="420" /></td>
    <td><img src="https://github.com/user-attachments/assets/95912a39-34ba-48ff-a739-647ed735655f" width="420" /></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/324de23e-ab56-42e7-b9ba-7b0bc40db9d8" width="420" /></td>
    <td><img src="https://github.com/user-attachments/assets/5c7a2bab-1221-4a4c-86fa-6f2409ff4d57" width="420" /></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/e54f862f-0da2-4e55-a36e-374885c12dc9" width="420" /></td>
    <td><img src="https://github.com/user-attachments/assets/5e2e9b4a-4943-4ec0-8deb-ab9810325f85" width="420" /></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/8128a0a4-3c08-4045-9085-723a4ce31a9d" width="420" /></td>
    <td><img src="https://github.com/user-attachments/assets/24eef543-cec9-41bb-a8c3-716ce28be080" width="420" /></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/e0e8f769-1a1e-4386-a059-3ce876884092" width="420" /></td>
    <td><img src="https://github.com/user-attachments/assets/c497ba72-9b5a-4e76-8fcf-a4c9d74a7303" width="420" /></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/dc1e8473-9412-4f39-a730-3f40d318e5f9" width="420" /></td>
    <td><img src="https://github.com/user-attachments/assets/cfbcc07d-ed9b-4a10-92dd-4cd2b476b088" width="420" /></td>
  </tr>
</table>

---

## 주요 기능

### 1. AI 기반 이적 예측
- 선수 이름을 입력하여 이적 가능성 예측
- AI 모델을 통한 이적 확률 및 관련 뉴스 제공
- 실시간 예측 결과 시각화

### 2. 축구 뉴스 및 커뮤니티
- 최신 축구 뉴스 조회 및 상세 보기
- 커뮤니티 게시판 (글 작성, 수정, 삭제, 댓글)
- 리치 텍스트 에디터를 활용한 게시글 작성
- 팀별/리그별 게시글 필터링

### 3. 중고 거래
- 축구 용품 중고 거래 게시판
- 가격 및 연락처 정보 입력
- 상세 페이지를 통한 거래 정보 확인

### 4. 승부예측 및 순위
- 경기 결과 예측 기능
- 시즌 순위 및 승부예측 순위 표시
- 사용자 랭킹 시스템

### 5. 사용자 인증 및 프로필
- 소셜 로그인 (카카오, 네이버)
- 사용자 프로필 관리
- 개인정보 설정

---

## 기술 스택

### Frontend
- **Framework**: React 19
- **Build Tool**: Vite 6.2.4
- **Routing**: React Router v7.4.1
- **State Management**: 
  - Redux Toolkit 2.6.1
  - Zustand 5.0.3
- **Styling**: Styled Components 6.1.16
- **Form Management**: 
  - React Hook Form 7.54.2
  - Yup 1.6.1
- **Rich Text Editor**: 
  - React Quill New 3.4.6
  - Quill 2.0.3
- **HTTP Client**: Axios 1.8.4
- **Date Handling**: Day.js 1.11.13
- **HTML Parsing**: html-react-parser 5.2.3
- **Icons**: 
  - React Icons 5.5.0
  - Lucide React 0.484.0
- **Security**: DOMPurify 3.2.6
- **Markdown**: Marked 15.0.12

### Development Tools
- **Linting**: ESLint 9.21.0
- **Plugin**: @vitejs/plugin-react-swc 3.8.0

---

## 프로젝트 구조

```
kickon-frontend-dev/
├── public/                 # 정적 파일
├── src/
│   ├── apis/              # API 통신 모듈
│   │   ├── axios-instance.js
│   │   └── domains/       # 도메인별 API
│   │       ├── auth/      # 인증 관련
│   │       ├── common/    # 공통 기능
│   │       ├── community/ # 커뮤니티
│   │       ├── main/      # 메인 페이지
│   │       ├── market/    # 중고 거래
│   │       ├── news/      # 뉴스
│   │       ├── ranking/   # 순위
│   │       └── report/    # 신고
│   ├── assets/            # 이미지 및 아이콘
│   ├── components/        # 재사용 가능한 컴포넌트
│   │   ├── Comment/       # 댓글 컴포넌트
│   │   ├── CommunityBoard/# 커뮤니티 게시판
│   │   ├── Header/        # 헤더
│   │   ├── Footer/        # 푸터
│   │   ├── LoginModal/    # 로그인 모달
│   │   ├── PostEditor/    # 게시글 에디터
│   │   ├── RankingTable/  # 순위 테이블
│   │   └── ...
│   ├── context/           # React Context
│   │   └── AuthContext.jsx
│   ├── features/          # Redux features
│   │   └── modal/
│   ├── hooks/             # Custom Hooks
│   │   ├── useAuthGuard.js
│   │   ├── useCustomFetch.js
│   │   └── useForm.js
│   ├── layout/            # 레이아웃 컴포넌트
│   │   └── root-layout.jsx
│   ├── pages/             # 페이지 컴포넌트
│   │   ├── Home/          # 홈
│   │   ├── Community/     # 커뮤니티
│   │   ├── News/          # 뉴스
│   │   ├── Market/        # 중고 거래
│   │   ├── Transferability/# 이적 예측
│   │   ├── ProfileSettings/# 프로필 설정
│   │   └── Signup/        # 회원가입
│   ├── store/             # 상태 관리
│   │   ├── store.js       # Redux store
│   │   └── useLeagueTeamStore.js # Zustand store
│   ├── utils/             # 유틸리티 함수
│   │   ├── formatDate.js
│   │   ├── imageUpload.js
│   │   ├── timeUtils.js
│   │   └── ...
│   ├── App.jsx            # 메인 App 컴포넌트
│   └── main.jsx           # 진입점
├── package.json
├── vite.config.js
└── README.md
```

---

## 설치 및 실행

### 필수 요구사항
- Node.js 22.x (권장)
- npm 또는 yarn

### 설치

```bash
# 의존성 설치
npm install
# 또는
yarn install
```

### 환경 변수 설정

프로젝트 루트에 `.env` 파일을 생성하고 다음 변수를 설정하세요:

```env
VITE_BASE_URL=your_api_base_url
VITE_API_PREDICT_URL=your_predict_api_url
```

### 개발 서버 실행

```bash
npm run dev
# 또는
yarn dev
```

개발 서버는 기본적으로 `http://localhost:5173`에서 실행됩니다.

### 빌드

```bash
npm run build
# 또는
yarn build
```

빌드된 파일은 `dist` 폴더에 생성됩니다.

### 프로덕션 미리보기

```bash
npm run preview
# 또는
yarn preview
```

---

## 서비스 아키텍처

![서비스 아키텍처](https://github.com/user-attachments/assets/584e4074-cf6e-43e0-92bb-e5ea2da2a9b5)

---

## 주요 구현 사항

### 상태 관리 전략
- **Redux Toolkit**: 전역 모달 상태 관리
- **Zustand**: 리그/팀 선택 상태 관리 (세션 스토리지 영속화)
- **React Context**: 인증 상태 관리

### 라우팅
- React Router v7을 활용한 SPA 라우팅
- 동적 라우팅을 통한 상세 페이지 구현
- 인증 가드 훅을 통한 보호된 라우트 관리

### 컴포넌트 설계
- 재사용 가능한 컴포넌트 구조
- Styled Components를 활용한 스타일링
- 반응형 디자인 구현 (모바일/데스크톱)

### API 통신
- Axios 인스턴스를 통한 중앙화된 API 관리
- 도메인별 API 모듈화
- 커스텀 훅을 통한 데이터 페칭

---

## 팀원

- [이해령](https://github.com/haerxeong)
- [윤정민](https://github.com/2ivii)
- [박상원](https://github.com/psw204)

---

## 문의

프로젝트에 대한 문의사항이 있으시면 아래 이메일로 연락해주세요.

- 이메일: kickon.project@gmail.com

