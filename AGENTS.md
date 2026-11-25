# AGENTS.md — growth-lens-frontend

공통 지침은 메인 레포 [AGENTS.md](https://github.com/AI-Campus-1st/growth-lens/blob/main/AGENTS.md)를 따릅니다. 이 레포에서 특히 지킬 것:

1. 한국어로 보고하고, 커밋·푸시·의존성 설치는 승인 후에만 합니다. 프레임워크를 임의로 선정하지 않습니다.
2. **Public 레포** — 비밀값·데이터·내부 결과 원본을 코드나 정적 파일에 넣지 않습니다. 클라이언트 번들에 들어가는 환경변수는 공개된다고 가정합니다.
3. 수치를 화면에서 재계산하지 않고 backend API 응답을 그대로 표시합니다.
4. 결과마다 출처·시장·기간·결과 유형·한계 라벨을 표시합니다.
