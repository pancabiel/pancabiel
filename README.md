# Gabriel Panca Ribeiro

Software engineer based in Blumenau, Brazil. I build full-stack web apps end-to-end, mostly Java/Spring on the backend and React on the frontend, and I like projects that start with a real person saying *"this is painful, can you make a tool for it?"*

## Featured projects

### 🍰 iCake: order management SaaS for home bakers · *closed source*

An order management app for small home-based confectioners, built after watching a family member juggle WhatsApp orders, ingredient lists, and delivery schedules on paper. **Currently being sold as a SaaS subscription, so the source is private.**

What's interesting under the hood: **schema-per-tenant** isolation so each baker's data lives in its own space, **custom landing pages for premium subscribers** so they can share a branded order page with their own customers, deployment on **AWS EC2 + S3**, and Flyway migrations, OpenAPI docs and Sentry for running it in production. Developed with **Claude Code** since early 2026.

`Java 25` · `Spring Boot` · `React` · `MySQL` · `Flyway` · `AWS EC2 + S3` · `Docker` · `GitHub Actions` · `Sentry`

### 🧭 Norte: management system for a travel agency · *closed source*

A management system built for a travel agency, in development since August 2026. **Client project, so the source is private.**

What's interesting under the hood: integration tests with **JUnit 5 and Testcontainers** against real PostgreSQL, CI and deploys through **GitHub Actions** to a Hetzner VPS, daily backups, Sentry for error tracking, and technical decisions recorded as **ADRs**.

`Java 25` · `Spring Boot` · `PostgreSQL` · `Flyway` · `JWT` · `React + Vite` · `Testcontainers` · `GitHub Actions` · `Sentry`

### 🏭 [ezcostura](https://github.com/pancabiel/ezcostura): production-tracking SaaS for clothing factories

A multi-tenant SaaS replacing paper-based shop-floor tracking for Brazilian clothing manufacturers. Operators register finished packs on a tablet that works offline and syncs when reconnected; owners get real-time per-operator and per-batch productivity reports.

What's interesting under the hood: **schema-per-tenant Postgres** with a routing DataSource, JWT tenant claims bridged from Reactor context to a per-request connection pool, and Flyway migrations run per-schema on boot. Offline-first PWA backed by IndexedDB with a background sync loop, so writes never block on the factory's flaky Wi-Fi.

`Java 21` · `Spring WebFlux` · `PostgreSQL` · `Flyway` · `React + Vite` · `TypeScript` · `Dexie` · `Workbox PWA`

### 🥗 [nutri](https://github.com/pancabiel/nutri): smart food tracker, built for myself

I got tired of typing every meal into nutrition apps, so I built a chat-style logger: I describe a meal in plain Portuguese or English, or snap a photo, and Claude parses it into structured nutrition data. It also reads packaged-food labels via the phone camera and remembers products I've logged before through semantic search.

What's interesting under the hood: **Quarkus + GraalVM native** compiled to a tiny AWS Lambda HTTP handler (sub-100ms cold starts), **pgvector** for semantic recall of previously-logged foods, and **Anthropic Claude** for both chat parsing and vision (meal photos and nutrition labels).

`Java 25` · `Quarkus` · `GraalVM native` · `AWS Lambda` · `React + Vite PWA` · `Supabase Postgres + pgvector` · `Anthropic Claude API`

## Tech I reach for

- **Backend:** Java (8 → 25), Spring Boot, Spring WebFlux, Quarkus, Hibernate, Flyway, JWT, GraalVM native
- **Frontend:** React, Angular, TypeScript, Vite, Tailwind, PWA / Workbox, IndexedDB / Dexie, Zustand
- **Data:** PostgreSQL (schema-per-tenant, pgvector), MySQL, Supabase
- **Infra:** Docker, GitHub Actions, AWS (EC2, S3, Lambda), Caddy, Hetzner Cloud, Sentry
- **Testing:** JUnit 5, Testcontainers
- **AI-assisted development:** Claude Code, Anthropic Claude API
- **Comfortable with:** multi-tenant architectures, offline-first sync, reactive backends, LLM/vision integrations, Jasper Reports, Java Swing

## Current role: Pública Tecnologia

Full Stack Java Developer working across both **desktop and web** platforms. The product is a public-sector management system used by **municipalities across many states of Brazil**, covering financial, accounting, fiscal, procurement, and administrative workflows.

Day-to-day:

- Refactoring large-scale accounting structures and public-sector procurement workflows.
- Designing and implementing new features and **integrations with Brazilian national banks and government systems**.
- Maintaining existing processes and building reports.
- Leading **code reviews** and providing technical guidance to the team to keep code quality high and aligned with engineering best practices.
- Together with three colleagues, responsible for the decisions, design and implementation of the **company's AI workflow with Claude Code**, and building internal applications to improve the company's processes.

`Java` · `Angular` · `JavaScript` · `Spring` · `Hibernate` · `Java Swing` · `Jasper Reports` · `MySQL` · `HQL` · `GitHub` · `Claude Code`

## Cool thing about my background

I represented Brazil at **WorldSkills 2019 in Kazan, Russia**, the international skills championships, finishing **4th of 27** in **Software Solutions for Business** and earning a **Medallion for Excellence**. Every test and all communication were in English.

📍 Blumenau, Brazil · Portuguese (native) & English (fluent)
🔗 [LinkedIn](https://www.linkedin.com/in/gabriel-panca-ribeiro-b864ba14b/)
