# Team Project – IT: Assessment and Passing Requirements

## 1. General principles

The course consists of three separately assessed components:

- Laboratory
- Lecture
- Project

Each component has its own final grade. The same application or source code may be used as a basis for more than one component where the requirements permit, but submitting it does not automatically pass all three components.

The aim is to develop genuine technical understanding, the ability to work with software engineering tools, independent learning and the ability to explain, verify and modify software.

AI tools are permitted when preparing assignments, projects and presentations. You remain responsible for correctness, security, reproducibility and your own understanding. **AI-generated work that you cannot explain or modify is not sufficient for a higher grade.**

**For any final grade above 3.0 in any of the three components, an individual oral assessment is mandatory.** Depending on the component, you will be expected to explain your own work, answer technical questions and, for laboratory and project assessment, independently modify or extend code without AI assistance. Tests, submitted assignments and team results alone do not guarantee a higher grade. No AI assistance is permitted during individual assessments unless explicitly authorised for a different exercise.

Previously announced alternative arrangements and attendance exceptions remain valid within their original scope. Individually approved study arrangements will be respected.

## 2. Laboratory – passing requirements

### Minimum requirements for grade 3.0

- Meet the laboratory attendance requirement (at least 80% of required sessions, subject to approved arrangements and previously announced alternatives).
- Complete and submit the following basic assignments in accordance with their instructions on Platon:
  1. **First Java CRUD**
  2. **Practical Assignment 1 – Task Manager & Team Collaboration**
- Complete the required laboratory activities and attend any announced compulsory assessments.
- Submit working solutions through Platon, not by email. Follow the required repository structure, GitHub collaboration and submission instructions.

Where a previous announcement stated that completing a task or attempting a test counts as attendance, that announcement remains valid. The scores of the practice tests conducted so far will not affect the final grade. New assessed tests may be conducted under supervision, and attendance at required laboratory sessions may be checked. Failure to meet the attendance requirement may result in failing the laboratory component.

### Requirements for a grade above 3.0

In addition to the basic requirements, complete both advanced assignments:

1. **First Java CRUD – REST API Extension**
2. **Practical Assignment – Advanced Task Manager & Team Collaboration**

These additional assignments are not required for students aiming only for 3.0. Use separate repositories as described in the assignment instructions.

An individual oral and practical assessment is mandatory for a higher grade. You may be asked to locate and explain code, demonstrate Git operations, modify REST endpoints or database queries, add a small feature, diagnose a problem or fix a bug. These tasks must be completed independently without AI.

| Final laboratory grade | Assessment criteria |
|---|---|
| 3.0 | Basic requirements fulfilled and satisfactory basic competence. |
| 3.5 | All required assignments completed; satisfactory individual oral and practical assessment of basic concepts and simple code changes. |
| 4.0 | Good understanding of submitted applications and independent implementation of straightforward changes. |
| 4.5 | Very good technical understanding, independent debugging and more substantial changes. |
| 5.0 | Excellent understanding and ability to independently solve more demanding practical problems, explain technical decisions and verify the resulting behaviour. |

The grade depends on demonstrated individual competence, not simply on the complexity of submitted code.

## 3. Lecture – passing requirements

The final lecture grade will be based on the mandatory presentation assignment, assessed tests/quizzes (including colloquia), and an examination. The examination may include an oral part; an individual oral assessment is mandatory for any final grade above 3.0. The presentation is a separately graded assignment with a significant impact on the final lecture grade. It does not replace the other assessments.

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

To pass the lecture, complete the mandatory presentation and satisfy the requirements of the announced tests and examination. **To obtain any final lecture grade above 3.0, including 3.5, you must earn at least 4.0 for the presentation assignment and successfully complete the individual oral assessment.**

The grade for the presentation is not the final lecture grade. Even a presentation graded 5.0 does not guarantee a final grade of 5.0. Final assessment dates, test thresholds and the exact weighting of the components will be communicated separately.

## 4. Project – passing requirements

### Objective

Design, implement, document and deliver a working software application. Demonstrate collaboration, technical decisions and the ability to deliver a reproducible solution.

Work in teams of two unless a different arrangement is approved. Larger integrated projects may involve several cooperating pairs, provided that each pair has a clearly defined component and each student's individual contribution is identifiable.

### Minimum requirements for grade 3.0

Create a working MVP (Minimum Viable Product) in a new GitHub repository for the project. You may start from a previous assignment and extend or adapt its code; do not modify the original submission as part of the new project.

A basic web application may use HTML, CSS, JavaScript and a hosted database/API such as Supabase, deployed using GitHub Pages. Other suitable technologies are also allowed. A basic project should have:

- A clear purpose, a working interface and at least one meaningful user workflow.
- Persistent data storage and functional create/read/update/delete operations where appropriate to the domain.
- A working deployment or another agreed reproducible demonstration.
- Source code, a README describing functionality, architecture, authors and contributions, setup/run instructions, screenshots and demonstration link.
- Evidence of collaboration through Git commits and Pull Requests.
- A demonstration showing that the application works.

Submit your project link through Platon according to the project submission instructions.

### Higher grades – advanced project and individual defence

For a grade above 3.0, extend the basic application with meaningful additional functionality and technical depth. An individual oral and practical project defence without AI assistance is mandatory.

An advanced project may use a Java REST backend (Spring Boot, Quarkus, Micronaut, Javalin or another suitable Java framework), a web frontend (Angular, React, Vue or equivalent), a mobile client, SQL or NoSQL persistence, authentication/authorization, tests and deployment. Choose technologies appropriate to the project; do not add unnecessary complexity.

| Final project grade | Assessment criteria |
|---|---|
| 3.0 | Working basic MVP, complete documentation and evidence of collaboration. |
| 3.5 | Basic requirements plus a meaningful functional improvement and satisfactory individual defence. |
| 4.0 | Extended application with coherent architecture, persistent data, documented interfaces, practical functionality and good individual defence. |
| 4.5 | Well-integrated application, more advanced functionality, meaningful automated tests, robust error handling and very good individual defence. |
| 5.0 | Substantial technical challenge, high-quality integrated implementation, clear architecture, reproducible deployment, practical verification and excellent individual defence. |

Examples of advanced challenges include a shared REST API with web and mobile clients, alternative frontends or persistence implementations, secure multi-user applications, test payment integration, or cooperation between several pairs developing interoperable components. These are alternatives, not a mandatory list of technologies. Real store publication and paid developer accounts are not required. Payments should use sandbox/test environments.

During the defence, you may be asked to explain the architecture, API, database, source code and contribution, and independently implement a change or fix a problem.

## 5. Submissions, deadlines and assessment organisation

- Submit each required assignment in its designated Platon submission area. Do not submit work by email as a replacement for Platon.
- Follow the individual assignment instructions and published deadlines. Keep original assignment repositories separate from extensions and the project.
- Use the dedicated GitHub account for the course and make repositories accessible for assessment.
- Team collaboration is allowed where specified; individual grades may differ according to demonstrated knowledge and contribution.
- Assessment dates, detailed test instructions, the topic allocation list and any remaining grading thresholds will be announced separately.
- If you have a previously approved individual arrangement or an explicitly announced alternative assessment route, its conditions remain applicable.

The objective is not simply to submit working software or AI-generated materials. It is to demonstrate that you can learn, understand, explain and, where required, independently develop software.
