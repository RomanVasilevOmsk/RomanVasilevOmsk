<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./assets/banner-dark.svg">
    <img width="100%" alt="Roman Vasilev — Senior Frontend Engineer, React and TypeScript" src="./assets/banner-light.svg">
  </picture>
</p>

<p align="center">
  <b>Senior Frontend Engineer · React / TypeScript · AI-assisted development</b><br>
  10+ years building product frontends — travel-tech, fintech, gov-tech
</p>

<p align="center">
  <samp>
    <a href="https://www.linkedin.com/in/roman-vasilev-1742191b8">linkedin</a> .
    <a href="https://t.me/don_macron">telegram</a> .
    <a href="mailto:zvezdarusy@gmail.com">email</a> .
    <a href="#english">english</a> .
    <a href="#русский">русский</a>
  </samp>
</p>

---

## English

### About

> Senior frontend engineer and feature lead. Right now I build a corporate travel platform —
> flights, rail and hotels for business clients — as a React 19 SPA in a pnpm + Turborepo
> monorepo. Over the past year I've also built an **AI harness on Claude Code** around that
> codebase: agents, skills, hooks and a local knowledge base the team uses to take a task from
> ticket to merge request.

### Stack

<p>
  <img alt="TypeScript, React, Redux, Vite, Node.js, Express, pnpm, Less, Vitest, Jest, Webpack, Next.js, Git, GitLab, Docker, Figma" src="https://skillicons.dev/icons?i=ts,react,redux,vite,nodejs,express,pnpm,less,vitest,jest,webpack,nextjs,git,gitlab,docker,figma&perline=16">
</p>

| Area              | Tools                                                                                                  |
| ----------------- | ------------------------------------------------------------------------------------------------------ |
| **Core**          | TypeScript · React 19 · Redux Toolkit / RTK Query · React Router · Mantine · i18next · Yup             |
| **Build**         | Vite · Webpack · pnpm workspaces · Turborepo · ESLint · Prettier · Husky + commitlint                  |
| **Quality**       | Playwright e2e (payments, 3DS) · Vitest · Jest / RTL · Storybook (340+ stories) · pixel-diff snapshots |
| **Server**        | Node.js · Express (static + API proxy) · WebSockets                                                    |
| **Observability** | LogRocket — weekly production-error triage turned into tickets                                         |
| **AI**            | Claude Code · Codex · Cursor · MCP · multi-agent pipelines · retrieval over docs                       |

### AI harness for a frontend team

Not "ask a chatbot, paste the code" — engineering scaffolding that lives in the repo and works the
same for everyone on the team.

| Layer            | What's inside                                                                                                                                                                 |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Agents**       | `arch` → `coder` → `reviewer` chain (ticket → plan → implementation → review), plus `debug`, `debug-fix`, `e2e`. One `/dev` command runs the whole chain                      |
| **Skills (34)**  | The codebase's conventions as executable instructions: RTK Query, Redux slices, DTOs and parsers, forms, error handling, i18n, routing, permissions, payments, Storybook, e2e |
| **Code review**  | One rulebook (severity, finding anatomy, verify-before-confirming) with two entry points: local self-check and GitLab MR review with a preview before anything is posted      |
| **Hooks**        | Type-check after edits, ticket detection in prompts, automatic Jira transitions, commit guard                                                                                 |
| **MCP**          | Jira / Confluence, GitLab, Figma, Playwright, LogRocket, Context7, Mantine docs                                                                                               |
| **Setup**        | One command checks the environment (tools, tokens, MCP servers, stale config) and pulls the knowledge bases                                                                   |
| **Test tooling** | HTTP interceptor to record/replay API traffic and run offline · visual probes (pixel-diff of Storybook and pages) · Chrome extension for routing to test stands               |

#### Retrieval over documentation

Agents don't guess API contracts — they read them. No vector DB: an agent-navigated Markdown
knowledge graph, which turned out more precise for spec lookup than embeddings.

```
Confluence (600+ spec pages)  ──sync──▶  Obsidian vault: Markdown + YAML frontmatter
                                           │  domain taxonomy: avia / hotel / rail / order / auth / api …
                                           │  ingest pass: [[wikilink]] graph between pages (LLM-wiki pattern)
                                           ▼
Architecture docs  ─────────mirror───▶  service map, routing, HTTP / message-queue maps
200+ backend repos ───────inventory──▶  "entity → service → shared-types contract" routing
                                           ▼
          arch agent: pick domain → search → read → follow links → plan with cited sources
```

Incremental sync, a map compiled from frontmatter, vault linting, `bats` tests for the scripts.

### Experience

| When        | Where                                                       | What                                                                                                                                                                                                                                                 |
| ----------- | ----------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 2024 → now  | **Aero Club** — business travel (gate.ru, anywayanyday.com) | Senior Frontend / R&D. Moved the app to a pnpm + Turborepo monorepo; booking and payment flows (overdraft, deposit, card), travel policies, add-on services, unified auth migration, AI harness                                                      |
| 2021 – 2024 | **SoftMediaLab**                                            | Senior Frontend. Lead frontend on a payments platform (cushion.ai): real-time WebSocket dashboards, LCP −35%, 5 payment providers. Frontend architecture for a utility customer portal and a regional social-card service (WCAG 2.1, 2FA, 3 locales) |
| 2021        | **Channex.io**                                              | Frontend. SaaS channel manager for apartment owners: calendars, booking lists, dashboards, Booking.com / Airbnb integrations                                                                                                                         |

