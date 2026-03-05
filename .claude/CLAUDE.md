# mahjong-kb 프로젝트 지시사항

## 프로젝트 개요
리치마작(일본식 마작) 종합 백과사전 Markdown 기반 지식 베이스.
Obsidian 볼트 호환 + 향후 Python RAG 파이프라인 연동.

## 콘텐츠 규칙

### 용어 표기 통일
- 쯔모 (O) / 츠모 (X)
- 리치 (O) / 리이치 (X)
- 탕야오 (O) / 단요구 (X)
- 일본어 원어 + 한국어 + 로마자 3개 항상 병기
- aliases에 대안 표기 포함

### 파일 네이밍
- 역(야쿠)/용어: 로마자 (`tanyao.md`, `riichi.md`)
- 규칙/전략/일반: 한글 (`리치.md`, `방어전략.md`)

### Frontmatter 공통 필드
```yaml
title, category, subcategory, difficulty, tags, aliases, date_created, date_modified, status
```

### 역(야쿠) 전용 추가 필드
```yaml
han, naki, kuisagari, japanese, romaji, korean
```

### difficulty 값
- beginner / intermediate / advanced / expert

### status 값
- draft / review / published

## 디렉토리 구조
- `content/` — 모든 콘텐츠
- `content/_templates/` — Obsidian 템플릿 5종
- `src/` — Python RAG 파이프라인 (Phase 3+)

## 내부 링크
- Obsidian 위키링크 형식 사용: `[[파일명]]` 또는 `[[파일명|표시텍스트]]`
- 관련 문서 섹션에서 태그와 링크 활용
