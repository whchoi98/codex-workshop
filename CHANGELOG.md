# Changelog

[![English](https://img.shields.io/badge/lang-English-blue.svg)](#english)
[![Korean](https://img.shields.io/badge/lang-%ED%95%9C%EA%B5%AD%EC%96%B4-red.svg)](#한국어)

---

# English

All notable changes to this project will be documented in this file.
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.0.0] - 2026-06-15

### Added

- Publish the initial Codex Deep Dive Workshop release as a PDF distribution of the two-day, 235-slide, twelve-module OpenAI Codex curriculum — "one agent for everywhere you code: CLI, IDE, App, and Web."
- Distribute the architecture deep-dive (45 slides) as `00_Codex-Architecture.pdf`, covering the Gather-Act-Verify agentic loop, the 8-layer architecture, models and built-in tools (GPT-5.x), sandbox modes and approval policies, context-window auto-compaction, and Skills/Subagents/Hooks/MCP integration.
- Distribute Module 1, Introduction & Core Concepts (23 slides), as `01_Codex_소개와_핵심개념.pdf`, covering the agent loop, autocomplete vs. coding agent, the five surfaces (CLI, IDE, App, Web, SDK), model selection and reasoning effort (GPT-5.5 lineup), and sandboxing/approval modes.
- Distribute Module 2, CLI Deep Dive (22 slides), as `02_CLI_Deep_Dive.pdf`, covering the interactive TUI vs. non-interactive `exec`, slash commands, `@file` references, Steer Mode, session resume, and MCP tool extension.
- Distribute Module 3, App & IDE (19 slides), as `03_App과_IDE.pdf`, covering the desktop App three-pane layout, the review panel with line-level partial approval, threads and git worktrees, automations / local environments / in-app browser / computer use, and the IDE extension.
- Distribute Module 4, Codex on Web (14 slides), as `04_Codex_on_Web.pdf`, covering asynchronous cloud delegation, the local vs. cloud execution model, reproducible cloud environments, internet-access control, and the GitHub PR workflow.
- Distribute Module 5, Lab A — First Agent Task (16 slides), as `05_Lab_A_첫_에이전트_작업.pdf`, a full-cycle hands-on lab: install and login, read-only repo exploration, reproducing and fixing a seeded bug test-first, approval and rollback drills, running tests/lint and opening a PR, and authoring an `AGENTS.md` project guide.
- Distribute Module 6, Configuration & Customization (22 slides), as `06_설정과_커스터마이징.pdf`, covering the six-layer config precedence, `config.toml` and profiles, approval/sandbox modes, the shell environment policy, `AGENTS.md`, and MCP server setup with prompt-injection defense.
- Distribute Module 7, Plugins, Skills, Subagents (14 slides), as `07_Plugins_Skills_Subagents.pdf`, covering plugins as a packaging unit, skills via `SKILL.md` and progressive disclosure, subagents for delegated context, choosing the right extension mechanism, and the `plugin-creator` scaffold.
- Distribute Module 8, Integrations & Security (15 slides), as `08_Integrations_Security.pdf`, covering GitHub/Slack/Linear integrations, the coding-agent threat model, prompt-injection defense, multi-layered security (sandboxing, permissions, review, audit), and least-privilege adoption.
- Distribute Module 9, Automation & SDK (15 slides), as `09_Automation_SDK.pdf`, covering non-interactive `codex exec` scripting, the Codex SDK, App Server mode, the GitHub Action, building MCP servers, and the trigger-execute-verify-deliver reference architecture.
- Distribute Module 10, Lab B — Automation Pipeline (15 slides), as `10_Lab_B_자동화_파이프라인.pdf`, a hands-on lab that builds an issue-to-PR pipeline: local `codex exec` validation, a labeled-issue GitHub Actions workflow, Secrets injection, test/lint verification gates, auto-generated PR with Slack notification, and a guardrail safety check.
- Distribute Module 11, Enterprise & Admin (15 slides), as `11_Enterprise_Admin.pdf`, covering SSO and scoped access tokens, org-level approval/sandbox policies, Amazon Bedrock deployment within the AWS data boundary (IAM/VPC/CloudTrail), governance, managed configuration, and enterprise admin rollout.
- Include two end-to-end hands-on labs (Lab A, Lab B) and nine timed mini-labs embedded across the lecture modules.
- Add a bilingual (English/Korean) `README.md` documenting the curriculum, prerequisites, install steps, recommended teaching order, and project structure.
- Add this bilingual `CHANGELOG.md`.
- Apply a consistent 16:9 design system with a bilingual layout (Korean body, English headings) across all twelve module PDFs.

[Unreleased]: https://github.com/whchoi98/codex-workshop/compare/v1.0.0...HEAD
[1.0.0]: https://github.com/whchoi98/codex-workshop/releases/tag/v1.0.0

---

# 한국어

이 프로젝트의 모든 주요 변경 사항은 이 파일에 기록됩니다.
이 문서는 [Keep a Changelog](https://keepachangelog.com/en/1.1.0/)를 기반으로 하며, [Semantic Versioning](https://semver.org/spec/v2.0.0.html)을 따릅니다.

## [Unreleased]

## [1.0.0] - 2026-06-15

### Added

- 2일 235 슬라이드, 12개 모듈 분량의 OpenAI Codex Deep Dive Workshop 커리큘럼을 PDF 배포 형태로 최초 공개 — "코드를 작성하는 모든 곳을 위한 하나의 에이전트: CLI, IDE, App, Web."
- 아키텍처 심화(45 슬라이드)를 `00_Codex-Architecture.pdf` 로 배포 — Gather-Act-Verify 에이전틱 루프, 8개 레이어 아키텍처, 모델과 내장 도구(GPT-5.x), 샌드박스 모드와 승인 정책, 컨텍스트 윈도우 자동 컴팩션, Skills/Subagents/Hooks/MCP 통합 포함.
- 모듈 1 소개와 핵심 개념(23 슬라이드)을 `01_Codex_소개와_핵심개념.pdf` 로 배포 — 에이전트 루프, 자동완성 vs 코딩 에이전트, 5가지 사용 환경(CLI, IDE, App, Web, SDK), 모델 선택과 추론 강도(GPT-5.5 라인업), 샌드박스·승인 모드 포함.
- 모듈 2 CLI Deep Dive(22 슬라이드)를 `02_CLI_Deep_Dive.pdf` 로 배포 — 대화형 TUI vs 비대화형 `exec`, slash 명령, `@파일` 참조, Steer Mode, 세션 재개, MCP 도구 확장 포함.
- 모듈 3 App과 IDE(19 슬라이드)를 `03_App과_IDE.pdf` 로 배포 — 데스크톱 App 3-pane 레이아웃, 라인 단위 부분 승인이 가능한 리뷰 패널, 스레드와 git worktree, automations / local environments / 내장 브라우저 / computer use, IDE 확장 포함.
- 모듈 4 Codex on Web(14 슬라이드)을 `04_Codex_on_Web.pdf` 로 배포 — 비동기 클라우드 위임, 로컬 vs 클라우드 실행 모델, 재현 가능한 클라우드 환경, 인터넷 접근 제어, GitHub PR 워크플로우 포함.
- 모듈 5 Lab A — 첫 에이전트 작업(16 슬라이드)을 `05_Lab_A_첫_에이전트_작업.pdf` 로 배포 — 풀 사이클 실습 랩: 설치·로그인, 읽기 전용 레포 탐색, 실패 테스트 우선 버그 재현·수정, 승인·롤백 드릴, 테스트/린트 실행과 PR 생성, `AGENTS.md` 지침서 작성.
- 모듈 6 설정과 커스터마이징(22 슬라이드)을 `06_설정과_커스터마이징.pdf` 로 배포 — 6계층 설정 우선순위, `config.toml`과 프로파일, 승인·샌드박스 모드, 셸 환경 정책, `AGENTS.md`, MCP 서버 설정과 프롬프트 인젝션 방어 포함.
- 모듈 7 Plugins, Skills, Subagents(14 슬라이드)를 `07_Plugins_Skills_Subagents.pdf` 로 배포 — 배포 단위로서의 플러그인, `SKILL.md`와 progressive disclosure 기반 스킬, 위임용 서브에이전트, 확장 메커니즘 선택 기준, `plugin-creator` 스캐폴드 포함.
- 모듈 8 Integrations와 Security(15 슬라이드)를 `08_Integrations_Security.pdf` 로 배포 — GitHub/Slack/Linear 연동, 코딩 에이전트 위협 모델, 프롬프트 인젝션 방어, 다층 보안(샌드박싱·권한·검토·감사), 최소 권한 도입 포함.
- 모듈 9 Automation과 SDK(15 슬라이드)를 `09_Automation_SDK.pdf` 로 배포 — 비대화형 `codex exec` 스크립팅, Codex SDK, App Server 모드, GitHub Action, MCP 서버 구축, 트리거-실행-검증-전달 레퍼런스 아키텍처 포함.
- 모듈 10 Lab B — 자동화 파이프라인(15 슬라이드)을 `10_Lab_B_자동화_파이프라인.pdf` 로 배포 — 이슈-투-PR 파이프라인을 구축하는 실습 랩: 로컬 `codex exec` 검증, 라벨 트리거 GitHub Actions 워크플로우, Secrets 주입, 테스트/린트 검증 게이트, Slack 알림 포함 PR 자동 생성, 가드레일 안전장치 점검.
- 모듈 11 Enterprise와 Admin(15 슬라이드)을 `11_Enterprise_Admin.pdf` 로 배포 — SSO와 범위 기반 액세스 토큰, 조직 단위 승인·샌드박스 정책, AWS 데이터 경계 내 Amazon Bedrock 배포(IAM/VPC/CloudTrail), 거버넌스, 중앙 관리 설정, 엔터프라이즈 관리자 롤아웃 포함.
- 2개의 End-to-End 실습 랩(Lab A, Lab B)과 강의 모듈 전반에 포함된 9개의 시간제 미니 랩 제공.
- 커리큘럼, 사전 요구 사항, 설치 절차, 권장 교육 순서, 프로젝트 구조를 다루는 이중 언어(영어/한국어) `README.md` 추가.
- 이중 언어 `CHANGELOG.md` 추가.
- 12개 모듈 PDF 전체에 16:9 비율과 이중 언어 레이아웃(한국어 본문, 영어 제목)으로 구성된 일관된 디자인 시스템 적용.

[Unreleased]: https://github.com/whchoi98/codex-workshop/compare/v1.0.0...HEAD
[1.0.0]: https://github.com/whchoi98/codex-workshop/releases/tag/v1.0.0
