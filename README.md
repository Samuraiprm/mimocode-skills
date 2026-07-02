<p align="center">
  <img src="https://img.shields.io/badge/навыки-23-brightgreen?style=for-the-badge&logo=shield&logoColor=white" alt="Навыки">
  <img src="https://img.shields.io/badge/фреймворки-6-blue?style=for-the-badge" alt="Фреймворки">
  <img src="https://img.shields.io/badge/лицензия-MIT-green?style=for-the-badge" alt="Лицензия">
  <img src="https://img.shields.io/badge/язык-🇷🇺%20English-blueviolet?style=for-the-badge" alt="Язык">
</p>

<h1 align="center">MiMoCode Skills</h1>

<p align="center">
  <b>23 готовых навыка для AI-агентов — кибербезопасность, дизайн, инженерные процессы, IoT/hardware security</b><br>
  Адаптировано из <a href="https://github.com/garrytan/gstack">gstack</a>, <a href="https://github.com/affaan-m/ECC">ECC</a>, <a href="https://github.com/bergside/typeui">TypeUI</a>, <a href="https://github.com/BrownFineSecurity/iothackbot">IoTHackBot</a> и репозиториев безопасности
</p>

<p align="center">
  <a href="#быстрый-старт">Быстрый старт</a> •
  <a href="#каталог-навыков">Навыки</a> •
  <a href="#использование">Использование</a> •
  <a href="#рабочие-процессы">Workflow'ы</a> •
  <a href="#источники">Источники</a> •
  <a href="README_EN.md">English</a>
</p>

---

## Что это?

Коллекция из **23 структурированных навыков**, которые дают AI-агентам специализированные возможности:

- **Ревью кода** с оценкой уверенности и классификацией серьёзности
- **Систематический дебаггинг** с анализом корневой причины
- **QA тестирование** с оценкой здоровья и триажем
- **Безопасный аудит** с чеклистами OWASP/WCAG
- **Пентест** с методологией PTES
- **Реагирование на инциденты** с плейбуками NIST/SANS
- **Дизайн-системы** с универсальными принципами UI/UX
- **TDD процессы** с циклами RED/GREEN/REFACTOR
- **IoT/Hardware Security** — анализ прошивок, Android, JTAG/UART, сеть

Каждый навык — это самодостаточный файл `SKILL.md` с:
- Триггерами (когда использовать)
- Пошаговым workflow'ом
- Командами и примерами кода
- Форматом вывода

---

## Быстрый старт

### Вариант 1: Клонировать целиком

```bash
git clone https://github.com/Samuraiprm/mimocode-skills.git ~/.mimocode/skills
```

### Вариант 2: Скопировать конкретные навыки

```bash
git clone https://github.com/Samuraiprm/mimocode-skills.git /tmp/mimocode-skills

# Выбрать только нужное
cp -r /tmp/mimocode-skills/code-review ~/.mimocode/skills/
cp -r /tmp/mimocode-skills/investigate ~/.mimocode/skills/
cp -r /tmp/mimocode-skills/security-review ~/.mimocode/skills/
```

### Вариант 3: Использовать в проекте

```bash
# Клонировать в проект
git clone https://github.com/Samuraiprm/mimocode-skills.git .mimocode-skills

# Или как submodule
git submodule add https://github.com/Samuraiprm/mimocode-skills.git .mimocode-skills
```

---

## Каталог навыков

### Инженерные процессы

