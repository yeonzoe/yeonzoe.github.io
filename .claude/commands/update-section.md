# 포트폴리오 섹션 업데이트

`index.html`의 특정 섹션 내용을 업데이트한다.

## 사용법

```
/update-section [섹션명]
/update-section skills
/update-section experience
/update-section projects
```

---

## 섹션별 처리 방식

### `skills` — 기술 스택 배지

- `#skills` 섹션의 `.skill-group` 카드 단위로 수정
- 배지 추가: `<span class="badge">새 스킬</span>` 형식
- 강조 배지: `<span class="badge gold">중요 스킬</span>`
- 그룹 추가 시 기존 5개 그룹 구조(Test / Automation / AI·Tools / Infra·CI / Language) 유지

### `experience` — 경력

- `#experience` 섹션의 `.exp-item` 단위로 수정
- 새 항목은 `.exp-list` 맨 위에 추가 (최신순)
- 기간, 회사명, 역할, 기간 라벨, 업무 목록 모두 포함
- 업무 목록은 `<li>` 형식, 강조는 `<strong>` 사용

### `projects` — 프로젝트 카드

- `/add-project` 커맨드 사용 권장
- 직접 수정 시 `.project-card` 단위로 추가/수정

### `hero` — 상단 통계

- `.stat-card` 수치 업데이트 (경력 년수, TC 수 등)

### `certs` — 자격 & 수상

- `.cert-card` 단위로 추가/수정

---

## 실행 절차

1. `$ARGUMENTS`로 섹션 파악
2. `index.html` 읽기
3. 해당 섹션 위치 파악
4. 사용자에게 어떤 내용을 추가/수정할지 확인 (불명확한 경우)
5. 수정 적용
6. 수정 내용 요약 출력
7. `/commit` 실행 안내

---

## 주의사항

- CSS 변수, 클래스명 변경하지 않는다
- 외부 라이브러리/CDN 추가하지 않는다
- `index.html` 단일 파일 구조를 유지한다
