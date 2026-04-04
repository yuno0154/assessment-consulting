# 2026 평가계획서 서면 컨설팅 시스템

중등 학생평가 종합 점검단 운영 도구

---

## 파일 구조

```
evaluation-consulting/
├── index.html       ← 검토자용 웹앱 (160명 사용)
├── admin.html       ← 관리자 전용 (로컬 보관, GitHub 업로드 금지)
├── library.json     ← 표준 라이브러리 데이터
└── README.md        ← 사용 안내
```

---

## 검토자 사용법 (index.html)

1. GitHub Pages 링크 접속
2. 기본 정보 입력 (학교급 / 학교명 / 과목명 / 수행평가 개수)
3. 항목 1, 1-1 판정 (과목 단위)
4. 수행평가별 항목 2, 3+4+7+6, 8, 5 판정
5. 컨설팅 의견 생성 → 워드 또는 TXT 다운로드
6. 학교별 게시판에 업로드

---

## 관리자 사용법 (admin.html)

> ⚠️ admin.html은 GitHub에 업로드하지 마세요. 로컬에만 보관하세요.

1. admin.html을 브라우저로 열기
2. GitHub 사용자명, Repository명, Personal Access Token 입력
3. 라이브러리 불러오기
4. 검토자 제안 문장 승인 / 수정 후 승인 / 반려
5. 새 표준 문장 직접 추가
6. 저장 시 GitHub library.json 자동 업데이트

---

## GitHub Pages 설정

1. Repository → Settings → Pages
2. Source: Deploy from a branch
3. Branch: main / (root)
4. Save → 링크 생성 확인

---

## Personal Access Token 생성

1. GitHub → Settings → Developer Settings
2. Personal Access Tokens → Tokens (classic)
3. Generate new token → repo 체크
4. 유효 기간: 1학기 종료 후 만료 설정 권장
5. 생성된 토큰은 admin.html에만 입력

---

## 점검 항목

| 항목 | 내용 | 단위 | 판정 수준 |
|------|------|------|---------|
| 1 | 성취기준 일치 | 과목 | 적절 / 보완 요청 |
| 1-1 | 누락 성취기준 (고교) | 과목 | 자동 |
| 2 | 수행평가명 적절성 | 수행평가 | 적절 / 보완 권고 / 보완 요청 |
| 3+4+7+6 ★ | 정합성 | 수행평가 | 적절 / 보완 권고 / 보완 요청 |
| 8 | 암기형·과제형·AI | 수행평가 | 적절 / 보완 요청 |
| 5 | 미응시 기본점수 | 수행평가 | 적절 / 보완 요청 |

---

## 문의

중등 학생평가 종합 점검단 운영팀