---

## Русский

### Обо мне

> Senior frontend-разработчик и фича-лид. Сейчас делаю корпоративную платформу деловых
> поездок — авиа, ЖД и отели для бизнес-клиентов — SPA на React 19 в pnpm + Turborepo-монорепо.
> Последний год строю вокруг этой кодовой базы **AI-харнесс на Claude Code**: агенты, скиллы,
> хуки и локальную базу знаний, через которые команда ведёт задачу от тикета до мерж-реквеста.

### Стек

| Область           | Инструменты                                                                                          |
| ----------------- | ---------------------------------------------------------------------------------------------------- |
| **Основа**        | TypeScript · React 19 · Redux Toolkit / RTK Query · React Router · Mantine · i18next · Yup           |
| **Сборка**        | Vite · Webpack · pnpm workspaces · Turborepo · ESLint · Prettier · Husky + commitlint                |
| **Качество**      | Playwright e2e (оплаты, 3DS) · Vitest · Jest / RTL · Storybook (340+ стори) · попиксельное сравнение |
| **Сервер**        | Node.js · Express (статика + API-прокси) · WebSockets                                                |
| **Наблюдаемость** | LogRocket — еженедельный разбор прод-ошибок в задачи                                                 |
| **AI**            | Claude Code · Codex · Cursor · MCP · мультиагентные пайплайны · поиск по документации                |

### AI-харнесс для фронтенд-команды

Не «спросил чат — вставил код», а инженерная обвязка, которая живёт в репозитории и одинаково
работает у всей команды.

| Слой                 | Что внутри                                                                                                                                                      |
| -------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Агенты**           | Цепочка `arch` → `coder` → `reviewer` (тикет → план → реализация → ревью), плюс `debug`, `debug-fix`, `e2e`. Команда `/dev` гоняет цепочку целиком              |
| **Скиллы (34)**      | Конвенции кодовой базы как исполняемые инструкции: RTK Query, Redux-слайсы, DTO и парсеры, формы, обработка ошибок, i18n, роуты, права, оплаты, Storybook, e2e  |
| **Ревью**            | Единый свод правил (severity, анатомия замечания, verify-before-confirming) и два входа: локальный self-check и ревью GitLab MR с превью перед публикацией      |
| **Хуки**             | Тип-чек после правок, распознавание тикета в промпте, автопереходы задач в Jira, защита коммитов                                                                |
| **MCP**              | Jira / Confluence, GitLab, Figma, Playwright, LogRocket, Context7, документация Mantine                                                                         |
| **Настройка**        | Одна команда проверяет окружение (инструменты, токены, MCP, отставание конфигов) и подтягивает базы знаний                                                      |
| **Тестовая обвязка** | HTTP-интерсептор для записи и реплея API и работы оффлайн · визуальные пробы (попиксельно Storybook и страницы) · Chrome-расширение для маршрутизации на стенды |

#### Поиск по документации

Агенты не угадывают контракты API, а читают их. Без векторной базы: граф знаний на Markdown, по
которому ходит агент, — для поиска по спецификациям это оказалось точнее эмбеддингов.

```
Confluence (600+ страниц спек)  ──sync──▶  Obsidian-vault: Markdown + YAML frontmatter
                                             │  доменная таксономия: avia / hotel / rail / order / auth / api …
                                             │  ingest: граф [[wikilinks]] между страницами (паттерн LLM-wiki)
                                             ▼
Архитектурная документация  ───mirror───▶  карта сервисов, роутинг, HTTP- и очереди
200+ бэкенд-репозиториев   ──inventory──▶  маршрут «сущность → сервис → контракт shared-types»
                                             ▼
           arch-агент: домен → поиск → чтение → проход по ссылкам → план со ссылками на источники
```

Инкрементальная синхронизация, карта из frontmatter, линтер базы, `bats`-тесты на скрипты.

### Опыт

| Когда         | Где                                                        | Что                                                                                                                                                                                                                                                    |
| ------------- | ---------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 2024 → сейчас | **Аэро Клуб** — деловой туризм (gate.ru, anywayanyday.com) | Senior Frontend / R&D. Перевёл проект в pnpm + Turborepo-монорепо; оформление и оплата заказов (овердрафт, депозит, карта), тревел-политики, докупка услуг, миграция на единую авторизацию, AI-харнесс                                                 |
| 2021 – 2024   | **СофтМедиаЛаб**                                           | Senior Frontend. Ведущий фронтенд платёжного сервиса (cushion.ai): real-time дашборды на WebSockets, LCP −35%, 5 платёжных провайдеров. Фронтенд-архитектура личного кабинета энергосбыта и сервиса «Единая социальная карта» (WCAG 2.1, 2FA, 3 языка) |
| 2021          | **Channex.io**                                             | Frontend. SaaS-агрегатор бронирований для владельцев апартаментов: календари, списки броней, дашборды, интеграции с Booking.com и Airbnb                                                                                                               |
