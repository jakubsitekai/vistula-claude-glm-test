# Presentation Topics – Web Application Development
**Course: Team Project – IT**

The purpose of this assignment is to independently explore an unfamiliar technical subject, evaluate reliable sources, understand how the technology works, and explain it clearly to other people. An IT engineer must be able to learn new technologies independently, verify examples and communicate technical knowledge. Follow the [assessment requirements](student-assessment-requirements.md).

## 1. Format and submission

**Basic (grade 3.0):** At least 40 minutes per team. A theoretical presentation is sufficient. Explain concepts, show examples (code snippets or diagrams are welcome), compare alternatives and explain common mistakes. A running application is not required.  
**Advanced (grades 4.0–5.0):** At least 120 minutes per team, including theory and a working application demonstration. The longer recording replaces the basic recording. Higher grade depends on technical depth and correctness, not duration alone. This is a mandatory graded lecture assignment, not the final lecture grade. To be eligible for any final lecture grade above 3.0 (including 3.5), students must earn at least 4.0 on this assignment, which requires the 120-minute track. The assignment significantly contributes to the final lecture grade; quizzes/tests and an examination (which may be oral; an individual oral assessment is mandatory for any final lecture grade above 3.0) remain separate requirements. Completing this assignment does not waive them or guarantee a higher final grade. The shared semester project also contributes to the final lecture grade; see the assessment requirements. If it meets the assigned presentation topic, the same application may be demonstrated. Exact weights and exam thresholds are to be announced.

### Repository and documentation requirements

See the [Presentation Repository Guide](presentation-repository-guide.md) for the required repository structure, README template, example architecture diagrams and submission checklist.

Each presentation must have its own GitHub repository. Submit the repository link in Platon. The repository must contain:

- `README.md`: presentation title/topic ID, authors and contributions, learning objectives, outline, link to the YouTube recording (unlisted is acceptable), links to all presentation materials, references and any demo projects.
- `presentation.pptx`: editable PowerPoint presentation with complete speaker notes for every narrated slide, matching the video. Optional: `presentation.pdf` as a convenient viewing copy; it does not replace the PPTX or notes.
- `doc/`: architecture diagrams where relevant and screenshots of working application/API, startup and representative operations for any practical demonstration.
- Source code for all demonstrated projects, in clearly named subdirectories when there is more than one.
- For each runnable project: prerequisites (JDK, framework/build tool versions), exact build/run/test commands, dependencies, configuration and example environment file without secrets, sample data or DB setup, expected output and example requests. Use Maven/Gradle wrapper where practical.
- For advanced work: describe architecture, API contract, persistence model, validation/error handling, automated tests and deployment or the approved local-only demo exception. Include URLs for hosted demos when required and screenshots showing actual execution, not AI-generated mockups.
- References to official documentation and third-party material; respect licences. No secrets or real personal data. Use demo data. No paid subscription or store account is compulsory.

Video may use human or AI narration. AI is allowed for slides, notes and code, but students are responsible for accuracy and reproducibility. Every demonstrated project must actually run from the submitted repository; generated code alone is not evidence. A clean checkout should be sufficient with the documented prerequisites.

### Assignment grading criteria

| Assignment grade | Requirements |
|---|---|
| 3.0 | At least 40 minutes; coherent, correct theoretical presentation; complete PPTX with notes, recording and README. Runnable application not required. |
| 4.0 | At least 120 minutes; all basic deliverables; working demonstrations specified by topic, clear architecture/code walkthrough, reproducible build/run instructions, screenshots and practical API examples. |
| 4.5 | All 4.0 requirements plus stronger technical explanation, meaningful tests, error scenarios, design tradeoffs and well-organized documentation. |
| 5.0 | All 4.5 requirements plus substantial topic-specific technical depth, reproducibility from clean checkout, useful automated verification and demonstrated extension or comparison. For application topics include practical SQL (schema, relation and queries); for framework comparison demonstrate all four implementations with identical contract, shared verification and a meaningful documented comparison; SQL can be an additional comparison example without requiring four databases. Explain limitations honestly. Real deployment where applicable and practical usefulness matter more than decorative slides. |

