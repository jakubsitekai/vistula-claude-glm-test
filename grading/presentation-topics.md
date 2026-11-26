# Presentation Topics – Web and AI Application Development
**Course: Team Project – IT**

The purpose of this assignment is to independently explore an unfamiliar technical subject, evaluate reliable sources, understand how the technology works, and explain it clearly to other people. An IT engineer must be able to learn new technologies independently, verify examples and communicate technical knowledge. Follow the [assessment requirements](student-assessment-requirements.md).

## 1. Format and submission

**Basic (grade 3.0):** At least 40 minutes per team. A theoretical presentation is sufficient. Explain concepts, show examples (code snippets or diagrams are welcome), compare alternatives and explain common mistakes. A running application is not required.  
**Advanced (grades 4.0–5.0):** At least 120 minutes per team, including theory and a working application demonstration. The longer recording replaces the basic recording. Higher grade depends on technical depth and correctness, not duration alone. This is a mandatory graded lecture assignment, not the final lecture grade. For a final lecture grade of 4.0 or higher, students must earn at least 4.0 on this assignment, which requires the 120-minute track. A presentation graded 3.0 is sufficient for eligibility for a final lecture grade of 3.0 or 3.5. The assignment significantly contributes to the final lecture grade; quizzes/tests and examination remain separate requirements. For final grades above 3.5, individual practical assessment without AI assistance is required; an oral assessment may also be required. Completing this assignment does not waive them or guarantee a higher final grade. The shared semester project also contributes to the final lecture grade; see the assessment requirements. If it meets the assigned presentation topic, the same application may be demonstrated. Passing Laboratory is required to pass Lecture. The semester project must be publicly deployed for final grades above 3.5; see the assessment requirements.

### Repository and documentation requirements

See the [Presentation Repository Guide](presentation-repository-guide.md) for the required repository structure, README template, example architecture diagrams and submission checklist.

Each presentation must have its own GitHub repository. Submit the repository link in Platon. The repository must contain:

- `README.md`: presentation title/topic ID, authors and contributions, learning objectives, outline, link to the YouTube recording (unlisted is acceptable), links to all presentation materials, references and any demo projects.
- `presentation.pptx`: editable PowerPoint presentation with complete speaker notes for every narrated slide, matching the video. Optional: `presentation.pdf` as a convenient viewing copy; it does not replace the PPTX or notes.
- `doc/`: architecture diagrams where relevant and screenshots of working application/API, startup and representative operations for any practical demonstration.
- Source code for all demonstrated projects, in clearly named subdirectories when there is more than one.
- For each runnable project: prerequisites (JDK or Python runtime, framework/build tool versions), exact build/run/test commands, dependencies, configuration and example environment file without secrets, sample data or DB setup, expected output and example requests. Use Maven/Gradle wrapper where practical.
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

Duration is a mandatory threshold, not an automatic grade. The minimum assignment grade of 4.0 is a necessary, not sufficient, condition for a final lecture grade of 4.0 or higher. A paid store account or publication approval is never necessary. Each member should be able to explain their contribution and the demonstrated design; an oral assessment may be required for a final lecture grade above 3.5.

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

Except for the dedicated comparison topics (A04 and A24), each advanced team builds a small but complete application around a chosen domain (tasks, events, book catalogue, expenses, inventory, courses). For web topics A01–A14, use a Java backend framework suitable for REST (Spring Boot, Quarkus, Micronaut, Javalin, Jakarta REST) and a web or mobile frontend. For AI topics A15–A24, use Java or Python as specified by the topic, with a REST backend and suitable frontend; A24 has a compact comparison exception. Explain end-to-end request flow and persistence. A topic-specific emphasis is mandatory; don't just repeat the same general CRUD tutorial. For A04, four compact, independently runnable local REST API examples satisfy the demo scope: no four full-stack apps, no mandatory frontend, separate databases or four hosted deployments.

Common minimum: list/detail, create/update/delete, validation and error messages; relational model with two related entities for SQL topics; representative test data; clear API contract (example below); persistence across reload; at least one automated API test and documented manual scenario. Web advanced track: host frontend and backend API, use hosted database if useful. Hosting platform is free choice, no paid services required; lecturer-approved alternative if free hosting unavailable. On 5.0 demonstrate practical SQL (schema, relationship, queries or comparison), meaningful extension and deeper technical explanation. Supabase PostgreSQL via backend JDBC or API is acceptable; never expose database credentials/service role keys. For basic examples direct browser-to-Supabase REST with public publishable key and appropriate RLS on demo data is sufficient. NoSQL emphasis can use MongoDB or another suitable hosted document store.

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

