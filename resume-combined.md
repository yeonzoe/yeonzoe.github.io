# 연향주 — QA Manager · Senior QA Engineer

**QA MANAGER · SENIOR QA ENGINEER (PLAYING MANAGER) · 13+ YEARS**

- 📧 hjyeon0917@gmail.com
- 🐙 github.com/yeonzoe
- 🔗 yeonzoe.github.io

> 매니저 + 엔지니어 통합본 — QA 조직·프로세스를 직접 설계·운영하면서 코드 레벨까지 hands-on으로 의사결정하는 플레잉 매니저.

---

## Summary

6개사에서 QA 조직을 **처음부터 설계·운영**해온 매니저 — 1인 QA·아르바이트 구조에서 정규직 전문 조직으로의 리빌딩을 4회 수행.
배포 프로세스 안정화 · **외주 업체 계약·운영 전 주기 관리** · R&R 설계 · 운영 이슈 보고 체계까지 조직 전 영역 직접 정립.
동시에 자동화 **969건**을 직접 설계·구현하고, Playwright(TS) · pytest · Maestro로 3단계 CI 품질 게이트(Preview → Beta → Production)를 구성.
Claude Code · MCP 기반 AI QA 파이프라인을 직접 구축·플러그인으로 패키징해 팀에 배포·운영 — 코드 레벨에서 의사결정하는 **플레잉 매니저**.
현재 직방·호갱노노·다음부동산 3개 서비스 QA 총괄, 수동 공수 **58% 절감**.

---

## Experience

### 직방 (ZIGBANG Co., Ltd) — QA Manager · 팀장
`2024.07 — 현재`

**조직 · 운영**
- **QA 조직 전면 리빌딩** — CS 겸임·시간제 아르바이트 구조 → 정규직 2인 + 계약직 2인 전문 조직으로 전환, R&R 정의
- **소속 조직 이동 협상·실행** — 서비스 운영 조직 → Tech 조직, QA 활동 범위를 운영 업무에서 서비스 품질 전반으로 확장
- **QA 외주 업체 계약·운영 총괄 (장기·단기·프로젝트 계약)** — 계약 유형별 복수 업체 견적·특성(상주 가능 여부·자동화 역량·투입 인력) 비교 후 선정 → 단가 조정·계약 체결(NDA) → 장기 상주(상시 회귀)·단기(배포 집중)·프로젝트(신규 기능) 업무 배분 → 외주 인력 온보딩·테스트 가이드·리소스 배분·산출물 리뷰까지 전 주기 관리
- **테스트 디바이스 자산 관리 체계 구축** — 업무용 디바이스 대여 프로세스 정립, 외주 인력 대여 연계
- **스프린트·배포 주기 구조 개편**, 직방/호갱노노 이슈 등록·관리 체계 통합, 모니터링 관제 → AI 모니터링 구조 전환

**엔지니어링 산출물**
- **통합 검증 정착으로 Critical 결함 41%↓** — 스프린트 통합 검증 프로세스 확립 후 Critical(High+Urgent) 버그 17건 → 10건으로 감소, 배포 전 미해결 0건 유지 (4개 스프린트 처리율 100%)
- **자동화 0 → 969건 직접 설계·구현** — Playwright(TypeScript) 웹 E2E **272**건 · pytest API **446**건 · Maestro 모바일 **251**건. ISO 25010 기반 11-컬럼 TC 표준 정의, 블랙박스 5기법(동등분할·경계값·결정테이블·상태전이·유스케이스) 전수 적용
- **3단계 CI 품질 게이트 구축** — Preview → Beta → Production 각 단계 GitHub Actions 자동 트리거, Allure 리포트 자동 배포, Slack 장애 알림 연동
- **AI QA 자동화 파이프라인 직접 구축** — 커스텀 Skills 27개 · Slash Commands 30여 개 · Hooks 12종 · MCP 연동 직접 구현. PRD 정제·구조 스캔(시프트 레프트) → TC 자동 생성 → Web/API/App 통합 sanity orchestrator → 회귀 영향 범위 자동 산출까지 엔드-투-엔드
- **QA 자동화 도구를 플러그인으로 패키징해 팀에 배포·버전 운영** — 사내 마켓플레이스 플러그인(v2.4.0)으로 패키징, product-hub MCP 연동으로 실제 BE 코드베이스 기반 TC 자동 생성까지 확장. 수동 공수 **58% 절감**
- **네트워크 계층 디버깅 표준화** — HTTP Toolkit(HTTPS 프록시·요청/응답 재현) · Flipper(iOS·Android 네트워크·로그·스토리지) · Postman으로 결함 재현성 확보
- **QA 대시보드 구축** — 스프린트 단위 TC 실시간 현황, GitHub Actions 자동 동기화, Allure·Slack 리포팅 통합

