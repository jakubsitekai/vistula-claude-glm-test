# Team Project – IT: Assessment and Passing Requirements

## 1. General principles

The course has two assessed components: **Laboratory** and **Lecture**. The semester project contributes to both final grades. The same application can also support the presentation where it meets the assigned topic requirements.

**Passing Laboratory is a university requirement for passing Lecture.** Students who fail Laboratory, including students who do not meet its attendance requirements, cannot pass Lecture.

The aim is to develop genuine technical understanding, the ability to work with software engineering tools, independent learning and the ability to explain, verify and modify software.

AI tools are permitted when preparing assignments, projects and presentations. You remain responsible for correctness, security, reproducibility and your own understanding. **AI-generated work that you cannot explain or modify is not sufficient for a higher grade.**

**For final grades above 3.5, an individual practical assessment without AI assistance is mandatory. An oral assessment may also be required.** You may be asked to explain your work, answer technical questions, or independently modify and extend your code. Submitted assignments, tests and team results do not automatically guarantee a particular grade. No AI assistance is permitted during individual assessments unless explicitly authorised for a different exercise.

Previously announced alternative arrangements and attendance exceptions remain valid within their original scope. Individually approved study arrangements will be respected.

## 2. Laboratory – passing requirements

### Minimum requirements for grade 3.0

- Meet the laboratory attendance requirement (at least 80% of required sessions, subject to approved arrangements and previously announced alternatives).
- Complete and submit the following basic assignments in accordance with their instructions on Platon:
  1. **First Java CRUD**
  2. **Practical Assignment 1 – Task Manager & Team Collaboration**
- Complete the basic version of the shared semester project described in Section 4, subject to previously announced alternative arrangements.
- Complete the required laboratory activities and attend any announced compulsory assessments.
- Submit working solutions through Platon, not by email. Follow the required repository structure, GitHub collaboration and submission instructions.

Where a previous announcement stated that completing a task or attempting a test counts as attendance, that announcement remains valid. The scores of the practice tests conducted so far will not affect the final grade. New assessed tests may be conducted under supervision, and attendance at required laboratory sessions may be checked. Failure to meet the attendance requirement may result in failing the laboratory component.

### Requirements for a grade above 3.0

In addition to the basic requirements, complete both advanced assignments:

1. **First Java CRUD – REST API Extension**
2. **Practical Assignment – Advanced Task Manager & Team Collaboration**

These additional assignments are not required for students aiming only for 3.0. Use separate repositories as described in the assignment instructions. For grades above 3.5, also complete the advanced version of the semester project, meet the public deployment requirement and pass its individual practical defence (Section 4).

For grades above 3.5, an individual practical assessment is mandatory. An oral assessment may also be required. You may be asked to locate and explain code, demonstrate Git operations, modify REST endpoints or database queries, add a small feature, diagnose a problem or fix a bug. These tasks must be completed independently without AI.

| Final laboratory grade | Assessment criteria |
|---|---|
| 3.0 | Basic requirements fulfilled and satisfactory basic competence. |
| 3.5 | All required assignments completed, meaningful functional improvement and demonstrated basic competence. |
| 4.0 | Good understanding of submitted applications and independent implementation of straightforward changes. Individual practical defence. |
| 4.5 | Good technical understanding, independent debugging, more substantial changes and good individual defence. |
| 5.0 | Very good technical understanding, ability to independently solve more demanding practical problems, explain technical decisions and verify the resulting behaviour. Very good individual defence. |

The grade depends on demonstrated individual competence, not simply on the complexity of submitted code.

## 3. Lecture – passing requirements

The final lecture grade will be based on the mandatory presentation assignment, the shared semester project, assessed tests/quizzes (including colloquia), and an examination. For final grades above 3.5, individual practical assessment is required; an oral assessment may also be required. The presentation is a separately graded assignment with a significant impact on the final lecture grade. It does not replace the other assessments.

Lecture attendance is not mandatory under the previously announced rules. Attendance at scheduled assessments may be required.

