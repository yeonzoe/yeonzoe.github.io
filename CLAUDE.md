# 연향주 — 포트폴리오 & 이력서 프로젝트

## 프로젝트 개요

연향주(yeonzoe)의 개인 포트폴리오 사이트 및 이력서 관리 레포.
GitHub Pages (`https://yeonzoe.github.io/resume/`)로 배포.

---

## 파일 구조

```
resume/
├── index.html                  # 포트폴리오 메인 페이지 (GitHub Pages)
├── resume/
│   └── 연향주_이력서.pdf        # 다운로드용 이력서
├── CLAUDE.md                   # 이 파일
└── .claude/
    ├── settings.json           # 플러그인 / 훅 설정
    ├── commands/               # 슬래시 커맨드
    └── handoffs/               # 세션 인계 문서
```

---

## 핵심 작업 흐름

```
이력서 업데이트 → index.html 수정 → /commit → git push → GitHub Pages 자동 배포
새 프로젝트 추가 → /add-project → /commit
섹션 수정 → /update-section [섹션명] → /commit
```

---

## 슬래시 커맨드

| 커맨드 | 설명 |
|--------|------|
| `/commit` | Conventional Commit 형식 커밋 (plugin 제공) |
| `/update-section` | 포트폴리오 특정 섹션 업데이트 |
| `/add-project` | 프로젝트 카드 추가 |
| `/deploy` | push + GitHub Pages 배포 안내 |
| `/handoff` | 세션 종료 전 작업 인계 문서 생성 |

---

## 포트폴리오 구성 섹션

| 섹션 ID | 내용 |
|---------|------|
| `#hero` | 이름, 직함, 연락처, 핵심 수치 |
| `#about` | 한 줄 소개 |
| `#skills` | 기술 스택 배지 (5개 그룹) |
| `#experience` | 경력 타임라인 (5개 회사) |
| `#projects` | 주요 프로젝트 카드 3개 |
| `#certs` | 자격증 & 수상 |

---

## 디자인 원칙

- **디자인 시스템**: CSS 변수 기반 (`--bg`, `--accent`, `--card` 등)
- **다크 테마**: `--bg: #08090C` 기준
- **강조색**: `--accent: #3ECFBE` (teal) / `--gold: #C9A84C`
- **폰트**: Bodoni Moda (display) + Sora (body) + JetBrains Mono (code/badge)
- **외부 프레임워크 없음**: Google Fonts만 허용

수정 시 위 시스템을 유지한다. 새 색상이나 폰트를 추가하지 않는다.

---

## 개인 정보 (커밋/배포에 포함 가능)

- 이름: 연향주
- 이메일: hjyeon@naver.com
- GitHub: github.com/yeonzoe
- 배포 URL: https://yeonzoe.github.io/resume/

---

## Git 설정

- **계정**: yeonzoe (개인)
- **remote**: `git@github-yeonzoe:yeonzoe/resume.git`
- **브랜치**: main 직접 push (단일 파일 사이트, PR 불필요)
- **커밋 형식**: Conventional Commits (`feat`, `fix`, `docs`, `chore`)
