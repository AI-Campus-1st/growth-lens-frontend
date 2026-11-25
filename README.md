# growth-lens-frontend (Public)

GrowthLens 화면 — 홈 대시보드, Market Opportunity, Marketing Timing, Promotion Intelligence, Revenue Analysis, AI Assistant, Monthly Seller Action Report

> 기획·설계는 메인 레포 [growth-lens](https://github.com/AI-Campus-1st/growth-lens)에서 관리합니다.
> **현재 상태: 디렉터리 구조만 있음. 프레임워크 미정(Streamlit 미사용), 화면 미구현.**

담당: 김한승 (모듈 화면 분담 방식은 미정)

## 구조
```text
src/pages/        # 화면
src/components/   # 공통·모듈별 컴포넌트
src/assets/       # 정적 리소스
```
프레임워크 확정 시 해당 관례에 맞게 조정합니다.

## 원칙
- **Public 레포**: API 키, 데이터, 내부 분석 원본을 넣지 않습니다. 데이터는 growth-lens-backend API로만 받습니다.
- 모든 결과 화면에 데이터 출처·시장(국가)·관측 기간·결과 유형(관측/추정/시뮬레이션)·한계를 표시합니다.
- 해외 데이터(M02·M04) 결과는 국내 판매자 데이터처럼 보이지 않도록 별도 라벨을 붙입니다.
- 브랜치·커밋: [CONTRIBUTING.md](https://github.com/AI-Campus-1st/growth-lens/blob/main/CONTRIBUTING.md) — `feature/platform-*`

## 보안 (클론 직후 1회)
```bash
git config core.hooksPath .githooks   # 비밀값·대용량 파일 커밋 차단 훅
cp .env.example .env                  # 실제 키는 .env 에만
```
규칙·유출 시 대응: [CONTRIBUTING.md §5](https://github.com/AI-Campus-1st/growth-lens/blob/main/CONTRIBUTING.md)
