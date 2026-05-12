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
- 지원 금액: 20,000,000 × 0.85 = **17,000,000원** (VAT 별도, 10만원 단위 반올림 — 기본 90% 규칙 대신 사용자 지시로 85% 적용)
- 지원 기간: **120일** (공고 명시 "3~4개월" 상한, 완성도 1순위 반영)

## 4. 포트폴리오 매칭

매칭 추천 조합: "SaaS B2B" 패턴(EZ-Approve / Harmony Link / Series-B).

| 순위 | 프로젝트 | 매칭 점수 | 핵심 근거 |
|-----|---------|----------|-----------|
| 1 | **EZ-Approve** | 매우 높음 | B2B SaaS, 50+ 페이지 어드민, 7 역할 + 6계층 보안(RBAC), 감사 로그, MUI v5, 워크플로우 추적 — 본 프로젝트의 권한 분리·감사 로그·대시보드 완성도 요건과 정합 |
| 2 | **Harmony Link** | 매우 높음 | **멀티테넌트 아키텍처**, OpenAI 기반 외부 AI 분석 연동, AWS CDK 인프라 직접 운영, 다국어 UI — 본 프로젝트의 멀티테넌시 + AI 엔진(Docker) 연동 + AWS 인프라 요건과 정합 |
| 3 | **Series-B** | 높음 | PR 1,652건 규모 B2B 어드민, 200~300+ API 엔드포인트, ChatGPT 기반 AI 보고서 자동 생성, 5계층 보안 — 본 프로젝트의 상용 안정성 + AI 호출 + 자동 리포트 요건과 정합 |

## 5. 최종 제안 요약

- **지원 금액**: 17,000,000원 (VAT 별도)
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

## 6. 최종 산출물

### 6.1 제안서 사이트 URL

https://proposal-router.claude-ai-b27.workers.dev/proposal-ai-copyright-saas-dashboard/

### 6.2 지원 금액 (복사용)

```
17,000,000원
```

### 6.3 지원 기간 (복사용)

```
120일
```

### 6.4 클라이언트 질문 답변

해당 없음 (공고에 명시된 클라이언트 질문 없음).

### 6.5 지원 내용 (전체 텍스트, 복사용)

