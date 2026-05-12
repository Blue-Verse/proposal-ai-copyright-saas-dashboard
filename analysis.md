# AI 기반 저작권 보호 B2B SaaS 대시보드 및 미들웨어 통합 개발 — 제안 분석 로그

> 생성일: 2026-05-12
> 공고 URL: https://www.wishket.com/project/155247/

## 1. 공고 파싱 결과

```yaml
job:
  title: "AI 기반 저작권 보호 B2B SaaS 대시보드 및 미들웨어 통합 개발"
  category: "개발/디자인/기획 > 웹 > 기타 (SaaSㆍ솔루션, 데이터 분석ㆍBI, Gen AI 서비스)"
  budget_range: "20,000,000원"
  duration: "90일"
  applicants: 10
  tech_stack: []   # 파트너 자유 제안
  description: |
    자체 개발 완료된 저작권 보호 AI 백엔드 엔진(API)과 연동하여,
    실제 고객(기업)이 사용할 프론트엔드 운영 대시보드, 인증·권한·회원관리 등을 처리할
    백엔드 미들웨어, 그리고 AWS 기반의 인프라 세팅을 턴키로 맡을 파트너사 모집.
    MVP가 아닌 상용화·운영 가능한 완성도 요구.
  requirements:
    - 권한별 화면 기획 및 UI/UX 디자인
    - 고객 대시보드 + 관리자 웹 프론트엔드
    - 인증·권한·회원관리·DB 설계 및 AI 엔진 API 호출 중계 미들웨어
    - AWS 기반 서버 환경 + CI/CD 파이프라인
    - 회원가입/로그인/비밀번호 재설정
    - 관리자·운영자·조회자 권한 분리
    - 멀티테넌시 (여러 기업이 하나의 플랫폼 공유)
    - 감사 로그
    - 콘텐츠 업로드/라이브러리, 보호 정책 설정
    - 실시간 침해 탐지 피드
    - 증거 패키지 조회·다운로드
    - Notice & Takedown 요청 추적
    - 이메일/SMS/인앱 알림
    - 차트 기반 분석 화면, 월간 리포트
    - 한국어/영어 이중언어
    - 클라이언트 제공 Docker 이미지(AI 엔진) 연동
    - CI/CD, SSL/TLS, 도메인 설정
  client_questions: []
  client_prepared:
    - 백엔드 엔진 API 문서 (국문/영문 Reference, Integration Contract)
    - Swagger/OpenAPI 스펙
    - Docker 이미지
    - 통합 테스트용 샘플 데이터
  priorities:
    - "1순위: 산출물 완성도"
    - "2순위: 금액"
    - "3순위: 일정 준수"
  preferred:
    - "SaaS 대시보드 / B2B 관리자 웹 개발 포트폴리오"
    - "다국어 UI / 멀티테넌시 구축 경험"
    - "상용 UI 프레임워크(MUI 등) 활용 경험"
  deliverables:
    - 기능 정의서 및 화면 기획서
    - 데이터베이스 설계서
    - 시스템 아키텍처 및 인프라 구성도
    - 프론트엔드 및 미들웨어 원본 소스 코드
    - 관리자 및 사용자 매뉴얼
  deadline: "2026-05-26"
  job_post_url: "https://www.wishket.com/project/155247/"
  urls: []
  images: []
```

## 2. URL/이미지 분석

- 참고 URL/이미지 없음 — 본 단계는 건너뜀.

## 3. 실현 가능성 분석 (내부용)

- **프로젝트 유형**: 풀스택 B2B SaaS(CRUD 중심) + 멀티테넌시 + 외부 API(AI 엔진) 연동
- **Feasibility 판정**: "가능" + 인증/외부 연동 측면에서 "조건부 가능" 일부 — 버퍼 +10~15%
- **기본 공수(AI 미적용)**: 약 157 M/D
  - 기획/요구사항/PRD: 12 M/D
  - Figma 디자인(권한별 + KR/EN): 15 M/D
  - 프론트엔드(대시보드·관리자·콘텐츠·탐지·리포트·다국어·RBAC UI): 55 M/D
  - 미들웨어(인증·RBAC·멀티테넌시·감사 로그·AI 엔진 프록시·Notice & Takedown·알림): 45 M/D
  - 인프라(AWS EC2/ECS·RDS·S3·CloudFront·ACM·Route53·Docker 통합·CI/CD): 14 M/D
  - QA/통합/배포/매뉴얼: 16 M/D
