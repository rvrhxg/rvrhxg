# rvrhxg · Python Backend

Портфолио самостоятельных учебных проектов: REST API, транзакции, моделирование данных и автоматические проверки. Основной стек — Python, FastAPI, SQLAlchemy, Alembic, PostgreSQL, aiogram, pytest и Docker.

## Python-проекты

| Проект | Что реализовано | Код |
|---|---|---|
| **Atelier Commerce** | Серверный поиск и cursor-пагинация, транзакционное оформление заказа, снимки цен, идемпотентность и защита от overselling | [E-commerce Platform](https://github.com/rvrhxg/E-commerce-Platform) |
| **Deskline** | Telegram-команды записи, административный REST API, расписания сотрудников, защита пересечений и повторов обновлений | [Telegram Business Bot](https://github.com/rvrhxg/Telegram-Business-Bot) |
| **Ledger** | Учёт операций, атомарный CSV-импорт, SQL-агрегации, сравнение периодов, бюджеты и экспорт отчётов | [Finance Dashboard](https://github.com/rvrhxg/Finance-Dashboard) |

В Python-проектах есть версионированные схемы, проверки прав, Docker, CI на Python3.12–3.14, браузерные сценарии и техническая документация. PostgreSQL-проверки выполняются для Atelier и Ledger; Deskline использует SQLite. Проверяются readiness, исключение секретов из HTTP-логов и восстановление тестовых резервных копий.

[Скриншоты, запуск и точные границы проверок](https://github.com/rvrhxg/Finance-Dashboard/blob/main/docs/PORTFOLIO.md)

## Другие fullstack-проекты

- [Relay HelpDesk](https://github.com/rvrhxg/-helpdesk-system) — обращения, роли, ответы и история изменений; Node.js24/SQLite.
- [Contour CRM](https://github.com/rvrhxg/business-crm) — клиенты, воронка, сделки и задачи; Node.js24/SQLite.

Все проекты — учебные MVP с вымышленными демоданными. Коммерческая эксплуатация и production-готовность не заявляются. Реальные платежи, банковские подключения и живая доставка Telegram не входят в подтверждённые сценарии.