### Mandatory assignment – Technical Presentation

The educational objective is to independently explore a technical subject, learn from reliable sources, understand a technology and communicate that knowledge clearly. Engineers must be able to learn unfamiliar technologies, verify technical claims and present practical solutions.

Work in pairs unless another arrangement is approved. Each team prepares one presentation on its assigned topic. Topic descriptions will be provided separately in **Presentation Topics**, and the topic allocation list will be announced separately.

**Basic track – assignment grade 3.0:** prepare at least 40 minutes of recorded presentation per team. A clear, technically correct theoretical presentation with diagrams and examples is sufficient. A working application is not required.

**Advanced track – assignment grades 4.0–5.0:** prepare at least 120 minutes of recorded presentation per team. Include theory, practical examples, a working demonstrator or runnable projects as required by the topic, architecture, code walkthrough, testing and deployment where applicable. The 120-minute presentation replaces the 40-minute presentation.

Duration is a mandatory minimum, not an automatic grade. The recording may use your own voice or AI-generated narration.

**Each presentation must have its own GitHub repository containing:**

- README.md with topic, authors, individual contributions, learning objectives, outline, links to the YouTube recording (unlisted is acceptable), presentation files and sources.
- An editable PowerPoint presentation (.pptx) with complete speaker notes consistent with the recording. A PDF copy is optional.
- Source code for all demonstrated applications, with prerequisites and precise build/run/test instructions, sample data, configuration without secrets, API examples and relevant screenshots.
- For advanced work: architecture diagrams, design decisions, database schema where applicable, validation/error handling, tests and hosted demo URLs where required by the topic.

See the [Presentation Repository Guide](presentation-repository-guide.md) for the required repository structure, README template, example diagrams and submission checklist.

Submit the repository link through Platon. The repository and recording must be accessible to the lecturer. Do not include secrets or real personal data. All demonstrated applications must actually run; AI-generated mockups are not evidence of working software. No paid developer account or paid service is compulsory.

### Presentation assignment grading

| Assignment grade | Requirements |
|---|---|
| 3.0 | Minimum 40 minutes; correct, coherent theory; complete slides, notes, recording and README. |
| 4.0 | Minimum 120 minutes; all required materials; working topic-specific demonstration, clear technical explanation and reproducible instructions. |
| 4.5 | All 4.0 requirements plus deeper analysis, meaningful tests, error scenarios and explanation of design tradeoffs. |
| 5.0 | All 4.5 requirements plus substantial technical depth, practical extension or comparison, reproducibility, automated verification and high educational value. Practical SQL is required for application-oriented topics; the four-framework comparison has its own scope. |

The detailed practical requirements depend on the assigned topic. For example, the four-framework comparison can use four small, independently runnable local REST APIs, while a dedicated Java framework presentation should demonstrate a more complete application. See the topic catalogue.

### Final lecture grade

To pass Lecture, you must first pass Laboratory, complete the mandatory presentation and semester project, and satisfy the requirements of the announced tests and examination, subject to applicable approved arrangements. A presentation graded 3.0 is sufficient for eligibility for a final lecture grade of 3.0 or 3.5. **For a final lecture grade of 4.0 or higher, you must earn at least 4.0 for the presentation assignment, complete the advanced semester project with public deployment and successfully complete the individual practical assessment.** An oral assessment may also be required.

The grade for the presentation is not the final lecture grade. Even a presentation graded 5.0 does not guarantee a final grade of 5.0. Assessment dates and detailed test instructions will be communicated separately.

## 4. Shared semester project – assessed within Laboratory and Lecture

**Complete a semester project in a team of two**, unless a different arrangement is approved. The project is a graded assignment contributing to both final grades. The laboratory assessment focuses on practical implementation and independent code changes; the lecture assessment focuses on understanding the architecture, technologies and design decisions. Where an individual defence is required, the same defence may provide evidence for both grades.

### Basic version (grade 3.0)

