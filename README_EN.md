<p align="center">
  <img src="https://img.shields.io/badge/skills-23-brightgreen?style=for-the-badge&logo=shield&logoColor=white" alt="Skills">
  <img src="https://img.shields.io/badge/frameworks-6-blue?style=for-the-badge" alt="Frameworks">
  <img src="https://img.shields.io/badge/license-MIT-green?style=for-the-badge" alt="License">
</p>

<h1 align="center">MiMoCode Skills</h1>

<p align="center">
  <b>23 production-ready skills for AI coding agents — cybersecurity, design, engineering, IoT/hardware security</b><br>
  Adapted from <a href="https://github.com/garrytan/gstack">gstack</a>, <a href="https://github.com/affaan-m/ECC">ECC</a>, <a href="https://github.com/bergside/typeui">TypeUI</a>, <a href="https://github.com/BrownFineSecurity/iothackbot">IoTHackBot</a>, and security research repos
</p>

<p align="center">
  <a href="#quick-start">Quick Start</a> •
  <a href="#skills-catalog">Skills</a> •
  <a href="#usage">Usage</a> •
  <a href="#workflows">Workflows</a> •
  <a href="#sources">Sources</a>
</p>

---

## What is this?

A collection of **23 structured skills** that give AI coding agents specialized capabilities:

- **Code review** with confidence scoring and severity classification
- **Systematic debugging** with root cause analysis
- **QA testing** with health scores and triage
- **Security audits** with OWASP/WCAG checklists
- **Penetration testing** with PTES methodology
- **Incident response** with NIST/SANS playbooks
- **Design systems** with universal UI/UX principles
- **TDD workflows** with RED/GREEN/REFACTOR cycles
- **IoT/Hardware security** — firmware, Android, JTAG/UART, network

Each skill is a self-contained `SKILL.md` file with:
- When to use (triggers)
- Step-by-step workflow
- Commands and code examples
- Output format

---

## Quick Start

### Option 1: Clone to MiMoCode

```bash
git clone https://github.com/Samuraiprm/mimocode-skills.git ~/.mimocode/skills
```

### Option 2: Copy specific skills

```bash
git clone https://github.com/Samuraiprm/mimocode-skills.git /tmp/mimocode-skills

# Pick only what you need
cp -r /tmp/mimocode-skills/code-review ~/.mimocode/skills/
cp -r /tmp/mimocode-skills/investigate ~/.mimocode/skills/
cp -r /tmp/mimocode-skills/security-review ~/.mimocode/skills/
```

### Option 3: Use in any project

```bash
# Clone into your project
git clone https://github.com/Samuraiprm/mimocode-skills.git .mimocode-skills

# Or as a submodule
git submodule add https://github.com/Samuraiprm/mimocode-skills.git .mimocode-skills
```

---

## Skills Catalog

### Engineering Workflow