Duration is a mandatory threshold, not an automatic grade. The minimum assignment grade of 4.0 is a necessary, not sufficient, condition for a final lecture grade above 3.0. A paid store account or publication approval is never necessary. Each member should be able to explain their contribution and the demonstrated design; an individual oral examination is mandatory for a final lecture grade above 3.0.

### Suggested timing

| Module | Basic (40 min) | Advanced (120 min) |
|---|---:|---:|
| Introduction, learning objectives | 5 | 10 |
| Main technology and theory | 20 | 30 |
| Architecture and design choices | 10 | 20 |
| Code walkthrough, live/demo scenarios | optional | 35 |
| Deployment, testing, troubleshooting | optional | 15 |
| Summary, questions, references | 5 | 10 |

Time allocations are suggestions; total minimum is mandatory. Slides and notes should be reusable as real educational material; avoid padding. Demo can be recorded and must be reproducible.

## 2. Common advanced demo specification

Except for the dedicated framework comparison topic (A04), each advanced team builds a small but complete application around a chosen domain (tasks, events, book catalogue, expenses, inventory, courses). Use a Java backend framework suitable for REST (Spring Boot, Quarkus, Micronaut, Javalin, Jakarta REST) and a web or mobile frontend. Explain end-to-end request flow and persistence. A topic-specific emphasis is mandatory; don't just repeat the same general CRUD tutorial. For A04, four compact, independently runnable local REST API examples satisfy the demo scope: no four full-stack apps, no mandatory frontend, separate databases or four hosted deployments.

Common minimum: list/detail, create/update/delete, validation and error messages; relational model with two related entities for SQL topics; representative test data; clear API contract (example below); persistence across reload; at least one automated API test and documented manual scenario. Web advanced track: host frontend and Java API, use hosted database if useful. Hosting platform is free choice, no paid services required; lecturer-approved alternative if free hosting unavailable. On 5.0 demonstrate practical SQL (schema, relationship, queries or comparison), meaningful extension and deeper technical explanation. Supabase PostgreSQL via backend JDBC or API is acceptable; never expose database credentials/service role keys. For basic examples direct browser-to-Supabase REST with public publishable key and appropriate RLS on demo data is sufficient. NoSQL emphasis can use MongoDB or another suitable hosted document store.

Shared example contract (adapt resource name consistently): GET /api/tasks, GET /api/tasks/{id}, POST /api/tasks, PUT/PATCH /api/tasks/{id}, DELETE /api/tasks/{id}, GET /api/tasks?status=OPEN. JSON, 201/400/404/204 as appropriate, documented validation. Each team owns its domain and may choose equivalent endpoints. OpenAPI recommended for comparisons. Avoid needless two full systems: two clients may share one API, two backends may implement one contract, or one backend may switch persistence adapters.

## 3. Ten basic topics – 40-minute theoretical presentations

| ID | Title | Required modules and examples |
|---|---|---|
| B01 | How Web Applications Work: HTML, CSS, JavaScript | Browser/server, DOM, events, forms, fetch, HTTP request/response, simple task list example. |
| B02 | HTTP, REST and JSON | URLs, methods, status codes, headers, JSON, CRUD API examples, client/server flow and error handling. |
| B03 | MVC and Layered Architecture | Model/view/controller, service/repository, separation of concerns, diagram and Java CRUD request walkthrough. |
| B04 | Relational Databases and SQL | Tables, primary/foreign keys, 1:N, SELECT/INSERT/UPDATE/DELETE, JOIN, transactions; tasks/categories schema. |
| B05 | Supabase and Backend-as-a-Service | PostgreSQL, generated REST, publishable keys, RLS, GitHub Pages, JS fetch, demo architecture without custom Java server. |
| B06 | Angular Fundamentals | Components, templates, services, dependency injection, routing, forms, HttpClient; task form examples. |
| B07 | React Fundamentals | Components, props, state, hooks, forms, router, fetching and rendering tasks; loading/error examples. |
| B08 | Java Backend Frameworks | Spring Boot, Quarkus, Micronaut, Javalin concepts; routing, JSON, dependency injection, simple REST handler and comparison. |
| B09 | SQL vs NoSQL | Relational vs document modelling, SQL JOIN vs embedding/references, MongoDB examples, consistency, tradeoffs. |
| B10 | Mobile and Cross-Platform Development | Native Android/iOS vs Flutter/React Native, REST clients, emulator, builds, signing, testing and store publication stages. |

