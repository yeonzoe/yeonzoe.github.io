# Case Study — 전 계층 테스트 자동화 (0 → 969)

| | |
|---|---|
| **회사 / 도메인** | 직방 (PropTech) |
| **역할** | QA Engineer (직접 설계·구현) |
| **기간** | 2024.07 ~ |

> *회사 내부 식별자·미공개 수치는 제외하고, 접근 방식과 공개 가능한 성과만 기술합니다.*

---

## 배경 (Problem)

3개 서비스를 운영하지만 **체계화된 TC도, 자동화도 전무**한 상태였습니다. 배포마다 수동 회귀에 2~3시간이 걸렸고, 검증 범위는 사람의 기억에 의존했습니다.

## 접근 (Approach)

품질을 "마지막 단계의 수동 확인"에서 **"개발 전 과정에 내재된 자동 검증"** 으로 전환하는 것을 목표로, 3계층 자동화 아키텍처를 0에서 설계했습니다.

1. **3계층 분리** — Web E2E(Playwright/TypeScript) · API(pytest) · App(Maestro). 각 계층의 책임을 명확히 나눠 결함을 계층별로 격리·재현
2. **TC 표준 정의** — ISO 25010 품질특성 + 설계기법을 명시하는 11-컬럼 표준. 블랙박스 5기법(동등분할·경계값·결정테이블·상태전이·유스케이스)을 전수 적용
3. **환경 중앙화** — 환경변수로 Production / Preview / Beta를 분기, **동일 TC를 3환경에서 실행**하고 URL만 전환
4. **안전 가드 내장** — 생성/수정/삭제(CUD) 테스트는 `skipOnProd` 가드로 상용 환경에서 자동 차단

## 방법 디테일 (How)

- **CI 품질 게이트 3단계** — Preview → Beta → Production. 각 단계를 GitHub Actions로 자동 트리거하고, Allure 리포트 자동 배포 + Slack 장애 알림 연동
- **BDD 하네스** — 한글 Gherkin 시나리오를 Orchestrator로 멀티 환경 × 스택 병렬 실행, TC ↔ Feature 자동 변환
- **디버깅 인프라** — 실패 시 자동 스크린샷, API 응답시간 임계치 모니터링, 토큰 자동 갱신, Visual Regression 픽셀 비교

## 결과 (Impact)

- 자동화 **0 → 969건** (Web 272 · API 446 · App 251)
- 배포 검증 **2~3시간 → 약 1분**
- 수동 회귀 **주 22시간 절감**
- 3환경 동일 TC 실행으로 환경별 회귀 누락 제거

## 사용 기술

`Playwright(TS)` `pytest` `Maestro` `Appium` `GitHub Actions` `Allure` `Behave(BDD)` `Newman`

---

← [방법론](../methodology.md) · [다른 사례](./)