Create a working MVP (Minimum Viable Product) in a new GitHub repository. You may start from an earlier application and extend or adapt its code; keep the original submission unchanged.

- A clear purpose, working web or mobile interface and a meaningful user workflow.
- A backend exposing a REST API, with persistent data storage and functional CRUD operations appropriate to the domain.
- A working deployment or an agreed reproducible demonstration for grades 3.0 and 3.5. For higher grades, public deployment is mandatory (see below).
- A README describing functionality, architecture, authors and individual contributions, exact setup/run instructions, API examples, screenshots and demonstration link.
- Evidence of collaboration through Git commits and Pull Requests.

Previously announced alternative assessment routes remain valid within their original scope.

### Technology choices

- **Java is the recommended backend language.** You may use Spring Boot, Quarkus, Micronaut, Javalin or another suitable Java framework.
- **Python is an equally valid alternative** (e.g. FastAPI, Flask or Django). Both Java and Python are eligible for all grades, including 5.0, subject to the same functional, architectural, testing and individual assessment requirements. If you choose Python, you do so at your own responsibility, without Python-specific support from the lecturer.
- Frontend technology is your choice: HTML/CSS/JavaScript, Angular, React, Vue or a suitable mobile framework. SQL databases are preferred; PostgreSQL/Supabase is acceptable. A NoSQL database is also possible where appropriate.
- The Python option applies to the semester project, not to previously assigned Java-specific tasks or presentation topics. The choice between Java and Python does not limit the maximum grade.

### Public deployment – required for final grades above 3.5

For a final grade of 4.0, 4.5 or 5.0, the semester project must be deployed and accessible from the public Internet via a public domain or subdomain. A free hosting-provider subdomain is acceptable; buying a domain is not required. The application, including its backend and all required services, must remain operational and publicly accessible from the date of submission in Platon until at least the final course grade has been awarded, without requiring a team member to start a local server. Keeping the application available until the end of the examination session is strongly recommended. Include the working public application URL prominently in `README.md` in the GitHub repository. Include actual screenshots of the running application as additional evidence; screenshots do not replace a working deployment. If authentication is necessary, provide the lecturer with a safe way to test the application without exposing credentials publicly.

### Advanced version and individual defence

For grades above 3.5, extend the basic application with meaningful functionality and technical depth. **An individual practical defence without AI assistance is mandatory.** An oral assessment may also be required. You may be asked to explain source code, architecture, API and database, demonstrate tests, modify an endpoint or query, implement a small feature or fix a bug. Tasks will be defined in terms of expected behaviour and verified through working results, your explanation and the source code in your GitHub repository, regardless of the chosen language. You are responsible for knowing your chosen technology and completing changes independently; language-specific help is not guaranteed.

| Target final grade | Project evidence required (necessary, not sufficient) |
|---|---|
| 3.0 | Working basic MVP, documentation and collaboration. |
| 3.5 | Meaningful functional improvement, working application and complete documentation. Java or Python. |
| 4.0 | Extended application, coherent architecture, persistent data, documented REST API, validation, tests, public deployment and individual defence. Java or Python. |
| 4.5 | Well-integrated application, advanced functionality, meaningful automated tests, robust error handling, public deployment and good individual defence. Java or Python. |
| 5.0 | Practical SQL, substantial technical challenge, high-quality integrated implementation, clear architecture, reproducible public deployment and very good individual defence. Java or Python. |

Examples of advanced challenges include a shared REST API with web and mobile clients, authentication and authorization, different persistence implementations, test payment integration, CI/CD or cooperation between several pairs developing interoperable components. These are alternatives, not a mandatory list. Use sandbox/test payments; paid developer accounts and real store publication are not required.

### Optional project track – AI-Powered Applications

Students may choose a conventional software application or an AI-powered application. Both tracks are eligible for all grades, including 5.0, in Java or Python. AI integration is optional and does not replace the common project requirements (working interface, REST API, persistence, documentation, collaboration and individual defence where required).