## 4. Fourteen advanced topics – 120-minute presentations and tutorials

### A01 – MVC and Server-Side Java Web Applications
**Focus:** architecture, MVC, service and repository layers, DTO vs entity.  
**Theory:** request lifecycle, MVC vs REST, dependency injection, validation, persistence and error handling.  
**Demo:** Library or customer manager, Java Spring Boot + Thymeleaf/Vaadin or equivalent, PostgreSQL, form validation, list/detail/edit/delete; expose JSON REST endpoints alongside UI. Show controller → service → repository → DB; explain why responsibilities are separated; deploy Java app and demonstrate an invalid request.  
**Stretch:** unit/integration tests, transactions, compare server-side UI to SPA.

### A02 – Angular Frontend with a Java REST Backend
**Focus:** Angular components, services, DI, reactive forms, router, HttpClient, observable/error handling.  
**Demo:** event registration or task manager, Angular + Java REST API + PostgreSQL. List, detail, form, filters, validation, asynchronous loading; inspect network requests. Show build/deploy frontend and backend; refresh route and demonstrate persistence.  
**Stretch:** component tests, accessibility, compare imperative and reactive flows.

### A03 – React Frontend with a Java REST Backend
**Focus:** components, props, state, hooks, effects, controlled forms, routing, API client and error states.  
**Demo:** same general CRUD domain as A02 is acceptable but React must be the main tutorial. React/Vite + Java REST API + SQL. Demonstrate loading, editing, updating state after mutation, navigation and hosted deployment.  
**Stretch:** compare React and Angular with the same backend, test UI, avoid stale data.

### A04 – Java REST Frameworks Compared: Spring Boot, Quarkus, Micronaut and Javalin
**Focus:** a comparative tutorial with more theory and four small runnable examples, not four elaborate applications.  
**Theory:** what a REST framework provides, project creation and dependencies, routes/controllers, JSON serialization, request validation, dependency injection or explicit wiring, error handling, configuration, testing and packaging. Explain differences in programming models and typical use cases.  
**Demo:** use the same small Task or Book API in four projects under `examples/spring-boot/`, `examples/quarkus/`, `examples/micronaut/`, `examples/javalin/`. Each supports GET list, GET by ID, POST, PUT/PATCH and DELETE with JSON, input validation, 400/404 and suitable success codes. In-memory storage is sufficient; no frontend, four separate databases or four hosted deployments required. Use the same test data, request examples and contract. Each project must actually build and run, with its own README or clearly separated instructions in the top-level README. Show startup, requests and responses for all four; use distinct ports or start them sequentially.  
**Stretch/5.0:** reusable HTTP contract test suite or script run against all four, packaging and configuration comparison, optional shared SQL example, evidence-based observations on implementation size and startup under documented comparable conditions. No unsupported performance rankings.  
**Suggested 120 min:** 15 min REST/framework basics, 20 min for each of four frameworks, 15 min comparative discussion/testing, 10 min summary.

### A05 – PostgreSQL, SQL and Persistence in Java
**Focus:** relational schema, PK/FK, JOIN, indexes, transactions, migrations, JDBC/JPA/Hibernate and query tradeoffs.  
**Demo:** order/products or tasks/categories with real 1:N relation, Java REST, form-based UI. Create schema, seed, CRUD, joined list and aggregate stats. Demonstrate query, constraints, persistence and rollback or error case; host API and DB.  
**Stretch:** compare JDBC and ORM, explain N+1, EXPLAIN a query.

### A06 – Document Databases and SQL vs NoSQL
**Focus:** modelling documents vs relations, embedding/references, indexing, querying, consistency.  
**Demo:** product catalogue or notes, Java REST backend + MongoDB/other document store and comparison SQL implementation (separate adapters or backend variants using same API). UI should remain compatible. Show comparable query and update, hosted API and DB; demonstrate tradeoffs rather than claiming one is universally better.  
**Stretch:** swap persistence adapter without changing API, compare constraints and transactions. Practical SQL comparison supports 5.0 requirement.