- **AI 보조 적용 절감(가중 평균 약 50%)**: 약 72 M/D
- **버퍼 +12.5%**: 약 81 M/D
- **달력 일수(1인 기준, 7/5 환산)**: 81 × 7 / 5 ≈ **114일**
- **클라이언트 예상 기간**: 90일
- **차이**: +24일 (약 27% 초과)
- **공고 명시 범위**: "3~4개월 안에 마무리"
- **판정**: 90일은 산출물 완성도 1순위 + 상용 안정성 요구에 비해 타이트. 공고 명시 상한인 4개월(120일)을 제안하는 것이 안전.

### 최종 결정
- 지원 금액: 20,000,000 × 0.9 = **18,000,000원** (VAT 별도, 10만원 단위 반올림)
- 지원 기간: **120일** (공고 명시 "3~4개월" 상한, 완성도 1순위 반영)

## 4. 포트폴리오 매칭

매칭 추천 조합: "SaaS B2B" 패턴(EZ-Approve / Harmony Link / Series-B).

| 순위 | 프로젝트 | 매칭 점수 | 핵심 근거 |
|-----|---------|----------|-----------|
| 1 | **EZ-Approve** | 매우 높음 | B2B SaaS, 50+ 페이지 어드민, 7 역할 + 6계층 보안(RBAC), 감사 로그, MUI v5, 워크플로우 추적 — 본 프로젝트의 권한 분리·감사 로그·대시보드 완성도 요건과 정합 |
| 2 | **Harmony Link** | 매우 높음 | **멀티테넌트 아키텍처**, OpenAI 기반 외부 AI 분석 연동, AWS CDK 인프라 직접 운영, 다국어 UI — 본 프로젝트의 멀티테넌시 + AI 엔진(Docker) 연동 + AWS 인프라 요건과 정합 |
| 3 | **Series-B** | 높음 | PR 1,652건 규모 B2B 어드민, 200~300+ API 엔드포인트, ChatGPT 기반 AI 보고서 자동 생성, 5계층 보안 — 본 프로젝트의 상용 안정성 + AI 호출 + 자동 리포트 요건과 정합 |

## 5. 최종 제안 요약

- **지원 금액**: 18,000,000원 (VAT 별도)
- **지원 기간**: 120일 (4개월)
- **핵심 제안 포인트**:
  1. 유사 B2B SaaS 대시보드 3건(EZ-Approve, Harmony-Link, Series-B) 1인 풀스택 수행 경험
  2. 멀티테넌시 + RBAC + 감사 로그 패턴 운영 검증
  3. 외부 AI 엔진(Docker/OpenAI/ChatGPT) 연동 미들웨어 설계 경험
  4. MUI v5 우대 사항 충족
  5. KR/EN 다국어 UI 실전 경험
  6. AWS + CI/CD 턴키 인프라 운영 경험
  7. 1순위 완성도 우선 — 4개월(120일) 권장 + 단계별 마일스톤(M1~M4) 검수
- **제안 기술 스택**:
  - FE: Next.js 14 + TypeScript + MUI v5 + Recharts + next-intl
  - BE: NestJS 10 + TypeORM + CASL
  - DB: PostgreSQL(RDS) + Redis(ElastiCache)
  - 인프라: AWS EC2/ECS Fargate + S3 + CloudFront + ACM + Route53 + SES/SNS
  - DevOps: Docker + GitHub Actions
- **선정 이유**:
  - 풀스택 TypeScript 단일 언어 → 장기 유지보수 효율
  - MUI v5 → 우대 사항 명시 + 디자인 공수 절감
  - NestJS의 모듈/가드/인터셉터 구조 → RBAC·감사 로그·멀티테넌시 미들웨어 구현에 자연스러움
  - PostgreSQL RLS → 행 단위 멀티테넌시 보안 가능
  - ECS Fargate → 클라이언트 Docker 엔진과 컨테이너 레벨에서 자연스럽게 통합