| Project idea | Basic functional scope | Possible advanced extension |
|---|---|---|
| AI Quiz Generator | Build an independent quiz platform inspired by [vistula.devlabs.pl](https://vistula.devlabs.pl/), with the aim of improving it. Enter educational text; generate, validate, edit and save quizzes; allow students to take quizzes and view results. | Structured JSON output, difficulty and question-count settings, session/access codes, duplicate detection, teacher dashboard, quality evaluation and other meaningful improvements over the reference platform. |
| AI Document Assistant | Upload or select demo documents, ask questions and save answers with source references. | RAG, chunking, embeddings, retrieval evaluation, grounded citations and handling unanswerable questions. |
| Semantic Book Search | Manage a book catalogue and search descriptions by meaning. | Vector search with pgvector, metadata filters, keyword baseline and retrieval metrics. |
| AI Task Manager | Manage tasks; suggest categories, priorities or subtasks. | Structured output validation, user approval, editable suggestions, comparison with rule-based logic. |
| AI Code Review Assistant | Select a public/demo repository or diff; generate and store review suggestions. | GitHub API, severity filters, line references, evaluation against known issues; read-only integration. |
| AI Recommendation System | Store user preferences and recommend items from a demo catalogue. | Compare recommendation methods, explain recommendations and evaluate on a small labelled dataset. |
| Intelligent Customer Support | Ask questions about a demo knowledge base and save conversations. | RAG, escalation for unknown answers, read-only tool calling, evaluation and conversation history. |
| Intelligent Image Classifier | Upload permitted demo images, classify using a pretrained model and store results. | Confidence thresholds, evaluation on labelled images, confusion matrix and comparison of models. |

A pretrained model, external API or local model is sufficient; training your own model is not required. No paid API subscription, GPU purchase or cloud account is compulsory. Use a suitable free option, local runtime or approved shared infrastructure where available. Document model/runtime, configuration, limits and reproducible setup. Keep API credentials on the backend; use synthetic, public or properly licensed data, never confidential material. Handle unavailable models, malformed outputs and timeouts. A deterministic mock is useful for automated tests but is not a substitute for demonstrating a real AI feature.

For higher grades, demonstrate meaningful AI integration, validation of model outputs, representative success and failure cases, repeatable tests and a reasoned evaluation of limitations. For 5.0, retain the common practical SQL requirement and demonstrate a substantial technical extension. Simply wrapping a chatbot API or generating the application's source code with AI does not guarantee a higher grade.

During an individual defence, the lecturer may request a technology-independent change (e.g. add a difficulty selector, filter stored results, introduce output validation, persist a new field, add a test or change a REST endpoint). The student must make and verify the change independently, without AI coding assistance. Running the project's AI feature as part of a functional test is allowed; using it to generate the solution to the assessment task is not.

The same application can support an assigned AI presentation topic if it meets the relevant specification. See [Presentation Topics](presentation-topics.md), A15–A24. The presentation remains a separate graded assignment.

If your semester project also meets your assigned presentation topic, you may demonstrate the same application in the presentation rather than build another full application. Keep the presentation repository and its documentation separate; link to the exact demonstrated code version and include reproducible examples as required.

Submit the shared project link once through the designated Platon submission area. Its assessment contributes to both final grades; neither grade is determined by the project alone.

## 5. Submissions, deadlines and assessment organisation

- Submit each required assignment in its designated Platon submission area. Do not submit work by email as a replacement for Platon.
- Follow the individual assignment instructions and published deadlines. Keep original assignment repositories separate from extensions and the project.
- Use the dedicated GitHub account for the course and make repositories accessible for assessment.
- Team collaboration is allowed where specified; individual grades may differ according to demonstrated knowledge and contribution.
- Assessment dates, detailed test instructions, the topic allocation list  will be announced separately.
- If you have a previously approved individual arrangement or an explicitly announced alternative assessment route, its conditions remain applicable.

The objective is not simply to submit working software or AI-generated materials. It is to demonstrate that you can learn, understand, explain and, where required, independently develop software.
