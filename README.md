# Git Branch Practice

브랜치 생성, 전환, 커밋, 병합을 연습하기 위한 간단한 웹 페이지입니다.

## 파일 구조

git-branch-practice
├─ index.html
├─ css
│  └─ style.css
└─ js
   └─ script.js

## 추천 브랜치 연습

### 1. 저장소 시작

```bash
git init
git add .
git commit -m "프로젝트 기본 구조 완성"
```

### 2. header 브랜치 만들기

```bash
git switch -c feature/header
```

index.html의 header 영역을 수정합니다.

```bash
git add .
git commit -m "header 메뉴 수정"
```

### 3. main으로 돌아오기

```bash
git switch main
```

### 4. content 브랜치 만들기

```bash
git switch -c feature/content
```

hero 또는 card 영역을 수정합니다.

```bash
git add .
git commit -m "content 영역 수정"
```

### 5. main에 병합하기

```bash
git switch main
git merge feature/header
git merge feature/content
```

## GitHub에 올리기

```bash
git remote add origin 저장소주소
git branch -M main
git push -u origin main
```

## GitHub Pages 배포

GitHub 저장소의 Settings → Pages → Branch에서 main / root를 선택합니다.
