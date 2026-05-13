# Gabriel Panca Ribeiro

Software engineer based in Blumenau, Brazil. I build full-stack web apps end-to-end — mostly Java/Spring on the backend and React on the frontend — and I like projects that start with a real person saying *"this is painful, can you make a tool for it?"*

## Featured projects

### 🍰 iCake — order management SaaS for home bakers · *closed source*

An order management app for small home-based confectioners, built after watching a family member juggle WhatsApp orders, ingredient lists, and delivery schedules on paper. **Currently being sold as a SaaS subscription, so the source is private.**

What's interesting under the hood: **schema-per-tenant** isolation so each baker's data lives in its own space, **custom landing pages for premium subscribers** so they can share a branded order page with their own customers, and deployment on **AWS EC2 + S3**.

`Java` · `Spring Boot` · `React` · `MySQL` · `AWS EC2 + S3` · `Docker` · `GitHub Actions`

### 🏭 [ezcostura](https://github.com/pancabiel/ezcostura) — production-tracking SaaS for clothing factories

A multi-tenant SaaS replacing paper-based shop-floor tracking for Brazilian clothing manufacturers. Operators register finished packs on a tablet that works offline and syncs when reconnected; owners get real-time per-operator and per-batch productivity reports.

What's interesting under the hood: **schema-per-tenant Postgres** with a routing DataSource, JWT tenant claims bridged from Reactor context to a per-request connection pool, and Flyway migrations run per-schema on boot. Offline-first PWA backed by IndexedDB with a background sync loop, so writes never block on the factory's flaky Wi-Fi.

`Java 21` · `Spring WebFlux` · `PostgreSQL` · `Flyway` · `React + Vite` · `TypeScript` · `Dexie` · `Workbox PWA`

### 🥗 [nutri](https://github.com/pancabiel/nutri) — smart food tracker, built for myself

I got tired of typing every meal into nutrition apps, so I built a chat-style logger: I describe a meal in plain Portuguese or English, or snap a photo, and Claude parses it into structured nutrition data. It also reads packaged-food labels via the phone camera and remembers products I've logged before through semantic search.

What's interesting under the hood: **Quarkus + GraalVM native** compiled to a tiny AWS Lambda HTTP handler (sub-100ms cold starts), **pgvector** for semantic recall of previously-logged foods, and **Anthropic Claude** for both chat parsing and vision (meal photos and nutrition labels).

`Java 25` · `Quarkus` · `GraalVM native` · `AWS Lambda` · `React + Vite PWA` · `Supabase Postgres + pgvector` · `Anthropic Claude API`

## Tech I reach for

- **Backend** — Java (8 → 25), Spring Boot, Spring WebFlux, Quarkus, Hibernate, Flyway, JWT, GraalVM native
- **Frontend** — React, Angular, TypeScript, Vite, Tailwind, PWA / Workbox, IndexedDB / Dexie, Zustand
- **Data** — PostgreSQL (schema-per-tenant, pgvector), MySQL, Supabase
- **Infra** — Docker, GitHub Actions, AWS (EC2, S3, Lambda), Caddy, Hetzner Cloud
- **Comfortable with** — multi-tenant architectures, offline-first sync, reactive backends, LLM/vision integrations, Jasper Reports, Java Swing

## Current role — Publica Tecnologia

Full Stack Java Developer working across both **desktop and web** platforms. The product is a public-sector management system used by **municipalities across many states of Brazil**, covering financial, accounting, fiscal, procurement, and administrative workflows.

Day-to-day:

- Refactoring large-scale accounting structures and public-sector procurement workflows.
- Designing and implementing new features and **integrations with Brazilian national banks and government systems**.
- Maintaining existing processes and building reports.
- Leading **code reviews** and providing technical guidance to the team to keep code quality high and aligned with engineering best practices.

`Java` · `Angular` · `JavaScript` · `Spring` · `Hibernate` · `Java Swing` · `Jasper Reports` · `MySQL` · `HQL` · `GitHub`

## Cool thing about my background

I represented Brazil at **WorldSkills 2019 in Kazan, Russia** — the international skills championships — competing in **Software Solutions for Business**.

📍 Blumenau, Brazil · Portuguese & English
🔗 [LinkedIn](https://www.linkedin.com/in/gabriel-panca-ribeiro-b864ba14b/)
