# rvrhxg · Python Backend

Разрабатываю самостоятельные проекты на Python: REST API, работу с базами данных, транзакции и инструменты диагностики. Основной стек — Python, FastAPI, SQLAlchemy, Alembic, PostgreSQL, aiogram, pytest и Docker.

## Python-проекты

| Проект | Что реализовано | Код |
|---|---|---|
| **Atelier Commerce** | Поиск и cursor-пагинация, постоянная корзина пользователя, версионирование её снимка, транзакционное оформление заказа и очистка корзины, идемпотентность и защита от продажи сверх остатка | [E-commerce Platform](https://github.com/rvrhxg/E-commerce-Platform) |
| **Deskline** | Telegram-команды записи, административный REST API, расписания сотрудников, защита пересечений и повторов обновлений | [Telegram Business Bot](https://github.com/rvrhxg/Telegram-Business-Bot) |
| **Ledger** | Учёт операций, атомарный CSV-импорт, SQL-агрегации, сравнение периодов, бюджеты и экспорт отчётов | [Finance Dashboard](https://github.com/rvrhxg/Finance-Dashboard) |
| **API Health Monitor** | HTTP-проверки, измерение времени ответа, тайм-ауты, ограниченные повторные попытки, безопасные JSON-логи и CSV; локальная демонстрация сбоя и восстановления | [API Health Monitor](https://github.com/rvrhxg/API-Health-Monitor) |

Atelier, Deskline и Ledger содержат проверки прав, Docker, браузерные сценарии и техническую документацию. PostgreSQL-проверки выполняются для Atelier и Ledger; Deskline использует SQLite. Проверяются readiness, исключение секретов из HTTP-логов и восстановление тестовых резервных копий.

API Health Monitor — отдельная CLI-утилита без сторонних runtime-зависимостей: 23 pytest-теста с mock HTTP и локальным демонстрационным сервером. Это разовая диагностика, без фонового планировщика и уведомлений.

Все четыре Python-проекта проверены в CI на Python 3.12–3.14.

## Демонстрации и проверки

- [Atelier: демонстрация интерфейса](https://github.com/rvrhxg/E-commerce-Platform/tree/main/docs/demo) · [CI постоянной корзины](https://github.com/rvrhxg/E-commerce-Platform/actions/runs/44296016413)
- [Deskline: демонстрация интерфейса](https://github.com/rvrhxg/Telegram-Business-Bot/tree/main/docs/demo)
- [Ledger: демонстрация интерфейса](https://github.com/rvrhxg/Finance-Dashboard/tree/main/docs/demo)
- [API Health Monitor: запуск и диагностика](https://github.com/rvrhxg/API-Health-Monitor#readme) · [CI Python 3.12–3.14](https://github.com/rvrhxg/API-Health-Monitor/actions/runs/44502702068)

Записи интерфейса показывают вымышленные сценарии; новые возможности описаны в актуальных README репозиториев.

## Другие fullstack-проекты

- [Relay HelpDesk](https://github.com/rvrhxg/-helpdesk-system) — обращения, роли, диалоги и аудит; SLA первого ответа и решения по приоритетам, индикаторы просрочек и аналитика команды. Node.js 24 / SQLite. [Скриншот SLA](https://github.com/rvrhxg/-helpdesk-system/blob/main/docs/screenshots/sla-analytics-desktop.png) · [CI](https://github.com/rvrhxg/-helpdesk-system/actions/runs/44501327397).
- [Contour CRM](https://github.com/rvrhxg/business-crm) — клиенты, воронка, сделки и задачи; Node.js 24 / SQLite.

Инструкции запуска, архитектура и ограничения находятся в README каждого проекта.

Все проекты — учебные MVP с вымышленными демоданными. Коммерческая эксплуатация и production-готовность не заявляются. Реальные платежи, банковские подключения и живая доставка Telegram не входят в подтверждённые сценарии.
