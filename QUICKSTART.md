# MiMoCode Skills — Быстрый старт

13 готовых навыков для AI-агентов — кибербезопасность, дизайн, инженерные процессы.

## Установка

```bash
# Полная установка
git clone https://github.com/Samuraiprm/mimocode-skills.git ~/.mimocode/skills

# Или выбрать конкретные навыки
git clone https://github.com/Samuraiprm/mimocode-skills.git /tmp/mimocode-skills
cp -r /tmp/mimocode-skills/code-review ~/.mimocode/skills/
```

## Навыки

| Навык | Категория | Описание |
|-------|-----------|----------|
| code-review | Инженерия | Ревью PR с оценкой уверенности |
| investigate | Инженерия | Систематический дебаггинг, root cause |
| qa-test | Инженерия | QA тестирование с health scores |
| search-first | Инженерия | Исследование перед кодом |
| verification-loop | Инженерия | Quality gates: build→types→lint→tests |
| tdd-workflow | Инженерия | TDD: RED→GREEN→REFACTOR |
| security-review | Безопасность | Чеклист и верификация безопасности |
| code-audit | Безопасность | Static analysis и паттерны уязвимостей |
| pentest | Безопасность | Методология PTES |
| incident-response | Безопасность | Плейбуки NIST/SANS |
| threat-hunting | Безопасность | Proactive hunting, MITRE ATT&CK |
| design-system | Дизайн | Универсальные принципы UI/UX |
| design-audit | Дизайн | Аудит UI на соответствие |

## Использование

```
Проведи ревью кода
Запусти investigate для этого бага
Сделай security review
```

Подробная документация: [README.md](README.md)