| Skill | Source | Description |
|-------|--------|-------------|
| [`code-review`](skills/code-review/SKILL.md) | [gstack](https://github.com/garrytan/gstack) | Pre-landing PR review — SQL safety, race conditions, trust boundary violations. Confidence scoring (1-10), severity classification (P0-P3) |
| [`investigate`](skills/investigate/SKILL.md) | [gstack](https://github.com/garrytan/gstack) | Systematic debugging — Iron Law: no fixes without root cause. 5 phases, 3-strike rule, structured debug report |
| [`qa-test`](skills/qa-test/SKILL.md) | [gstack](https://github.com/garrytan/gstack) | QA testing web apps — 3 tiers (Quick/Standard/Exhaustive), health score across 8 categories, before/after comparison |
| [`search-first`](skills/search-first/SKILL.md) | [ECC](https://github.com/affaan-m/ECC) | Research before coding — search package registries, GitHub, docs. Adopt/Extend/Build decision matrix |
| [`verification-loop`](skills/verification-loop/SKILL.md) | [ECC](https://github.com/affaan-m/ECC) | Quality gates — build → types → lint → tests → security → diff. Stop and fix on failure |
| [`tdd-workflow`](skills/tdd-workflow/SKILL.md) | [ECC](https://github.com/affaan-m/ECC) | Test-driven development — RED → GREEN → REFACTOR. 80%+ coverage, git checkpoints |

### Security

| Skill | Source | Description |
|-------|--------|-------------|
| [`security-review`](skills/security-review/SKILL.md) | [ECC](https://github.com/affaan-m/ECC) | Security checklist — secrets, input validation, auth, API security, data protection. PASS/FAIL verification |
| [`code-audit`](skills/code-audit/SKILL.md) | [CyberSecurity-Skills](https://github.com/Hi-FullHouse/CyberSecurity-Skills) | Security code audit — static analysis (bandit, semgrep, gosec), vulnerability patterns, framework-specific checks |
| [`pentest`](skills/pentest/SKILL.md) | [Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) | Penetration testing — PTES lifecycle: recon → scanning → exploitation → post-exploitation → report |
| [`incident-response`](skills/incident-response/SKILL.md) | [Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) | IR procedures — NIST/SANS PICERL framework, playbooks for ransomware, phishing, data breach, insider threat |
| [`threat-hunting`](skills/threat-hunting/SKILL.md) | [Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) | Proactive threat hunting — hypothesis-driven, MITRE ATT&CK mapping, detection rule creation |

### Design

| Skill | Source | Description |
|-------|--------|-------------|
| [`design-system`](skills/design-system/SKILL.md) | [TypeUI](https://github.com/bergside/typeui) | Universal design principles — 4pt grid spacing, typography scale, WCAG accessibility, 12 UX laws |
| [`design-audit`](skills/design-audit/SKILL.md) | [TypeUI](https://github.com/bergside/typeui) | UI audit — spacing, typography, contrast, components, interaction, accessibility. Compliance check |

### IoT & Hardware Security

| Skill | Source | Description |
|-------|--------|-------------|
| [`iot-nmap`](iot-nmap/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | Network recon — two-phase scan, service detection, NSE scripts |
| [`iot-chipsec`](iot-chipsec/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | UEFI/BIOS firmware — rootkit detection, EFI inventory, NVRAM |
| [`iot-apktool`](iot-apktool/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | Android APK — resource decoding, smali code |
| [`iot-jadx`](iot-jadx/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | Android decompile — DEX → Java, hardcoded credentials |
| [`iot-jtagprobe`](iot-jtagprobe/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | Hardware debug — SWD/JTAG probe, OPEN/LOCKED/DEAD |
| [`iot-picocom`](iot-picocom/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | UART console — bootloader, shell, firmware extraction |
| [`iot-telnetshell`](iot-telnetshell/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | Telnet shell — unauthenticated access, BusyBox |
| [`iot-wsdiscovery`](iot-wsdiscovery/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | WS-Discovery — ONVIF camera and IoT detection |
| [`iot-iotnet`](iot-iotnet/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | Traffic analysis — IoT protocols, vulnerabilities |
| [`iot-ffind`](iot-ffind/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | File finder — type detection, ext2/3/4, F2FS extraction |

---

## Usage

### Natural Language

Just describe what you need — MiMoCode picks the right skill:

```
Проведи ревью кода на ветке feature/auth
Обеги дебаг: упал запрос к API
Сделай QA тестирование сайта https://staging.myapp.com
Проведи security review этого модуля
```

### Explicit Skill Name

Mention the skill name directly:

```
Запусти code-review
Запусти investigate для этого бага
Запусти pentest для тестирования эндпоинта
```

### Combine Skills

Chain multiple skills in one task:

```
Сделай код-ревью, потом верификацию, потом security review
```

---

## Workflows

### New Feature
```
search-first → tdd-workflow → code-review → verification-loop
```

### Bug Fix
```
investigate → code-audit → verification-loop
```

### Pre-Release
```
code-review → security-review → qa-test → verification-loop
```

### Security Audit
```
code-audit → security-review → pentest
```

### Incident
```
incident-response → threat-hunting → code-audit
```

### UI/UX
```
design-system → design-audit
```

### IoT Pentest
```
iot-nmap → iot-wsdiscovery → iot-iotnet → pentest
```

### Firmware Analysis
```
iot-chipsec → iot-ffind → code-audit
```

### Android Reverse Engineering
```
iot-apktool → iot-jadx → code-audit
```

### Hardware Debug
```
iot-jtagprobe → iot-picocom → iot-telnetshell
```

---

## Skill Details

### code-review

**When:** Before merging PRs, reviewing diffs

**Workflow:**
1. Detect base branch and get diff
2. Apply critical categories: SQL safety, race conditions, shell injection, type coercion
3. Score confidence (1-10) and severity (P0-P3)
4. Output structured findings

**Example output:**
```
[P1] (confidence: 9/10) app/models/user.rb:42 — SQL injection via string interpolation
Fix: Use parameterized queries
```

### investigate

**When:** Bugs, errors, "it was working yesterday"

**Workflow:**
1. Root Cause Investigation — collect symptoms, read code, check changes
2. Pattern Analysis — race condition, null propagation, state corruption
3. Hypothesis Testing — verify before fixing. 3-strike rule
4. Implementation — minimal diff, regression test
5. Verification & Report

**Iron Law:** No fixes without root cause.

### qa-test

**When:** "Does this work?", pre-launch testing

**Tiers:**
- Quick: Critical/high only
- Standard: + medium issues
- Exhaustive: + cosmetic

**Health score:** Weighted average across Console, Links, Visual, Functional, UX, Performance, Content, Accessibility.

### search-first

**When:** Before writing new code

**Decision matrix:**
| Signal | Action |
|--------|--------|
| Exact match, well-maintained | Adopt |
| Partial match | Extend (wrapper) |
| Multiple weak matches | Compose |
| Nothing found | Build custom |

### verification-loop

**When:** After features, before PRs, after refactoring

**Phases:** Build → Type Check → Lint → Tests → Security → Diff

**Rule:** Stop and fix if any phase fails.

### tdd-workflow

**When:** New features, bug fixes, refactoring

**Cycle:** RED (failing test) → GREEN (minimal code) → REFACTOR (clean up)

**Requirements:** 80%+ coverage, git checkpoints after each stage.

### security-review

**When:** Auth, input handling, API endpoints, secrets

**Checklist:** Secrets, Input Validation, Auth, API Security, Data Protection

### code-audit

**When:** Security audit, compliance

**Process:** Detect language → Run static analysis → Check vulnerability patterns → Framework-specific checks

**Tools:** bandit, semgrep, gosec, brakeman, spotbugs

### pentest

**When:** Authorized penetration testing only

**PTES Lifecycle:** Recon → Scanning → Exploitation → Post-Exploitation → Report

**⚠️ Authorized use only.** Never test systems without written permission.

### incident-response

**When:** Responding to security incidents

**Framework:** PICERL (Preparation, Identification, Containment, Eradication, Recovery, Lessons Learned)

**Playbooks:** Ransomware, Phishing/BEC, Data Breach, Insider Threat

### threat-hunting

**When:** Proactive threat search

**Process:** Form hypothesis → Identify data sources → Investigate → Map to MITRE ATT&CK → Create detection rules

### design-system

**When:** Design decisions, UI components

**Principles:**
- 4-point grid (4, 8, 12, 16, 24, 32, 48, 64, 96 px)
- Inner gaps < outer gaps (proximity grouping)
- Typography: min 16px primary, 14px secondary
- Accessibility: WCAG 2.1/2.2 AA baseline

### design-audit

**When:** UI review before launch

**Categories:** Spacing, Typography, Contrast, Components, Interaction, Accessibility

---

## Compatibility

These skills work with any AI coding agent that supports markdown files:

- MiMoCode
- Claude Code
- Codex
- Cursor
- OpenCode
- Any agent that reads SKILL.md files

---

## Sources

| Repository | Stars | Skills Adapted |
|------------|-------|----------------|
| [gstack](https://github.com/garrytan/gstack) | 119K | code-review, investigate, qa-test |
| [ECC](https://github.com/affaan-m/ECC) | 225K | search-first, verification-loop, security-review, tdd-workflow |
| [TypeUI](https://github.com/bergside/typeui) | — | design-system, design-audit |
| [Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) | — | pentest, incident-response, threat-hunting |
| [CyberSecurity-Skills](https://github.com/Hi-FullHouse/CyberSecurity-Skills) | — | code-audit |
| [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | — | iot-nmap, iot-chipsec, iot-apktool, iot-jadx, iot-jtagprobe, iot-picocom, iot-telnetshell, iot-wsdiscovery, iot-iotnet, iot-ffind |

---

## Contributing

1. Fork the repo
2. Create your skill: `mkdir skills/my-skill`
3. Write `SKILL.md` following the existing format
4. Submit a PR

**Skill format:**
```markdown
---
name: skill-name
description: What it does
origin: source repo
---

## When to Use
...

## Workflow
### Step 1: ...
### Step 2: ...

## Output
```

---

## License

MIT — use freely in personal and commercial projects.

---

<p align="center">
  <sub>Built with care for the AI coding community</sub>
</p>