### 머스트잇 (명품 커머스) — QA Manager · 팀장
`2023.10 — 2024.06 · 9개월`

- **QA 조직 신설** — 개발팀 겸임 구조 → 독립 QA팀 분리, Jira 전용 프로젝트 + 이슈 자동 복제 워크플로우 개발
- **QA 전용 테스트 환경 구축** — QA/Staging 인프라 분리, Apple Enterprise Membership 추가 가입, App 디버깅 환경 정비로 긴급 배포 반복 사이클 제거
- **4단계 검증 프로세스 표준화** — 기획 → 인수 → 회귀 → 스테이징, 배포 판단 기준 **7항목** 문서화
- **전사 테스트 관리 툴 도입** — AIO Test Management Tool 선정·전파, Kick-Off부터 Sign-Off까지 템플릿 정립
- **운영 이슈 보고 프로세스 정립**, 배포 버전 관리 방식 개선(BE/FE/Native App 통합 버전 관리)
- 메인홈 · 카테고리 · GNB · 상품목록/상세 · 필터 · 찜 전면 개편 프로젝트 SDLC 리딩 (PO 없는 Agile 구조 대응)

### 그라운드엑스 (Ground X · Klaytn) — QA Manager · 파트 리드
`2022.03 — 2023.10 · 1년 8개월`

- **외주 QA 운영 체계 구축 (프로젝트 계약)** — 복수 업체 견적·도메인 전문성 비교 후 선정 → 프로젝트 단위 리소스(M/M) 산정·단가 조정·계약 체결(NDA) → 외주 테스터 가이드 제공·산출물 리뷰까지 전 주기 직접 운영, 외주 운영 비용 **40% 절감**
- **클립 지갑 5계층 통합 QA 설계** — 앱 · 웹 · 서버 · BOF · bapp SDK Full Coverage TC + 쿠버네티스 대시보드 활용 서버 환경 검증
- **카카오톡 지갑-NFT 연동 전수 검증** — 상태전이 기법으로 인증 실패·만료·재시도 20+ 시나리오 검증
- **NFT 테스트 데이터 생성 자동화** — 수동 20분 → 자동 2분, 대량 민팅으로 성능 부하 데이터셋 확보
- **BDD 기반 3단계 문서 체계 수립** — 체크리스트 · 테스트케이스 · 시나리오 구분, Daily Scrum·주간 보고·회고로 QA 공유 문화 정착
- 토큰 스왑 · 멀티체인 · 오픈월렛 · NFT 체크인/에어드랍 · Bapp API Service 신규 기능 런칭 QA 주도

### 야놀자Tech (R&D) — QA Manager
`2020.10 — 2022.03 · 1년 6개월`

- **회원가입 완료율 20% 개선** — 동등분할·경계값 분석으로 이탈 지점 식별, 멤버급 등급 상향 사용자 **30% 증가**
- **초기 결함 검출률 40% 상승** — 동치분할·경계값·상태전이 기법을 팀 표준으로 정착
- **데일리호텔 통합 TC 0건 → 전수 재설계** — 포인트 · 트루리뷰 · 서브홈 · 결제수단 영역 TC 신규 작성·체계화
- 이해관계자 간 진척도·이슈 에스컬레이션 규칙 정의

### 이우소프트 — QA Manager
`2016.12 — 2020.03 · 3년 4개월`