### A07 – Cloud Hosting and Backend-as-a-Service
**Focus:** static hosting, BaaS vs custom backend, REST, RLS, authentication boundary, environment/config, CORS, TLS.  
**Demo:** deploy basic HTML/JS or Angular/React + Supabase directly as one architecture, and Java REST backend + SQL as second architecture for advanced track. Show same task management functionality, compare request paths/security and where secrets belong; demo error handling.  
**Stretch:** deployment automation, compare hosted PostgreSQL via JDBC vs generated Supabase REST.

### A08 – Authentication, Authorization and Secure Web Forms
**Focus:** identity vs permissions, password handling, sessions/tokens, backend enforcement, RLS, validation, common web security pitfalls.  
**Demo:** personal tasks or reservations with demo accounts, Java REST backend and SQL, Angular/React/other frontend. Login, CRUD restricted to owner, show unauthorized/forbidden request, no hardcoded credentials. Deploy and verify access controls.  
**Stretch:** role-based access, integration tests, token expiry; use managed auth if appropriate, do not implement custom cryptography.

### A09 – Testing, CI/CD and Deployment of Java Web Applications
**Focus:** unit/integration/E2E, Git branches/PR review, pipelines, Docker, environment config, logs and reproducible release.  
**Demo:** Java REST CRUD + SQL + frontend, build/test via GitHub Actions, one intentional failing test and fix, Docker or equivalent packaging, hosted web and API; show versioned build and rollback strategy.  
**Stretch:** contract test, database migration test, frontend E2E; no production secrets in repo.

### A10 – Cross-Platform Mobile Applications: Android and iOS
**Focus:** native vs cross-platform, Flutter/React Native or other framework, REST, forms, app lifecycle, signing, build/release, store review and privacy.  
**Demo:** mobile client for task/event/catalogue service backed by Java REST + SQL; list/form/edit, persistent server data, API error, run Android emulator/device. Demonstrate iOS simulator/device if accessible, otherwise document platform-specific steps and limitations; shared code and API contract. Show Android APK/AAB build, iOS Xcode archive or documented build path, store listing/checklist, internal testing/TestFlight procedure, optional real distribution on authorized account.  
**Stretch:** both builds or test distribution, mobile/web shared backend, sandbox payments if relevant. Do not require buying Play/Apple developer account or Mac; equivalent reproducible demonstration acceptable. Public store approval is not a grading prerequisite.

### A11 – Spring Boot: Building a Complete REST Application
**Focus:** Spring Boot, Spring MVC REST, IoC/DI, auto-configuration, Spring Data and testing.  
**Theory modules:** create a project, Maven/Gradle dependencies and starters; application properties/profiles; `@RestController`, request mapping and DTOs; constructor injection, service/repository; Bean Validation and exception handling; JPA/JDBC and transactions; test and deploy.  
**Demo:** customer/order or task/category manager with SQL (PostgreSQL or Supabase PostgreSQL), Java Spring Boot REST API, simple HTML/JS or SPA with forms. Full CRUD, related records, filter, validation, 400/404, REST requests, database persistence. Show logs and trace controller → service → repository; run automated API tests and hosted Java/API demo.  
**Stretch/5.0:** migrations, transaction use case, structured error responses, integration tests against real/test SQL database, explain auto-configuration and test boundaries.

### A12 – Quarkus: Building and Deploying a Java REST Application
**Focus:** Quarkus extensions, Jakarta REST, CDI, configuration, development mode and deployment.  
**Theory modules:** bootstrap and dependencies, dev mode, resource class and JSON, CDI service wiring, validation/error mapping, Hibernate ORM/Panache or JDBC, database config, tests, JVM/native packaging concepts.  
**Demo:** inventory/products and categories, Quarkus REST API + PostgreSQL, form-based web client; CRUD, filter, relation, validation, API error, persistence, automated API tests; package and deploy Java runtime.  
**Stretch/5.0:** migration, transaction, profiles and integration tests; explain JVM vs native build tradeoffs, optional native build if environment supports it (not mandatory).