## 5. Optional AI presentation topics (A15–A24)

All ten AI subjects are available in two versions: a **40-minute theoretical presentation** (assignment grade 3.0) or a **120-minute presentation with working practical examples** (assignment grades 4.0–5.0). The basic version covers the theory modules and illustrative examples without requiring a runnable application. The advanced version covers theory, architecture, code, actual demonstrations and verification. Use a Java or Python backend unless the topic specifies a particular language. The normal documentation, grading and individual assessment rules apply.

You may reuse your semester project when it matches the assigned subject. No paid AI API, dedicated GPU or custom model training is compulsory. Use an appropriate local or available hosted model, document the model and configuration, and demonstrate an actual working AI feature. Keep credentials server-side, use permitted demo data, validate outputs and handle errors. Tests may use mocks to be repeatable; the actual demonstration must use a real model. For application-oriented topics targeting 5.0, include the common practical SQL requirement. A24 is a framework comparison and may use compact examples, with SQL as an optional extension.

### A15 – Building LLM-Powered Applications in Java
**Focus:** integrating language models into Java applications with Spring AI or LangChain4j.  
**Theory:** LLM APIs, messages, model configuration, prompt templates, temperature, structured responses, service boundaries, secrets, error handling and testing.  
**Demo:** Java REST service and frontend generating quiz questions or task suggestions. Validate output, persist results, allow user edits, show actual model response and API failures; document model setup and test with a fake provider.  
**Stretch/5.0:** schema-validated output, SQL history, provider abstraction and repeatable evaluation.

### A16 – Building LLM-Powered Applications in Python
**Focus:** Python-based LLM integration, FastAPI/Flask/Django and a model SDK or suitable framework.  
**Theory:** HTTP and model clients, prompt construction, response models, validation, synchronous/asynchronous requests, environment configuration and tests.  
**Demo:** document summariser or task assistant with REST endpoints, simple frontend, persistent history, validated model outputs and error handling. Demonstrate clean setup with pinned dependencies.  
**Stretch/5.0:** SQL persistence, provider-independent service, testable response schemas, timeout handling and evaluation.

### A17 – Retrieval-Augmented Generation (RAG)
**Focus:** answering questions using retrieved information.  
**Theory:** ingestion, text extraction, chunking, embeddings, vector retrieval, context construction, citations, hallucinations and retrieval limitations.  
**Demo:** AI Document Assistant with permitted demo documents, ingestion and query API, search and answer UI, persisted documents and source references. Demonstrate supported and unanswerable queries.  
**Stretch/5.0:** compare chunk sizes or retrieval strategies, measure retrieval quality and groundedness on a fixed question set, SQL metadata.

### A18 – Embeddings and Vector Databases
**Focus:** semantic similarity and vector search.  
**Theory:** embedding models, vectors, cosine similarity, distance metrics, indexing, metadata filters and keyword versus semantic search.  
**Demo:** semantic book catalogue with CRUD, embedding generation, PostgreSQL/pgvector (or suitable vector store), search API and frontend. Compare keyword and semantic results using a small reproducible test set.  
**Stretch/5.0:** SQL joins/filters, hybrid search, precision at k, measured indexing or query tradeoffs.

### A19 – AI Agents and Tool Calling
**Focus:** model-driven function calls, orchestration and controlled actions.  
**Theory:** tools and schemas, model/tool interaction, execution loop, error handling, permission boundaries, prompt injection and human approval.  
**Demo:** task assistant with read-only lookup tools and an explicitly confirmed task-creation action through the application's API. Persist actions and results; show rejected invalid tool calls and safe handling of untrusted text.  
**Stretch/5.0:** SQL audit log, bounded execution, approval workflow, tests for malformed tool calls and unauthorized actions. Do not connect real financial or destructive operations.

### A20 – Running AI Models Locally
**Focus:** local model inference and application integration.  
**Theory:** open-weight models and licences, inference runtimes (e.g. Ollama or llama.cpp), quantization, memory requirements, context, privacy, latency and API compatibility.  
**Demo:** local model exposed via an API, connected to a Java/Python REST application and simple UI with saved requests/results. Document hardware and model selection, demonstrate real inference, handle unavailable runtime. A suitable approved shared local runtime is acceptable.  
**Stretch/5.0:** compare two model configurations on the same hardware and dataset, measure response quality/latency, SQL request history.