| Навык | Источник | Описание |
|-------|----------|----------|
| [`code-review`](code-review/SKILL.md) | [gstack](https://github.com/garrytan/gstack) | Ревью PR перед мержем — SQL safety, race conditions, trust boundary. Confidence score (1-10), severity (P0-P3) |
| [`investigate`](investigate/SKILL.md) | [gstack](https://github.com/garrytan/gstack) | Систематический дебаггинг — Iron Law: нет фикса без root cause. 5 фаз, 3-strike rule |
| [`qa-test`](qa-test/SKILL.md) | [gstack](https://github.com/garrytan/gstack) | QA тестирование web-приложений — 3 tier'а, health score по 8 категориям, до/после сравнение |
| [`search-first`](search-first/SKILL.md) | [ECC](https://github.com/affaan-m/ECC) | Исследование перед кодом — поиск в registries, GitHub, docs. Adopt/Extend/Build матрица |
| [`verification-loop`](verification-loop/SKILL.md) | [ECC](https://github.com/affaan-m/ECC) | Quality gates — build → types → lint → tests → security → diff. Стоп при ошибке |
| [`tdd-workflow`](tdd-workflow/SKILL.md) | [ECC](https://github.com/affaan-m/ECC) | TDD — RED → GREEN → REFACTOR. 80%+ coverage, git checkpoints |

### Безопасность

| Навык | Источник | Описание |
|-------|----------|----------|
| [`security-review`](security-review/SKILL.md) | [ECC](https://github.com/affaan-m/ECC) | Чеклист безопасности — secrets, input, auth, API, data. PASS/FAIL верификация |
| [`code-audit`](code-audit/SKILL.md) | [CyberSecurity-Skills](https://github.com/Hi-FullHouse/CyberSecurity-Skills) | Аудит кода — static analysis (bandit, semgrep, gosec), паттерны уязвимостей |
| [`pentest`](pentest/SKILL.md) | [Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) | Пентест — PTES: recon → scanning → exploitation → post-exploitation → report |
| [`incident-response`](incident-response/SKILL.md) | [Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) | IR — NIST/SANS PICERL, плейбуки: ransomware, phishing, data breach, insider threat |
| [`threat-hunting`](threat-hunting/SKILL.md) | [Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) | Proactive hunting — hypothesis-driven, MITRE ATT&CK, detection rules |

### Дизайн

| Навык | Источник | Описание |
|-------|----------|----------|
| [`design-system`](design-system/SKILL.md) | [TypeUI](https://github.com/bergside/typeui) | Универсальные принципы — 4pt grid, typography scale, WCAG, 12 UX-законов |
| [`design-audit`](design-audit/SKILL.md) | [TypeUI](https://github.com/bergside/typeui) | Аудит UI — spacing, typography, contrast, components, interaction, accessibility |

### IoT и Hardware Security

| Навык | Источник | Описание |
|-------|----------|----------|
| [`iot-nmap`](iot-nmap/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | Сетевая разведка — двухфазовый скан, service detection, NSE scripts |
| [`iot-chipsec`](iot-chipsec/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | Анализ UEFI/BIOS — rootkit detection, EFI inventory, NVRAM |
| [`iot-apktool`](iot-apktool/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | Android APK — декодирование ресурсов, smali код |
| [`iot-jadx`](iot-jadx/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | Android decompile — DEX → Java, hardcoded credentials |
| [`iot-jtagprobe`](iot-jtagprobe/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | Hardware debug — SWD/JTAG probe, OPEN/LOCKED/DEAD |
| [`iot-picocom`](iot-picocom/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | UART консоль — bootloader, shell, firmware extraction |
| [`iot-telnetshell`](iot-telnetshell/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | Telnet shell — unauthenticated access, BusyBox |
| [`iot-wsdiscovery`](iot-wsdiscovery/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | WS-Discovery — обнаружение ONVIF камер и IoT |
| [`iot-iotnet`](iot-iotnet/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | Анализ трафика — протоколы IoT, уязвимости |
| [`iot-ffind`](iot-ffind/SKILL.md) | [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | Поиск файлов — type detection, ext2/3/4, F2FS extraction |

---

## Использование

### На естественном языке

Просто опишите задачу — MiMoCode подберёт навык:

```
Проведи ревью кода на ветке feature/auth
Обеги дебаг: упал запрос к API, вот ошибка...
Сделай QA тестирование сайта https://staging.myapp.com
Проведи security review этого модуля
```

### Явное указание навыка

Напишите имя навыка:

```
Запусти code-review
Запусти investigate для этого бага
Запусти pentest для тестирования эндпоинта
```

### Комбинация навыков

Объедините несколько навыков в одну задачу:

```
Сделай код-ревью, потом верификацию, потом security review
```

---

## Рабочие процессы

### Новая фича
```
search-first → tdd-workflow → code-review → verification-loop
```

### Баг-фикс
```
investigate → code-audit → verification-loop
```

### Перед релизом
```
code-review → security-review → qa-test → verification-loop
```

### Security аудит
```
code-audit → security-review → pentest
```

### Инцидент
```
incident-response → threat-hunting → code-audit
```

### UI/UX
```
design-system → design-audit
```

### IoT пентест
```
iot-nmap → iot-wsdiscovery → iot-iotnet → pentest
```

### Firmware анализ
```
iot-chipsec → iot-ffind → code-audit
```

### Android реверс
```
iot-apktool → iot-jadx → code-audit
```

### Hardware debug
```
iot-jtagprobe → iot-picocom → iot-telnetshell
```

---

## Подробное описание каждого навыка

### code-review

**Когда:** перед мержем PR, при проверке диффа

**Workflow:**
1. Определяет base branch и получает diff
2. Проверяет критичные категории: SQL injection, race conditions, shell injection, type coercion
3. Оценивает confidence (1-10) и severity (P0-P3)
4. Выводит структурированные находки

**Пример вывода:**
```
[P1] (confidence: 9/10) app/models/user.rb:42 — SQL injection через интерполяцию строк
Fix: Использовать параметризованные запросы
```

### investigate

**Когда:** баги, ошибки, "вчера работало"

**Workflow:**
1. Root Cause Investigation — собирает симптомы, читает код, проверяет изменения
2. Pattern Analysis — race condition, null propagation, state corruption
3. Hypothesis Testing — проверяет перед фиксом. 3-strike rule
4. Implementation — минимальный diff, regression test
5. Verification & Report

**Iron Law:** Нет фикса без root cause.

### qa-test

**Когда:** "does this work?", тестирование перед релизом

**Tier'ы:**
- Quick: Только critical/high
- Standard: + medium
- Exhaustive: + cosmetic

**Health score:** Взвешенное среднее по Console, Links, Visual, Functional, UX, Performance, Content, Accessibility.

### search-first

**Когда:** перед написанием нового кода

**Матрица решений:**
| Сигнал | Действие |
|--------|----------|
| Точное совпадение, поддерживается | Adopt |
| Частичное совпадение | Extend (обёртка) |
| Слабые совпадения | Compose |
| Ничего не найдено | Build |

### verification-loop

**Когда:** после фич, перед PR, после рефакторинга

**Фазы:** Build → Type Check → Lint → Tests → Security → Diff

**Правило:** Стоп и фикс если любая фаза упала.

### tdd-workflow

**Когда:** новые фичи, баг-фиксы, рефакторинг

**Цикл:** RED (падающий тест) → GREEN (минимальный код) → REFACTOR (очистка)

**Требования:** 80%+ coverage, git checkpoints после каждого этапа.

### security-review

**Когда:** auth, обработка ввода, API эндпоинты, секреты

**Чеклист:** Secrets, Input Validation, Auth, API Security, Data Protection

### code-audit

**Когда:** security аудит, compliance

**Процесс:** Определение языка → Static analysis → Паттерны уязвимостей → Framework-specific проверки

**Инструменты:** bandit, semgrep, gosec, brakeman, spotbugs

### pentest

**Когда:** авторизованный пентест

**PTES:** Recon → Scanning → Exploitation → Post-Exploitation → Report

**⚠️ Только для авторизованного тестирования!**

### incident-response

**Когда:** реагирование на инциденты

**Фреймворк:** PICERL (Preparation, Identification, Containment, Eradication, Recovery, Lessons Learned)

**Плейбуки:** Ransomware, Phishing/BEC, Data Breach, Insider Threat

### threat-hunting

**Когда:** proactive поиск угроз

**Процесс:** Гипотеза → Источники данных → Расследование → MITRE ATT&CK → Detection rules

### design-system

**Когда:** дизайн-решения, UI компоненты

**Принципы:**
- 4-point grid (4, 8, 12, 16, 24, 32, 48, 64, 96 px)
- Inner gaps < outer gaps
- Typography: min 16px primary, 14px secondary
- Accessibility: WCAG 2.1/2.2 AA

### design-audit

**Когда:** ревью UI перед релизом

**Категории:** Spacing, Typography, Contrast, Components, Interaction, Accessibility

---

## IoT и Hardware Security (из IoTHackBot)

### iot-nmap

**Когда:** сетевая разведка, сканирование портов

**Workflow:**
1. Быстрый SYN scan всех 65535 портов
2. Service detection на найденных портах
3. NSE scripts для доп. enumeration

**Особенность:** Автоматически обрабатывает "host down" с -Pn

### iot-chipsec

**Когда:** анализ UEFI/BIOS прошивок

**Возможности:**
- Детектирует rootkit'ы: LoJax, ThinkPwn, HackingTeam, MosaicRegressor
- Генерирует EFI inventory с хэшами (MD5, SHA256)
- Извлекает NVRAM переменные
- Парсит SPI flash descriptors

### iot-apktool

**Когда:** reverse engineering Android APK

**Возможности:**
- Декодирует AndroidManifest.xml
- Извлекает ресурсы, layouts, strings
- Disassemble в smali код
- Репакетинг модифицированных APK

### iot-jadx

**Когда:** декомпиляция Android приложений

**Возможности:**
- Конвертирует DEX → читаемый Java исходник
- Поиск hardcoded credentials
- Анализ логики приложения

### iot-jtagprobe

**Когда:** hardware debug, JTAG/SWD тестирование

**Возможности:**
- Классифицирует устройства: OPEN / LOCKED / DEAD
- Sweep SWD и JTAG на разных clock speeds
- Декодирует DPIDR/IDCODE → вендор (STM32, NXP, Nordic, TI)
- Halt + memory read для подтверждения контроля

### iot-picocom

**Когда:** UART консоль к IoT устройствам

**Возможности:**
- Manipulation bootloader'а
- Shell enumeration
- Firmware extraction
- Python helper скрипт для автоматизации

### iot-telnetshell

**Когда:** telnet доступ к IoT

**Возможности:**
- Тестирование unauthenticated shell
- Device enumeration
- BusyBox command handling
- Pre-built enumeration скрипты

### iot-wsdiscovery

**Когда:** обнаружение IoT устройств в сети

**Возможности:**
- WS-Discovery протокол сканер
- Обнаружение ONVIF камер
- Автоматическое определение subnet

### iot-iotnet

**Когда:** анализ сетевого трафика IoT

**Возможности:**
- Детектирует протоколы IoT
- Находит уязвимости в трафике
- Анализ PCAP файлов

### iot-ffind

**Когда:** поиск и анализ файлов в firmware

**Возможности:**
- Определяет типы файлов
- Извлекает ext2/3/4 и F2FS файловые системы
- Предназначен для firmware анализа

---

## Совместимость

Навыки работают с любым AI-агентом, поддерживающим markdown:

- MiMoCode
- Claude Code
- Codex
- Cursor
- OpenCode
- Любой агент, читающий SKILL.md

---

## Источники

| Репозиторий | Звёзд | Навыков адаптировано |
|------------|-------|---------------------|
| [gstack](https://github.com/garrytan/gstack) | 119K | code-review, investigate, qa-test |
| [ECC](https://github.com/affaan-m/ECC) | 225K | search-first, verification-loop, security-review, tdd-workflow |
| [TypeUI](https://github.com/bergside/typeui) | — | design-system, design-audit |
| [Anthropic-Cybersecurity-Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) | — | pentest, incident-response, threat-hunting |
| [CyberSecurity-Skills](https://github.com/Hi-FullHouse/CyberSecurity-Skills) | — | code-audit |
| [IoTHackBot](https://github.com/BrownFineSecurity/iothackbot) | — | iot-nmap, iot-chipsec, iot-apktool, iot-jadx, iot-jtagprobe, iot-picocom, iot-telnetshell, iot-wsdiscovery, iot-iotnet, iot-ffind |

---

## Вклад

1. Форкните репозиторий
2. Создайте навык: `mkdir skills/my-skill`
3. Напишите `SKILL.md` по существующему формату
4. Отправьте PR

**Формат навыка:**
```markdown
---
name: skill-name
description: Что делает
origin: исходный репо
---

## Когда использовать
...

## Workflow
### Шаг 1: ...
### Шаг 2: ...

## Вывод
```

---

## Лицензия

MIT — свободное использование в личных и коммерческих проектах.

---

<p align="center">
  <sub>Создано с заботой для AI coding сообщества</sub>
</p>
