# Codex Deep Dive Workshop

[![License: Proprietary](https://img.shields.io/badge/license-Proprietary-blue.svg)](#license)
[![Build](https://img.shields.io/badge/build-passing-brightgreen.svg)](./)
[![Version](https://img.shields.io/badge/version-1.0.0-green.svg)](./CHANGELOG.md)
[![English](https://img.shields.io/badge/lang-English-blue.svg)](#english)
[![Korean](https://img.shields.io/badge/lang-%ED%95%9C%EA%B5%AD%EC%96%B4-red.svg)](#한국어)

A 2-day OpenAI Codex curriculum delivered as twelve rendered PDF modules covering 235 slides, two hands-on labs, and nine embedded mini-labs.
12개 모듈 PDF와 235 슬라이드, 2개의 종합 실습 랩과 9개의 미니 랩으로 제공되는 2일간의 OpenAI Codex 커리큘럼입니다.

---

# English

## Overview

Codex Deep Dive Workshop is a Korean-language technical curriculum for OpenAI Codex. Its theme is simple: "one agent for everywhere you code — CLI, IDE, App, and Web."

The material ships as ready-to-present PDF slide decks. It walks a team step by step, from the first install all the way to an autonomous issue-to-PR pipeline that runs without human intervention.

The repository root holds **twelve module PDFs** totaling **235 slides**. They are made up of one architecture deep-dive (`00_Codex-Architecture.pdf`) plus eleven sequential modules.

Two of those modules — Lab A and Lab B — are full hands-on labs, and most lecture modules close with a timed mini-lab.

Every deck follows a consistent design system and a bilingual layout (Korean body, English headings) for a uniform visual identity.

## Features

- **Twelve rendered PDF modules** — 235 slides total: an architecture deep-dive plus Intro & Core Concepts, CLI, App & IDE, Codex on Web, Configuration, Plugins/Skills/Subagents, Integrations & Security, Automation & SDK, Enterprise & Admin, and two labs. All PDFs ship at the project root for direct access.
- **Layered architecture deep-dive** — `00_Codex-Architecture.pdf` (45 slides) walks the full agent stack: the agentic loop, Input, Knowledge, Execution & Multi-Agent, Observability, and Integration layers, plus when to reach for Skills vs. Subagents vs. MCP vs. Hooks.
- **Two end-to-end hands-on labs** — Lab A drives the full cycle from install and login through bug fix, regression, and PR creation; Lab B builds an autonomous issue-to-PR automation pipeline with secrets, triggers, validation gates, and guardrails.
- **Nine timed mini-labs** — Lecture modules close with a 10–20 minute mini-lab so learners apply each concept immediately.
- **Covers every Codex surface** — CLI, IDE extension, desktop App, Codex on Web (cloud), and the Automation/SDK + GitHub Action path are each given a dedicated module.
- **Enterprise & security throughout** — Sandboxing, approval modes, prompt-injection defense, threat modeling, authentication, governance, managed configuration, and Amazon Bedrock deployment.
- **Self-contained — no build step required** — PDFs ship pre-rendered; consumers only need a PDF viewer.

## Prerequisites

- A PDF viewer to read the module decks at the project root.
- The Codex CLI installed to follow the mini-labs and Lab A / Lab B (see Module 1, "Quickstart — 설치").
- A GitHub account and repository for the integration and automation labs (Lab B, Module 8, Module 9).
- `git` to clone this repository.

## Installation

```bash
# 1. Clone the repository
git clone https://github.com/whchoi98/codex-workshop.git
cd codex-workshop

# 2. Open a module PDF (example: the architecture deep-dive)
xdg-open 00_Codex-Architecture.pdf    # Linux
# open  00_Codex-Architecture.pdf       # macOS

# 3. List all modules in teaching order
ls -1 *.pdf
```

## Usage

The recommended teaching order follows the numeric prefix `00` → `11`.

```bash
# Day 1 — concepts and surfaces
xdg-open 00_Codex-Architecture.pdf        # Architecture deep-dive
xdg-open 01_Codex_소개와_핵심개념.pdf       # Intro & core concepts
xdg-open 02_CLI_Deep_Dive.pdf             # CLI
xdg-open 03_App과_IDE.pdf                  # App & IDE
xdg-open 04_Codex_on_Web.pdf              # Codex on Web
xdg-open 05_Lab_A_첫_에이전트_작업.pdf       # Lab A (full-cycle lab)

# Day 2 — customization, extension, and automation
xdg-open 06_설정과_커스터마이징.pdf          # Configuration
xdg-open 07_Plugins_Skills_Subagents.pdf  # Plugins, Skills, Subagents
xdg-open 08_Integrations_Security.pdf     # Integrations & Security
xdg-open 09_Automation_SDK.pdf            # Automation & SDK
xdg-open 10_Lab_B_자동화_파이프라인.pdf      # Lab B (automation pipeline lab)
xdg-open 11_Enterprise_Admin.pdf          # Enterprise & Admin
```

## Project Structure

```
codex-workshop/
├── README.md                              # This file
├── CHANGELOG.md                           # Per-version change history
├── 00_Codex-Architecture.pdf              # Architecture deep-dive, 45 slides
├── 01_Codex_소개와_핵심개념.pdf             # M1 Intro & Core Concepts, 23 slides
├── 02_CLI_Deep_Dive.pdf                   # M2 CLI Deep Dive, 22 slides
├── 03_App과_IDE.pdf                        # M3 App & IDE, 19 slides
├── 04_Codex_on_Web.pdf                    # M4 Codex on Web, 14 slides
├── 05_Lab_A_첫_에이전트_작업.pdf            # M5 Lab A — first agent task, 16 slides
├── 06_설정과_커스터마이징.pdf               # M6 Configuration & Customization, 22 slides
├── 07_Plugins_Skills_Subagents.pdf        # M7 Plugins, Skills, Subagents, 14 slides
├── 08_Integrations_Security.pdf           # M8 Integrations & Security, 15 slides
├── 09_Automation_SDK.pdf                  # M9 Automation & SDK, 15 slides
├── 10_Lab_B_자동화_파이프라인.pdf           # M10 Lab B — automation pipeline, 15 slides
└── 11_Enterprise_Admin.pdf                # M11 Enterprise & Admin, 15 slides
```

Modules are numbered in teaching order. Modules 5 (Lab A) and 10 (Lab B) are hands-on labs; the remaining lecture modules each end with a timed mini-lab. The total is **235 slides across 12 PDFs**.

## Contributing

Contributions are welcome. Follow this flow:

1. **Fork** the repository on GitHub.
2. **Branch** from `main`: `git checkout -b fix/your-change`.
3. **Commit** using [Conventional Commits](https://www.conventionalcommits.org):
   - `feat: add prompt-injection demo to module 08`
   - `fix: correct approval-mode table in module 01`
   - `docs: clarify module order in README`
4. **Push** to your fork: `git push origin fix/your-change`.
5. **Open a Pull Request** referencing the relevant issue and describing the change.

For changes that affect slide content, please cite the module and slide number in the commit body so reviewers can cross-reference the PDF.

## License

This project is distributed under **Proprietary** terms. Internal use, private delivery to customers, and modification for internal training are permitted; external redistribution and commercial resale are prohibited.

## Contact

- Maintainer: **Choi WooHyung** — Principal Solutions Architect, AWS Korea
- Email: whchoi98@gmail.com / whchoi@amazon.com
- LinkedIn: [linkedin.com/in/woohyungchoi](https://linkedin.com/in/woohyungchoi)
- Issues: open an issue on the repository hosting this project.

---

# 한국어

## 개요

Codex Deep Dive Workshop은 OpenAI Codex를 위한 한국어 기술 커리큘럼입니다. "코드를 작성하는 모든 곳을 위한 하나의 에이전트 — CLI, IDE, App, Web"이라는 주제를 다룹니다.

자료는 발표용 PDF 슬라이드로 제공됩니다. 첫 설치부터 사람 개입 없이 도는 이슈-투-PR 자동화 파이프라인까지 팀을 단계적으로 안내합니다.

저장소 루트에는 총 **235 슬라이드** 분량의 **12개 모듈 PDF**가 있습니다. 아키텍처 심화 모듈(`00_Codex-Architecture.pdf`) 하나와 순차적인 11개 모듈로 구성됩니다.

그중 두 모듈(Lab A, Lab B)은 종합 실습 랩이고, 대부분의 강의 모듈은 시간제 미니 랩으로 마무리됩니다.

모든 자료는 일관된 디자인 시스템과 이중 언어(한국어 본문, 영어 제목) 레이아웃을 따라 시각 정체성을 유지합니다.

## 주요 기능

- **12개 모듈 PDF 산출물** — 총 235 슬라이드: 아키텍처 심화 모듈과 함께 소개·핵심 개념, CLI, App과 IDE, Codex on Web, 설정·커스터마이징, Plugins/Skills/Subagents, Integrations·Security, Automation·SDK, Enterprise·Admin, 그리고 두 개의 랩으로 구성됩니다. 모든 PDF가 저장소 루트에 위치하여 즉시 열람 가능.
- **계층형 아키텍처 심화** — `00_Codex-Architecture.pdf`(45 슬라이드)는 에이전트 전체 스택을 다룹니다: 에이전트 루프, Input·Knowledge·Execution & Multi-Agent·Observability·Integration 레이어, 그리고 Skills vs. Subagents vs. MCP vs. Hooks의 선택 기준.
- **2개의 End-to-End 실습 랩** — Lab A는 설치·로그인부터 버그 수정, 회귀 테스트, PR 생성까지 풀 사이클을 다루고, Lab B는 시크릿·트리거·검증 게이트·가드레일을 갖춘 자율 이슈-투-PR 자동화 파이프라인을 구축합니다.
- **9개의 시간제 미니 랩** — 강의 모듈은 10~20분 미니 랩으로 마무리되어, 학습자가 각 개념을 즉시 실습할 수 있습니다.
- **Codex의 모든 사용 환경 포함** — CLI, IDE 확장, 데스크톱 App, Codex on Web(클라우드), Automation/SDK + GitHub Action 경로를 각각 전용 모듈로 다룹니다.
- **전반에 걸친 엔터프라이즈·보안** — 샌드박싱, 승인 모드, 프롬프트 인젝션 방어, 위협 모델, 인증, 거버넌스, 관리형 설정, Amazon Bedrock 배포.
- **빌드 단계 없는 즉시 활용** — PDF가 사전 렌더링되어 제공되므로 PDF 뷰어만 있으면 바로 사용할 수 있습니다.

## 사전 요구 사항

- 저장소 루트의 모듈 PDF를 열어볼 수 있는 PDF 뷰어.
- 미니 랩과 Lab A / Lab B를 따라 하기 위한 Codex CLI 설치(모듈 1 "Quickstart — 설치" 참고).
- 연동·자동화 랩(Lab B, 모듈 8, 모듈 9)을 위한 GitHub 계정과 저장소.
- 저장소 클론에 사용할 `git`.

## 설치 방법

```bash
# 1. 저장소 클론
git clone https://github.com/whchoi98/codex-workshop.git
cd codex-workshop

# 2. 모듈 PDF 열기 (예: 아키텍처 심화)
xdg-open 00_Codex-Architecture.pdf    # Linux
# open  00_Codex-Architecture.pdf       # macOS

# 3. 강의 순서대로 모든 모듈 확인
ls -1 *.pdf
```

## 사용법

권장 교육 순서는 숫자 접두사 `00` → `11`을 따릅니다.

```bash
# Day 1 — 개념과 사용 환경
xdg-open 00_Codex-Architecture.pdf        # 아키텍처 심화
xdg-open 01_Codex_소개와_핵심개념.pdf       # 소개와 핵심 개념
xdg-open 02_CLI_Deep_Dive.pdf             # CLI
xdg-open 03_App과_IDE.pdf                  # App과 IDE
xdg-open 04_Codex_on_Web.pdf              # Codex on Web
xdg-open 05_Lab_A_첫_에이전트_작업.pdf       # Lab A (풀 사이클 랩)

# Day 2 — 커스터마이징, 확장, 자동화
xdg-open 06_설정과_커스터마이징.pdf          # 설정과 커스터마이징
xdg-open 07_Plugins_Skills_Subagents.pdf  # Plugins, Skills, Subagents
xdg-open 08_Integrations_Security.pdf     # Integrations와 Security
xdg-open 09_Automation_SDK.pdf            # Automation과 SDK
xdg-open 10_Lab_B_자동화_파이프라인.pdf      # Lab B (자동화 파이프라인 랩)
xdg-open 11_Enterprise_Admin.pdf          # Enterprise와 Admin
```

## 프로젝트 구조

```
codex-workshop/
├── README.md                              # 이 파일
├── CHANGELOG.md                           # 버전별 변경 사항
├── 00_Codex-Architecture.pdf              # 아키텍처 심화, 45 슬라이드
├── 01_Codex_소개와_핵심개념.pdf             # M1 소개와 핵심 개념, 23 슬라이드
├── 02_CLI_Deep_Dive.pdf                   # M2 CLI Deep Dive, 22 슬라이드
├── 03_App과_IDE.pdf                        # M3 App과 IDE, 19 슬라이드
├── 04_Codex_on_Web.pdf                    # M4 Codex on Web, 14 슬라이드
├── 05_Lab_A_첫_에이전트_작업.pdf            # M5 Lab A — 첫 에이전트 작업, 16 슬라이드
├── 06_설정과_커스터마이징.pdf               # M6 설정과 커스터마이징, 22 슬라이드
├── 07_Plugins_Skills_Subagents.pdf        # M7 Plugins, Skills, Subagents, 14 슬라이드
├── 08_Integrations_Security.pdf           # M8 Integrations와 Security, 15 슬라이드
├── 09_Automation_SDK.pdf                  # M9 Automation과 SDK, 15 슬라이드
├── 10_Lab_B_자동화_파이프라인.pdf           # M10 Lab B — 자동화 파이프라인, 15 슬라이드
└── 11_Enterprise_Admin.pdf                # M11 Enterprise와 Admin, 15 슬라이드
```

모듈은 교육 순서대로 번호가 매겨져 있습니다. 모듈 5(Lab A)와 10(Lab B)은 종합 실습 랩이며, 나머지 강의 모듈은 각각 시간제 미니 랩으로 마무리됩니다. 전체 분량은 **12개 PDF, 235 슬라이드**입니다.

## 기여 방법

기여를 환영합니다. 아래 순서를 따라 주세요.

1. GitHub에서 저장소를 **포크(Fork)** 합니다.
2. `main`에서 새 **브랜치(Branch)** 를 생성합니다: `git checkout -b fix/your-change`.
3. [Conventional Commits](https://www.conventionalcommits.org) 형식으로 **커밋(Commit)** 합니다.
   - `feat: 모듈 08에 프롬프트 인젝션 데모 추가`
   - `fix: 모듈 01의 승인 모드 표 수정`
   - `docs: README의 모듈 순서 설명 명확화`
4. 포크된 저장소에 **푸시(Push)** 합니다: `git push origin fix/your-change`.
5. 관련 이슈를 참조하고 변경 사항을 설명하며 **Pull Request** 를 엽니다.

슬라이드 내용이 변경되는 경우, 리뷰어가 PDF와 대조할 수 있도록 커밋 본문에 모듈과 슬라이드 번호를 명시해 주세요.

## 라이선스

이 프로젝트는 **Proprietary** 조건으로 배포됩니다. 내부 활용, 고객사 대상 비공개 발표, 사내 교육 목적의 수정은 허용되며, 외부 공개 재배포와 상업적 재판매는 금지됩니다.

## 연락처

- 메인테이너: **최우형(Choi WooHyung)** — Principal Solutions Architect, AWS Korea
- 이메일: whchoi98@gmail.com / whchoi@amazon.com
- LinkedIn: [linkedin.com/in/woohyungchoi](https://linkedin.com/in/woohyungchoi)
- 이슈: 이 프로젝트가 호스팅된 저장소에 이슈를 등록해 주세요.