- **AI 의료 진단 SW QA** — FDA · 식약처 의료 인증 TC 설계 및 획득, **2019 대한민국 SW 기술대상 수상** 프로젝트 참여
- **Selenium · Python 자동화 도입** — 반복 수행 TC 자동화로 수행 시간 단축
- **3단계 품질 프로세스 수립** — Alpha → Beta → FCS 단계별 TC 기준 정의
- **X-ray Detector HW-SW 인터페이스 검증 프로세스 수립** — 무선 Detector 장비 양산 출시 지원

### 아이온커뮤니케이션즈 (CMS 솔루션) — QA Manager
`2012.07 — 2016.11 · 4년 5개월`

- **일본향 CMS 솔루션 ISO 9126 기반 품질 관리** — 일본 시장 매출 1위(2015~2016) 기간 품질 담당, 시장 점유율 **18.8%**
- **비대면 계약 e.Form io 온프레미스 → AWS 클라우드 전환 검증** — Waterfall → Agile 전환 시 QA 프로세스 재설계
- **일본 고객 VOC 70% 직접 대응** — 일본어 원문 분석·번역, 기술 문서 작성 겸임

---

## Skills

| 영역 | 내용 |
|---|---|
| 리더십 · QA 전략 | QA 조직 빌딩(0→1, 1→N), **외주 업체 계약·단가 협상·인력 가이드·관리(장기·단기·프로젝트)**, R&R 설계, 배포 프로세스 정립, 이슈 에스컬레이션 규칙, 이해관계자 커뮤니케이션, 회고·공유 문화 정립 |
| 테스트 설계 | 블랙박스 5기법(동등분할 · 경계값 · 결정테이블 · 상태전이 · 유스케이스), BDD(GWT), Risk-Based Testing, Test Pyramid, 품질 게이트 설계, ISO 25010 / ISO 9126 |
| 자동화 | Playwright (TypeScript), pytest, Maestro, Appium, Selenium, REST Assured, Newman, Allure |
| API 테스트 | Postman, Newman, pytest + requests, OpenAPI/Swagger 검증 |
| AI 워크플로우 | Claude Code (커스텀 Skills 27개 · Slash Commands 30여 개 · Hooks 12종 직접 구현 · 사내 마켓플레이스 플러그인 v2.4.0 패키징·배포), Cursor, MCP 연동(product-hub·Figma·Playwright), Spec-Driven Development, AI 보조 개발(vibe coding) 품질 보장 파이프라인 |
| 디버깅 · 네트워크 | HTTP Toolkit, Flipper (iOS·Android), Charles Proxy, Wireshark, Xcode, Android Studio |
| CI / CD | GitHub Actions, Slack Webhook, Preview/Beta/Production 멀티 스테이지 |
| 언어 · DB | Python, TypeScript, JavaScript, SQL (Oracle · PostgreSQL · MongoDB), Git, Linux |
| 도메인 | PropTech(부동산), 커머스(명품·여행·숙박), 핀테크(블록체인·NFT 지갑·SDK), 의료 AI(FDA·식약처), CMS(B2B 일본) |

> **도메인 적응력** — 규제 도메인(의료 AI FDA·핀테크 블록체인)과 고속 성장 플랫폼(커머스·프롭테크)을 모두 경험하며 **어떤 환경에서도 빠르게 품질 프로세스를 셋업**. 일본향 CMS 품질 관리 경험 + 일본어(JLPT 2급·OPIc AL)로 **글로벌(일본 시장) 확장 QA·커뮤니케이션** 직접 대응.

---

## Education

- **한국교통대학교** — 컴퓨터과학과 (졸업) · 2008 — 2010
- **경북전문대학** — 디지털방송영상학과 (졸업) · 2004 — 2006

---

## Credentials

- **ISTQB CTFL** — 국제 소프트웨어 테스팅 자격 · 2018
- **PMBOK 6.0 · BABOK 3.0 · Agile/Scrum/Lean/Kanban** (KOSTA) · 2018
- **JLPT 2급 · OPIc 일본어 AL** — 업무 수준 일본어 구사
- **HTA Enterprise JAVA Developer 과정** (중앙일보, 6개월) · 2010
