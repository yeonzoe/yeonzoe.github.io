# 배포

변경사항을 push하고 GitHub Pages 배포 상태를 안내한다.

## 사용법

```
/deploy
```

---

## 실행 절차

### Step 1: 미커밋 변경 확인

```bash
git status --short
```

변경이 있으면 → `/commit` 먼저 실행하도록 안내하고 중단.

### Step 2: Push

```bash
git push origin main
```

### Step 3: 배포 안내

push 성공 시 다음 정보 출력:

```
✅ Push 완료

배포 URL: https://yeonzoe.github.io/resume/
반영 시간: 통상 1~3분

GitHub Actions 상태 확인:
https://github.com/yeonzoe/resume/actions

※ 최초 1회: repo Settings → Pages → Source: main / root 설정 필요
```

### Step 4: GitHub Actions 상태 (선택)

`gh run list --repo yeonzoe/resume --limit 3` 로 최근 배포 상태 확인 가능하면 표시.
