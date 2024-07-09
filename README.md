
<div align= "center">WorkAid BackOffice Front</div>
<br/>

# 🛠️ Built With

- React
- Typescript
- Redux
- sass
  <br/>
  <br/>

### Source Code Editor

Visual Studio Code

[다운받기](https://code.visualstudio.com/download)
<br/>
<br/>

### Git Information

| UTEC GIT 종류 | Bonobo Git Server                                                                                          |
| ------------- | ---------------------------------------------------------------------------------------------------------- |
| URL           | http://218.50.154.98:3000/Bonobo.Git.Server/Home/LogOn?ReturnUrl=%2FBonobo.Git.Server%2FRepository%2FIndex |
| username      | admin                                                                                                      |
| password      | 권지수/홍승표 대리님께 문의                                                                                |

| 기존 jsp 프로젝트 URL
(groupware_backoffice) | http://218.50.154.98:3000/Bonobo.Git.Server/Repository/Detail/bd2d6b31-aa99-44bb-ba7f-c4815aee843f |
| 사용법 참고 링크 | https://luvris2.tistory.com/429#google_vignette |
<br/>
<br/>

### Google Cloud Information(Google login & API)

| Web Client | https://console.cloud.google.com/apis/credentials/oauthclient/932432376019-0fpmse70honc5t713f6jatnmgrtlv30i.apps.googleusercontent.com?authuser=3&project=groupware-864fb&supportedpurview=project |
| ---------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ID         | mailto:dev@utec.kr                                                                                                                                                                                 |
| PW         | 홍승표 대리님 혹은 김동석 부장님께 문의                                                                                                                                                            |

  <br/>
  <br/>

### WorkAid BackOffice Information

| JSP 관련 문의                       | 권지수 대리님, 홍승표 대리님(기존 작업물은 퍼블리셔가 따로 있었음)                                                                              |
| ----------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| FIgma (디자인 팀에게 요청 필요)     | https://www.figma.com/design/XAw5TNsmyl9PB9C4hGTFds/%EA%B7%B8%EB%A3%B9%EC%9B%A8%EC%96%B4-IA_Back-office?node-id=5359-30881&t=v6JD3hL5Plu5WsCk-1 |
| Zeplin (디자인 팀에게 요청 필요)    | https://app.zeplin.io/project/6684a782cba1436f9877949f/screen/6684a7fee330f6a845ce2de6                                                          |
| live server                         | https://office.workaid.ai/                                                                                                                      |
| dev server                          | https://office.utec.kr/                                                                                                                         |
| live server API Swagger for flutter | https://gwapi.workaid.ai/swagger/swagger-ui/index.html#/Work%20API                                                                              |
| dev server API Swagger for flutter  | https://gwapi.utec.kr/swagger/swagger-ui/index.html#/Work%20API                                                                                 |
| header&menu animation ref1          | https://angular-material.fusetheme.com/sign-in?redirectURL=%2Fdashboards%2Fanalytics                                                            |
| header&menu animation ref2          | https://mofidjango.pixelstrap.net/login_home?next=/dashboard_03                                                                                 |

  <br/>
  <br/>

### utec-groupware-webapp/ 프로젝트 구조

```bash
utec-groupware-webapp/
│
├── public/                         # 정적 파일
│   ├── index.html                  # 메인 HTML 파일
│   ├── logo192.png                 # 웹사이트 로고 아이콘(192px)
│   ├── logo512.png                 # 웹사이트 로고 아이콘(512px)
│   └── favicon.ico                 # 웹사이트 파비콘
│
├── src/                            # 소스 코드 저장 디렉토리
│   ├── components/                 # 재사용 가능한 UI 컴포넌트 디렉토리
│   │   ├── chart/                  # 차트 관련 컴포넌트 모음
│   │   │   └── Barchart/           # BarChart 차트 컴포넌트
│   │   ├── common/                 # 일반적으로 사용되는 컴포넌트 모음
│   │   │   ├── Header/             # Header 컴포넌트 (상단)
│   │   │   └──HeaderMenu /         # HeaderMenu 컴포넌트 (왼쪽 사이드)
│   │   ├── layout/                 # 레이아웃 관련 컴포넌트 모음
│   │   │   ├── MainLayout/         # 로그인 분기 후 보여지는 레이아웃 컴포넌트(ex. 대시보드)
│   │   │   └──PublicLayout /       # 로그인 전 보여지는 레이아웃 컴포넌트
│   │   └── modal/                  # 팝업/모달 관련 컴포넌트 모음
│   │       └──nonModal /           # 논모달 관련 컴포넌트 모음
│   │           └──InfoPersonal /   # Header 컴포넌트에 사용되는 로그아웃 버튼있는 논모달 컴포넌트
│   │
│   ├── hooks/                      # custom hook 디렉토리
│   │
│   ├── pages/                      # page 디렉토리
│   │   ├── DashBoard/              # 대시보드 페이지
│   │   ├── Login/                  # 로그인 페이지
│   │   └── NotFound/               # 404 / NotFound 페이지
│   │
│   ├── assets/                     # 이미지, 폰트 등의 정적 리소스 디렉토리
│   │   ├── images/                 # 이미지 모음(가장 상위에는 jsp 프로젝트에서 사용하던 이미지들 포함됨)
│   │   │   └──update1.0 /          # jsp 프로젝트에서 react로 개발하면서 추가된 이미지 모음
│   │   │       └──icons /          # icon 이미지만 모음
│   │   ├── scss/                   # 공통사용되는 scss 모음
│   │   └── webfonts/               # 웹폰트 모음
│   │
│   ├── shared/                     # 유틸리티 함수 + router 관련 디렉토리
│   │   ├── routes/                 # router 관련 모음(ex. 페이지 추가시 routing도 추가 필요, 로그인/비로그인에 따라 분기처리 하기 위해 따로 관리)
│   │   └── utils/                  # 유틸리티 함수 모음(ex. fullscreen)
│   │
│   └── store/                      # Redux 디렉토리

```

  <br/>
  <br/>

### package.json

```json
{
  "name": "utec-groupware-webapp",
  "version": "0.1.0",
  "private": true,
  "dependencies": {
    "@react-oauth/google": "^0.12.1", // google login
    "@reduxjs/toolkit": "^2.2.6", // redux 간편화를 위함
    "@testing-library/jest-dom": "^5.17.0",
    "@testing-library/react": "^13.4.0",
    "@testing-library/user-event": "^13.5.0",
    "@types/jest": "^27.5.2",
    "@types/react": "^18.3.3",
    "@types/react-chartjs-2": "^2.5.7", // chart.js 라이브러리
    "@types/react-dom": "^18.3.0",
    "chart.js": "^4.4.3", // chart.js 라이브러리
    "chartjs-plugin-datalabels": "^2.2.0", // chart.js 라이브러리
    "react": "^18.3.1",
    "react-chartjs-2": "^5.2.0", // chart.js 라이브러리
    "react-dom": "^18.3.1",
    "react-helmet": "^6.1.0", // SEO
    "react-helmet-async": "^2.0.5", // SEO
    "react-scripts": "5.0.1",
    "swiper": "^11.1.4", // Swiper -> login 페이지 swiper에 사용됨
    "tsconfig-paths-webpack-plugin": "^4.1.0", // 프로젝트 Alias 절대경로 설정을 위해 사용
    "typescript": "^4.9.5", // typescript 기반의 프로젝트입니다
    "web-vitals": "^2.1.4"
  },
  "scripts": {
    "start": "craco start", // 프로젝트 Alias 절대경로 설정을 위해 craco 사용
    "build": "craco build", // 프로젝트 Alias 절대경로 설정을 위해 craco 사용
    "test": "craco test", // 프로젝트 Alias 절대경로 설정을 위해 craco 사용
    "eject": "react-scripts eject",
    "postbuild": "react-snap" // SEO
  },
  "eslintConfig": {
    "extends": ["react-app", "react-app/jest"]
  },
  "browserslist": {
    "production": [">0.2%", "not dead", "not op_mini all"],
    "development": [
      "last 1 chrome version",
      "last 1 firefox version",
      "last 1 safari version"
    ]
  },
  "devDependencies": {
    "@craco/craco": "^7.0.0",
    "@types/node": "^20.14.9",
    "@types/react-paginate": "^7.1.1", // 게시판 등 페이지네이션 용
    "@types/react-redux": "^7.1.25", // Redux
    "@types/react-router-dom": "^5.3.3", // 페이지 라우팅 처리
    "axios": "^1.3.4", // API통신용
    "classnames": "^2.3.2", // classNames 기능용
    "jest": "^29.6.1", // TDD
    "react-paginate": "^8.1.4", // 게시판 등 페이지네이션 용
    "react-redux": "^8.0.5", // Redux
    "react-router-dom": "^6.7.0", // 페이지 라우팅 처리
    "react-snap": "^1.23.0", // SEO
    "redux": "^5.0.1", // Redux
    "redux-persist": "^6.0.0", // Redux 상태 초기화 방지
    "sass": "^1.57.1" // SCSS로 CSS 개발 중
  }
}
```

  <br/>
  <br/>

### 프로젝트 실행 방법

1. 프로젝트 시작 전 최상위 폴더에 .env.development 파일 추가 필요

```bash
# dev server
# REACT_APP_API_URL = https://office.utec.kr
# 홍승표 대리님 로컬로 켜주신 서버(켜주셔야만 사용 가능)
REACT_APP_API_URL = http://192.168.220.225:8099
# local server
# REACT_APP_API_URL = http://localhost:8099
# live server
# REACT_APP_API_URL = https://office.workaid.ai

```

1. 프로젝트 시작 전 yarn 의존성 설치 필요

```bash
yarn install
```

1. 프로젝트 시작

```bash
yarn run dev
```

1. [localhost:3000](http://localhost:3000) 확인
   <br/>
   <br/>

# 📄 License

This project is licensed under the terms of the [UTEC](https://www.utec.kr/) license.
<br/>
<br/>