### A13 – Micronaut: Building a Java REST Application
**Focus:** compile-time DI, HTTP routing, configuration, serialization, Micronaut Data and test tooling.  
**Theory modules:** project creation, dependencies/annotation processing, `@Controller`, constructor injection, DTOs/JSON, validation and errors, repository and SQL, HTTP client, testing, packaging/deployment.  
**Demo:** course registration or library catalogue, Micronaut REST API + PostgreSQL, simple frontend forms; CRUD, relations, filter, error handling and persistence. Show generated build artifacts or explain compile-time wiring, run API tests and deploy.  
**Stretch/5.0:** integration tests, configuration environments, migration and transaction, compare compile-time injection conceptually with Spring; don't assert performance benefits without measurement.

### A14 – Javalin: Building a Lightweight Java REST Application
**Focus:** explicit routes and handlers, minimal framework, JSON, service separation and manual dependency wiring.  
**Theory modules:** create Maven/Gradle Java project, Javalin server startup, HTTP context and route handlers, serialization, DTO validation, error handlers, service/repository construction, JDBC/connection management, tests and packaging.  
**Demo:** book catalogue or expense manager, Javalin REST API + PostgreSQL and simple HTML/JS forms. Full CRUD, related records, filters, meaningful status codes and persistent data; compare raw handlers to separated service/repository. Test requests and host Java API.  
**Stretch/5.0:** connection pooling, migrations, transaction and API integration tests; explain what the framework does and what must be supplied explicitly, compare with annotation-driven frameworks.

For all four dedicated framework presentations, the framework itself is the central learning topic. Demonstrate the path from an empty project to a runnable REST service before expanding it into the complete application. A short frontend is sufficient; spend the bulk of the tutorial on backend decisions, code, database, API verification and deployment.

Official framework documentation: [Spring Boot](https://docs.spring.io/spring-boot/), [Quarkus](https://quarkus.io/guides/), [Micronaut](https://docs.micronaut.io/), [Javalin](https://javalin.io/documentation).

## 5. Deployment notes and references

- Angular and React client-side SPAs can run on GitHub Pages. Angular build must use the correct project base href; React/Vite set base to /REPO/ for project Pages. Use hash routing (Angular withHashLocation; React HashRouter) or explicitly handle static-host deep links; GitHub Pages is not a Java/Node server and does not provide a general SPA rewrite. Publish built assets rather than raw source.
- Java API must run on separate server/container hosting for advanced web track. Students may choose a suitable free-tier service or approved alternative; verify quotas and cold starts before requiring any specific service. SQL/NoSQL can be hosted independently. Configure CORS correctly.
- Mobile: Google Play internal testing still needs a developer account; Android APK emulator/device demo can be done without one. Apple free Xcode personal-team testing has limitations; TestFlight/App Store distribution requires appropriate membership. Accredited educational institutions may be eligible for Apple fee waiver. Do not require personal payment. Use test tracks/sandbox, not real payment transactions.
- Official references: [Angular deployment](https://angular.dev/tools/cli/deployment), [Angular routing](https://angular.dev/guide/routing/router-reference), [Vite static deploy](https://vite.dev/guide/static-deploy), [Google Play testing](https://support.google.com/googleplay/android-developer/answer/9845334), [Apple membership](https://developer.apple.com/help/account/membership/programs-overview/), [Apple enrolment](https://developer.apple.com/help/account/membership/program-enrollment).

## 6. Topic allocation and team work

The lecturer will assign topics to students or teams. A separate allocation list will be provided. Do not assume that every team must cover every topic. The same assigned subject can be addressed at basic or advanced depth; confirm the appropriate specification with the lecturer if necessary.

Work in pairs unless a different arrangement is approved. Prepare one coherent presentation per team, with clearly identified contributions. You may cover complementary technologies in the same presentation (e.g. two frontends using a common API, or two persistence implementations). If assigned subjects overlap or conflict after forming a team, ask the lecturer to confirm the final topic. Do not create multiple full presentations unless explicitly instructed.

Choose the topic-specific examples, explain the whole architecture at an overview level, and focus on the assigned technology. Keep the demonstrations reproducible. A topic assignment is not a requirement to purchase any software or developer account.
