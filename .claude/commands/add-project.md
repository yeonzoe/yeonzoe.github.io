# 프로젝트 카드 추가

포트폴리오의 `#projects` 섹션에 새 프로젝트 카드를 추가한다.

## 사용법

```
/add-project [프로젝트명]
/add-project QA 모니터링 자동화
```

---

## 실행 절차

### Step 1: 정보 수집

`$ARGUMENTS`에서 프로젝트명 추출. 아래 정보를 사용자에게 확인:

1. **프로젝트명** (한글 2줄 권장, 예: `969 TC\n자동화 시스템`)
2. **아이콘** (이모지 1개, 예: ⚙️ 🤖 📊 🔍 🛡️)
3. **설명** (2~3문장, 한국어)
4. **태그** (기술 스택, 최대 6개)

### Step 2: 카드 생성

아래 템플릿으로 카드 HTML 생성:

```html
<div class="project-card fade-up">
  <div class="project-icon">{아이콘}</div>
  <div class="project-title">{프로젝트명 라인1}<br>{프로젝트명 라인2}</div>
  <div class="project-desc">
    {설명 2~3문장}
  </div>
  <div class="project-tags">
    <span class="project-tag">{태그1}</span>
    <span class="project-tag">{태그2}</span>
  </div>
</div>
```

### Step 3: 삽입 위치

`.projects-grid` 내부 마지막 카드 뒤에 추가.
카드가 4개 이상이 되면 그리드를 `repeat(2, 1fr)` 로 변경 고려.

### Step 4: 완료 안내

추가된 카드 내용 요약 후 `/commit` 실행 안내.