### A21 – Structured Output and Prompt Engineering
**Focus:** reliable machine-readable model output.  
**Theory:** prompt structure, examples, delimiters, schema design, JSON validation, retries, failure modes and untrusted input.  
**Demo:** quiz generator or task extractor returning structured JSON, validated on the backend before saving; editable frontend, configurable number/category of results and error cases.  
**Stretch/5.0:** SQL persistence, schema comparison, test corpus, measure valid-output rate and semantic accuracy separately.

### A22 – Testing and Evaluating AI Applications
**Focus:** measuring model-based application behaviour rather than assuming correctness.  
**Theory:** deterministic application tests versus probabilistic model evaluation, test datasets, expected behaviour, quality metrics, regression checks, cost and latency, evaluation limitations.  
**Demo:** small model-based classifier, extractor or question-answering application with a REST API, UI, saved test cases and results. Compare expected and actual outputs; automate repeatable tests with mocks and run a real-model evaluation.  
**Stretch/5.0:** SQL evaluation history, compare prompts/models on a fixed dataset, report measured results and failure categories.

### A23 – Machine Learning and Recommendation Systems
**Focus:** classical ML or recommendation techniques integrated into software.  
**Theory:** feature representation, supervised learning or recommendation methods, training/test separation, baselines, model evaluation, bias and limitations.  
**Demo:** catalogue recommendation or classification system using a pretrained model or a small reproducible dataset and appropriate algorithm, REST prediction/recommendation API, user-facing interface and persisted results.  
**Stretch/5.0:** compare baseline and alternative, report suitable metrics on held-out data, SQL catalogue/preferences, explain cold-start or classification errors.

### A24 – Spring AI vs LangChain4j
**Focus:** comparing Java LLM integration frameworks using the same model and task.  
**Theory:** model clients, dependency/configuration, prompts, structured output, tool and retrieval abstractions, testability, framework tradeoffs.  
**Demo:** two small independently runnable Java REST projects implementing the same quiz generation or structured extraction endpoint, one Spring AI and one LangChain4j. Use a common input/output contract, model configuration and test scenarios. A full frontend, separate databases and two hosted deployments are not required; show real requests and responses.  
**Stretch/5.0:** shared automated contract verification, same model and test corpus, measured output validity and documented implementation differences. SQL is an optional comparison extension.

## 6. Deployment notes and references

- Angular and React client-side SPAs can run on GitHub Pages. Angular build must use the correct project base href; React/Vite set base to /REPO/ for project Pages. Use hash routing (Angular withHashLocation; React HashRouter) or explicitly handle static-host deep links; GitHub Pages is not a Java/Node server and does not provide a general SPA rewrite. Publish built assets rather than raw source.
- Java or Python API must run on separate server/container hosting for advanced web track. Students may choose a suitable free-tier service or approved alternative; verify quotas and cold starts before requiring any specific service. SQL/NoSQL can be hosted independently. Configure CORS correctly.
- Mobile: Google Play internal testing still needs a developer account; Android APK emulator/device demo can be done without one. Apple free Xcode personal-team testing has limitations; TestFlight/App Store distribution requires appropriate membership. Accredited educational institutions may be eligible for Apple fee waiver. Do not require personal payment. Use test tracks/sandbox, not real payment transactions.
- Official references: [Angular deployment](https://angular.dev/tools/cli/deployment), [Angular routing](https://angular.dev/guide/routing/router-reference), [Vite static deploy](https://vite.dev/guide/static-deploy), [Google Play testing](https://support.google.com/googleplay/android-developer/answer/9845334), [Apple membership](https://developer.apple.com/help/account/membership/programs-overview/), [Apple enrolment](https://developer.apple.com/help/account/membership/program-enrollment).

## 7. Topic allocation and team work

The lecturer will assign topics to students or teams. A separate allocation list will be provided. Do not assume that every team must cover every topic. The same assigned subject can be addressed at basic or advanced depth; confirm the appropriate specification with the lecturer if necessary.

Work in pairs unless a different arrangement is approved. Prepare one coherent presentation per team, with clearly identified contributions. You may cover complementary technologies in the same presentation (e.g. two frontends using a common API, or two persistence implementations). If assigned subjects overlap or conflict after forming a team, ask the lecturer to confirm the final topic. Do not create multiple full presentations unless explicitly instructed.

Choose the topic-specific examples, explain the whole architecture at an overview level, and focus on the assigned technology. Keep the demonstrations reproducible. A topic assignment is not a requirement to purchase any software or developer account.
