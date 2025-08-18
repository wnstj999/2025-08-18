# 오늘 학습

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