```
안녕하세요, AI 기반 저작권 보호 B2B SaaS 대시보드 및 미들웨어 통합 개발 프로젝트에 지원합니다.

본 프로젝트에 대한 상세 제안서(견적서, 공수계산서, PRD, 일정, 포트폴리오)를 별도 페이지로 준비하였습니다. 아래 링크에서 확인해 주시면 감사하겠습니다.
▶ 제안서 상세 페이지: https://proposal-router.claude-ai-b27.workers.dev/proposal-ai-copyright-saas-dashboard/
▶ 위시켓 포트폴리오: https://www.wishket.com/partners/p/blueverse1/

---

<프로젝트 진행 제안>

■ 프로젝트 분석
- 자체 개발 완료된 저작권 보호 AI 백엔드 엔진(Docker)과 연동되는 멀티테넌트 B2B SaaS 대시보드, 인증·권한·감사 로그를 처리하는 미들웨어, AWS 인프라·CI/CD를 턴키로 구축
- 핵심 요구사항: 관리자·운영자·조회자 권한 분리, 멀티테넌시, 콘텐츠 관리, 실시간 침해 탐지 피드, 증거 패키지, Notice & Takedown 추적, 이메일·SMS·인앱 알림, 차트 분석·월간 리포트, KR/EN 다국어
- 1순위(산출물 완성도)에 맞춘 단계별 검수(M1~M4) 기반 운영
- 제안 기술 스택: Next.js 14 + TypeScript + MUI v5 + Recharts + next-intl / NestJS 10 + TypeORM + CASL / PostgreSQL(RDS) + Redis / AWS EC2 또는 ECS Fargate + S3 + CloudFront + ACM + Route53 + SES/SNS / Docker + GitHub Actions
- 선정 이유: 풀스택 TypeScript 단일 언어로 장기 유지보수 효율 / MUI v5는 우대 사항 명시 + 디자인 공수 절감 / NestJS는 RBAC·감사 로그·멀티테넌시 미들웨어에 적합 / PostgreSQL은 RLS로 행 단위 멀티테넌시 보안 가능 / ECS Fargate로 클라이언트 Docker 엔진과 컨테이너 레벨 통합 자연스러움

■ 작업 일정 (총 120일, 4개월)

[Phase 1] Day 1–30 (4주)
- 요구사항 정의서, IA, 화면 기획서, DB 설계, 시스템 아키텍처, Figma UI/UX 디자인(권한별 + KR/EN)
- AWS 인프라 1차 셋업, 클라이언트 제공 AI 엔진 Docker 이미지 통합 테스트
- OpenAPI 기반 미들웨어 IF 설계

[Phase 2] Day 31–60 (4주)
- JWT + CASL 기반 인증·RBAC, 멀티테넌시 데이터 격리, 감사 로그 인프라
- 콘텐츠 업로드(S3 멀티파트)·라이브러리·보호 정책 설정 화면
- AI 엔진 API 호출 중계 1차(재시도/실패 큐 포함)

[Phase 3] Day 61–90 (4주)
- 실시간 침해 탐지 피드(WebSocket), 증거 패키지 조회·다운로드
- Notice & Takedown 요청 추적 워크플로우(제출 상태 + 후속 조치)
- 이메일(SES)·SMS(SNS)·인앱 알림 통합, 차트 분석 화면(Recharts), 월간 리포트 PDF

[Phase 4] Day 91–120 (4주)
- KR/EN 다국어 마무리, 통합/회귀 테스트, 보안 점검
- 관리자/사용자 매뉴얼, 운영 가이드
- 프로덕션 배포, 안정화 및 1차 무상 하자 보수 진입

■ 마일스톤 및 산출물
- M1 (Day 30): 요구사항 정의서·화면 기획서·ERD·아키텍처도·Figma 디자인 시안·AWS 1차 환경·AI 엔진 통합 테스트
- M2 (Day 60): 인증·RBAC·멀티테넌시·콘텐츠 관리·AI 엔진 중계 1차 데모 환경
- M3 (Day 90): 탐지 피드·증거 패키지·Takedown 추적·알림·차트·월간 리포트 통합 데모
- M4 (Day 120): 다국어·통합 테스트 리포트·매뉴얼·프로덕션 배포·하자 보수 진입

■ 미팅 시 협의 필요 사항
- AI 엔진의 침해 이벤트 전달 방식(Webhook push / Polling) 및 평균 호출량/피크 대응 기준
- 멀티테넌시 격리 수준(스키마 분리 vs 행 분리 + RLS) 및 백업·복구 정책
- Notice & Takedown 워크플로우의 상태 단계 정의 및 외부 법무·플랫폼사 연동 여부
- 영문 UI 적용 범위(전체 vs 핵심 운영 흐름) 및 영문 매뉴얼 범위
- AWS 계정·청구 주체(클라이언트 계정에 직접 배포 vs 임시 위탁 계정)
- 운영 단계의 모니터링/온콜 책임 범위
- 본 공고가 "고도화 의뢰 예정"으로 명시되어 있어, 1차 납품 이후 고도화 범위·시기 사전 논의

---

<유사 프로젝트 진행 경험>

▶ EZ-Approve — 기업용 전자결재 SaaS (2026.01–2026.03, 약 9주)
- 프로젝트 유형: B2B SaaS / 기업용 어드민 / 전자결재
- 핵심 기능: 다단계 전자결재(8종 결재 액션), 7 사용자 역할 + 6계층 보안(CASL/RBAC), VICS 규제 보고, Lexical 리치 에디터(170파일, 26 커스텀 노드), 실시간 공동 편집(Yjs/CRDT), 토큰 기반 외부 셀프서비스 포탈, 50+ 페이지, 120~150 API 엔드포인트
- 유사점: 본 프로젝트의 3단계 권한 분리(관리자·운영자·조회자) + 감사 로그 + 대규모 어드민 화면 운영 패턴과 정합 / MUI v5 기반 대규모 화면 운영 경험 / 워크플로우 상태 추적(결재 ↔ Takedown 추적)
- 기술 스택: NestJS 10, Next.js 13, TypeScript, MySQL 8, Lexical+Yjs, CASL, MUI v5, Docker

▶ Harmony Link — 시니어 주간보호 멀티테넌트 SaaS (2025, 약 6개월)
- 프로젝트 유형: B2B SaaS / 헬스케어 / 멀티테넌트
- 핵심 기능: 멀티테넌트 아키텍처(센터 단위 데이터 격리 + 권한 분리), OpenAI 기반 AI 건강 분석 파이프라인, 알림 채널(이메일·푸시·인앱), AWS CDK 인프라, 한국어·영어 다국어 UI, 133K+ LOC, 140+ 엔드포인트
- 유사점: 본 프로젝트의 "여러 기업이 하나의 플랫폼을 쓰는" 멀티테넌시 요구사항과 동일 패턴 / 외부 AI 엔진 호출·재시도·실패 큐 패턴 운영 경험 / AWS CDK·CI/CD 1인 운영 / KR/EN 다국어 UI 실전
- 기술 스택: NestJS, Next.js, TypeScript, MySQL, AWS CDK, Docker, OpenAI

▶ Series-B — VC 펀드 관리 플랫폼 (2023.11–2024.12, 14개월)
- 프로젝트 유형: 핀테크 / VC 펀드 관리 / 대규모 B2B 어드민
- 핵심 기능: PR 1,652건, 50+ 페이지, 22 도메인 모듈, 80+ 엔티티, 200~300+ API 엔드포인트, ChatGPT 기반 AI 투자 보고서 자동 생성, VICS 규제 5종, NICE KYC, 5계층 보안 + DLP + GeoIP
- 유사점: 본 프로젝트의 상용 안정성·다중 권한·감사 로그 요건과 정합 / ChatGPT 기반 AI 보고서 자동 생성 패턴이 본 프로젝트 AI 엔진 중계 + 월간 리포트 자동 생성과 동일 구조 / AWS 5계층 보안 직접 설계 경험
- 기술 스택: Next.js 13, NestJS 10, TypeScript, MySQL, Lexical+Yjs, AWS, ChatGPT API

---

<사용 기술과 툴>

▶ 개발 기술
- 프론트엔드: Next.js 14 (App Router) + TypeScript + MUI v5 + Recharts + next-intl
- 미들웨어(백엔드): NestJS 10 + TypeORM + class-validator + CASL
- DB / 캐시: PostgreSQL (Amazon RDS) + Redis (ElastiCache)
- 인증: JWT + Refresh Token, RBAC(CASL)
- 실시간: WebSocket(Socket.io)
- 알림: AWS SES(이메일) + AWS SNS(SMS) + 인앱(WebSocket)
- 파일: AWS S3 + CloudFront + Pre-signed URL
- 인프라: AWS EC2 또는 ECS Fargate + RDS + S3 + CloudFront + ACM + Route53 + Secrets Manager
- 컨테이너: Docker (클라이언트 제공 AI 엔진 이미지와 통합)
- CI/CD: GitHub Actions → ECR → ECS 블루/그린 또는 롤링 배포
- 모니터링: CloudWatch + Sentry

▶ 개발 도구 및 인프라
- 버전 관리: GitHub
- CI/CD: GitHub Actions
- 클라우드: AWS
- 컨테이너: Docker

▶ 커뮤니케이션
- 일일 진행 공유: Slack 또는 카카오톡
- 주간 미팅: Zoom / Google Meet
- 문서 공유: Notion 또는 Google Docs
- 이슈 트래킹: GitHub Issues
```

### 6.6 관련 포트폴리오 추천 (위시켓 폼 선택용)

1. **EZ-Approve** — B2B SaaS 어드민·RBAC·감사 로그·워크플로우 추적 패턴이 본 프로젝트와 동일 구조
2. **Harmony Link** — 멀티테넌트 아키텍처 + 외부 AI 엔진 연동 + AWS 인프라 직접 운영 + KR/EN 다국어
3. **Series-B** — 대규모 B2B 어드민·AI 자동 보고서·5계층 보안으로 상용 안정성 입증

