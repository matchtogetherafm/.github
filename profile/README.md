# 매치투게더AFM

> 축구를 사랑하는 모든 분들을 위한 원스톱 플랫폼 — 소셜매치 · 용품 쇼핑 · 커뮤니티

---

## 1. 프로젝트 개요

| 항목 | 내용 |
|------|------|
| 프로젝트명 | 매치투게더AFM |
| 개발 기간 | 2025.01 ~ |
| 플랫폼 | Web (반응형) |
| 배포 | - |

## 2. 프로젝트 소개

**매치투게더AFM**은 11vs11 축구 소셜매치 매칭, 공식 용품 쇼핑, 커뮤니티를 하나로 합친 축구 라이프 플랫폼입니다.

회원가입 후 간단한 설문을 통해 선수 티어를 부여받고, 포지션을 선택하여 경기에 참가할 수 있습니다. 경기 외에도 AFM 공식 유니폼·트레이닝 용품을 구매하고, 커뮤니티에서 경기 후기와 용품 리뷰를 공유할 수 있습니다.

## 3. 프로젝트 목표

- 누구나 쉽게 11vs11 축구 경기를 찾고 참가할 수 있는 매칭 시스템 구축
- 설문 기반 티어 시스템으로 실력에 맞는 균형 잡힌 팀 구성
- 축구 경기 매칭부터 용품 구매, 커뮤니티까지 하나의 플랫폼에서 해결
- 직관적인 포지션 선택 UI로 누구나 쉽게 이용 가능한 UX 제공

## 4. 주요 기능

### AFM 소셜매치
- 4-3-3 포메이션 기반 11vs11 경기 매칭
- 2시간 매치 = 1경기(전반 1시간) + 2경기(후반 1시간)
- Black Team vs White Team 팀 구성
- 포지션별 참가 신청 및 결제

### 선수 티어 시스템
- 설문 기반 8단계 티어 자동 산정 (전설 → 뉴비)
- 공식 리그 경력 · 축구 구력 · 현재 활동 상태 반영
- 관리자 수동 티어 조정 기능

### AFM 오피셜 스토어
- 공식 유니폼, 트레이닝 용품 쇼핑몰
- 장바구니 · 주문 · 배송 관리
- 카테고리: 상의, 하의, 플레이킷, 세트, 팀 패키지

### 커뮤니티
- 경기 후기, 용품 리뷰, 자유 게시판
- 댓글 · 좋아요 기능

### 기타
- JWT 기반 인증 (Access Token + Refresh Token)
- 마이페이지 (프로필, 주문내역, 위시리스트, 내 글, 내 경기)
- 고객지원 (FAQ, 공지사항, 1:1 문의)

## 5. 팀원 소개

| 이름 | 역할 |
|------|------|
| 최태웅 | Frontend |
| 남경은 | Backend |
| | |
| | |

## 6. 기술 스택

### Frontend

| 구분 | 기술 |
|------|------|
| Framework | Next.js 14 (App Router) |
| Language | TypeScript |
| Styling | Tailwind CSS |
| UI Components | shadcn/ui (Radix UI) |
| Form / Validation | React Hook Form, Zod |
| HTTP Client | Axios |
| Icons | Lucide React |
| Carousel | Embla Carousel |

### Backend

| 구분 | 기술 |
|------|------|
| Framework | |
| Language | |
| Database | |
| ORM | |
| Authentication | JWT (Access + Refresh Token) |
| Deployment | |

## 7. 문서 자료

| 문서 | 링크 |
|------|------|
| 프로젝트 계획서 | [작성 예정]() |
| ERD | [작성 예정]() |
| 시스템 아키텍처 다이어그램 | [작성 예정]() |
| API 명세서 | [작성 예정]() |
| 화면 설계서 (Figma) | [작성 예정]() |

## 8. 실행 가이드

### 사전 요구사항

- Node.js 18 이상
- npm

### 설치 및 실행

```bash
# 저장소 클론
git clone https://github.com/matchtogetherafm/afm.git
cd afm

# 의존성 설치
npm install

# 환경 변수 설정
cp .env.local.example .env.local

# 개발 서버 실행
npm run dev
http://localhost:3000에서 확인할 수 있습니다.

빌드

npm run build
npm run start
환경 변수

NEXT_PUBLIC_API_BASE_URL=http://localhost:8080

