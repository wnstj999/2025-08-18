# 오늘 학습 최종단

📡 GNB vs LNB 정리
1. GNB (gNB, Next Generation NodeB)

의미: 5G NR(New Radio)에서 사용하는 기지국(Base Station)

**4G의 eNB(evolved NodeB)**에 해당하는 개념

구성 요소:

CU (Central Unit): 중앙 처리 기능 담당 (제어 및 일부 사용자 plane 처리)

DU (Distributed Unit): 기지국에 가까운 분산 처리 장치 (저지연 사용자 plane 처리)

RU (Radio Unit): 실제 안테나와 연결되어 RF 신호 송수신 담당

기능:

무선 자원 제어(RRC)

스케줄링, 핸드오버

사용자 데이터 송수신 (5G Core와 연결)

➡️ 쉽게 말하면, 5G 무선망에서 사용자 단말(UE)과 5G Core를 연결하는 기지국 역할

2. LNB (Low Noise Block Downconverter)

의미: 위성 통신(Satellite Communication)에서 사용되는 저잡음 블록 변환기

위성 안테나(패러볼라 접시)에 장착되는 장치

역할:

위성에서 내려오는 고주파(Ku-band, Ka-band 등) 신호를 수신

신호를 증폭(저잡음 증폭, LNA 기능)

**저주파(IF, Intermediate Frequency)**로 변환 → 케이블을 통해 셋톱박스/모뎀으로 전달 가능

특징:

위성 수신 환경에서 잡음 지수(Noise Figure) 최소화

장거리 전송을 위해 주파수 변환과 저손실 신호 전달 지원

➡️ 쉽게 말하면, 위성 안테나에서 수신한 약한 신호를 증폭하고 처리하기 쉬운 주파수로 변환하는 장치

📄 MD (Markdown) 파일이란?

확장자 .md 를 가진 텍스트 파일

Markdown(마크다운) 이라는 문법을 사용해서 작성한 문서

마크다운은 글을 꾸미는 약속 같은 거예요.
→ 워드처럼 버튼을 눌러 굵게/제목/표를 만드는 게 아니라,
→ *특수문자(#, , - 등) 를 이용해서 텍스트만으로 서식을 표현하는 방식이에요.

✨ 왜 쓰냐?

가볍고 읽기/쓰기 쉬움 (일반 텍스트 기반)

GitHub, GitLab, Notion 같은 서비스에서 자동으로 예쁘게 변환됨

협업용 문서, 가이드, 설명서(특히 README.md)에 많이 사용됨

🎨 UI와 UX 정리
1. UI (User Interface, 사용자 인터페이스)

정의: 사용자가 제품·서비스와 직접 상호작용하는 화면이나 요소

포함되는 것들:

버튼, 메뉴, 아이콘, 글꼴, 색상, 레이아웃

웹사이트 디자인, 앱 화면, 컨트롤 패널 등

초점: "보이는 것"과 "조작하는 방법"

👉 쉽게 말해 “겉모습과 조작법”

2. UX (User Experience, 사용자 경험)

정의: 사용자가 제품·서비스를 사용하면서 느끼는 총체적인 경험

포함되는 것들:

사용 편리성(Usability)

직관적 흐름(Information Architecture)

감정적 만족감

접근성, 속도, 신뢰성

초점: "느낌, 만족도, 효율성"

👉 쉽게 말해 “써보니 어땠는가”

1️⃣ 웹/보안 분야: Content Security Policy (CSP)

정의: 웹 페이지에서 어떤 리소스(스크립트, 이미지, 스타일 등)를 허용할지 브라우저에 알려주는 보안 정책

목적: XSS(교차 사이트 스크립팅) 공격, 데이터 인젝션 방지

예시:

Content-Security-Policy: default-src 'self'; img-src https://example.com; script-src 'self' https://cdn.example.com


설명:

default-src 'self' → 기본 리소스는 자기 서버만 허용

img-src https://example.com → 이미지는 example.com에서만 불러오기

script-src ... → 스크립트는 자기 서버와 CDN만 허용

2️⃣ 통신/전력 분야: Cloud Service Provider

정의: 클라우드 서비스를 제공하는 회사(예: AWS, Azure, GCP)

역할: 서버, 스토리지, DB, 네트워크, 보안 서비스 제공

3️⃣ 보안 인증: Cryptographic Service Provider

정의: 암호화 서비스(키 생성, 인증서 관리 등)를 제공하는 소프트웨어/모듈

사용 예: Windows에서 인증서 기반 암호화, 디지털 서명

💡 요약

웹 개발 관련이면 → Content Security Policy

클라우드 관련이면 → Cloud Service Provider

암호화/보안 관련이면 → Cryptographic Service Provider

Workspace (워크스페이스)란?

의미: 개발자가 작업하는 프로젝트 작업 공간

VS Code에서는 폴더, 설정, 확장, 터미널 환경 등을 하나로 묶어서 관리하는 단위예요.

쉽게 말하면 **“이 프로젝트만을 위한 VS Code 환경”**이라고 생각하면 됩니다.

종류
1️⃣ 폴더 워크스페이스 (Folder Workspace)

특징: 단일 폴더를 열어서 작업

.vscode 폴더 안에 프로젝트 설정 저장

장점: 설정이 단순하고 바로 사용 가능

사용 예: 작은 프로젝트, 단일 폴더 작업

2️⃣ 멀티 루트 워크스페이스 (Multi-root Workspace)

특징: 여러 폴더를 하나로 묶어서 관리

.code-workspace 파일로 워크스페이스 설정 저장

장점: 여러 프로젝트를 한 VS Code 창에서 관리 가능

사용 예: 프론트엔드/백엔드가 다른 폴더일 때

설정 방법

폴더 워크스페이스:

폴더 열기 → 자동으로 워크스페이스 생성

.vscode/settings.json에 프로젝트별 설정 저장

멀티 루트 워크스페이스:

File > Add Folder to Workspace → 여러 폴더 추가

File > Save Workspace As… → .code-workspace 파일로 저장

VS Code에서 확인/전환

왼쪽 상단 폴더 이름 → 현재 워크스페이스 확인 가능

File > Open Workspace… → 다른 워크스페이스 열기

💡 핵심 요약:

워크스페이스 = 프로젝트 작업 공간

폴더 워크스페이스 = 단일 프로젝트

멀티 루트 워크스페이스 = 여러 프로젝트를 한 번에 관리
