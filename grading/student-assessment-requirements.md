# Team Project – IT: Assessment and Passing Requirements

## 1. General principles

The course has two final grades: **Laboratory** and **Lecture**. The semester project is a shared assignment contributing to both grades; there is no separate final project grade. You prepare one semester project, not two. The same application can also support the presentation where it meets the assigned topic requirements. Each final grade has its own assessment criteria.

The aim is to develop genuine technical understanding, the ability to work with software engineering tools, independent learning and the ability to explain, verify and modify software.

AI tools are permitted when preparing assignments, projects and presentations. You remain responsible for correctness, security, reproducibility and your own understanding. **AI-generated work that you cannot explain or modify is not sufficient for a higher grade.**

**For any final grade above 3.0 in either component, an individual oral assessment is mandatory.** Depending on the component, you will be expected to explain your own work, answer technical questions and, for laboratory and the shared project assessment, independently modify or extend code without AI assistance. Tests, submitted assignments and team results alone do not guarantee a higher grade. No AI assistance is permitted during individual assessments unless explicitly authorised for a different exercise.

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

These additional assignments are not required for students aiming only for 3.0. Use separate repositories as described in the assignment instructions. For a higher grade, also complete the advanced version of the shared semester project and pass its individual defence (Section 4).

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

The final lecture grade will be based on the mandatory presentation assignment, the shared semester project, assessed tests/quizzes (including colloquia), and an examination. The examination may include an oral part; an individual oral assessment is mandatory for any final grade above 3.0. The presentation is a separately graded assignment with a significant impact on the final lecture grade. It does not replace the other assessments.

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

To pass the lecture, complete the mandatory presentation, the basic shared semester project and satisfy the requirements of the announced tests and examination, subject to previously announced alternatives. **To obtain any final lecture grade above 3.0, including 3.5, you must earn at least 4.0 for the presentation assignment, complete the advanced shared semester project and successfully complete the individual oral assessment.**

The grade for the presentation is not the final lecture grade. Even a presentation graded 5.0 does not guarantee a final grade of 5.0. Final assessment dates, test thresholds and the exact weighting of the components will be communicated separately.

## 4. Shared semester project – assessed within Laboratory and Lecture

There is no separate final project grade. **Complete one semester project in a team of two**, unless a different arrangement is approved. The project contributes to both final grades. The laboratory assessment focuses on practical implementation and independent code changes; the lecture assessment focuses on understanding the architecture, technologies and design decisions. A single individual defence may provide evidence for both grades.

### Basic version (grade 3.0)

Create a working MVP (Minimum Viable Product) in a new GitHub repository. You may start from an earlier application and extend or adapt its code; keep the original submission unchanged.

- A clear purpose, working web or mobile interface and a meaningful user workflow.
- A backend exposing a REST API, with persistent data storage and functional CRUD operations appropriate to the domain.
- A working deployment or an agreed reproducible demonstration.
- A README describing functionality, architecture, authors and individual contributions, exact setup/run instructions, API examples, screenshots and demonstration link.
- Evidence of collaboration through Git commits and Pull Requests.

Previously announced alternative assessment routes remain valid within their original scope.

### Technology choices

- **Java is the preferred backend language.** You may use Spring Boot, Quarkus, Micronaut, Javalin or another suitable Java framework.
- Python is an alternative backend option (e.g. FastAPI, Flask or Django) for the standard project route up to grade 4.0. To be eligible for a final grade of 4.5 or 5.0 through this route, the project backend must be implemented in Java.
- Frontend technology is your choice: HTML/CSS/JavaScript, Angular, React, Vue or a suitable mobile framework. SQL databases are preferred; PostgreSQL/Supabase is acceptable. A NoSQL database is also possible where appropriate.
- The Python option applies to the semester project, not to previously assigned Java-specific tasks or presentation topics. The technology choice does not automatically determine the grade.

### Advanced version and individual defence

For grades above 3.0, extend the basic application with meaningful functionality and technical depth. **An individual oral and practical defence without AI assistance is mandatory.** You may be asked to explain source code, architecture, API and database, demonstrate tests, modify an endpoint or query, implement a small feature or fix a bug.

| Target final grade | Project evidence required (necessary, not sufficient) |
|---|---|
| 3.0 | Working basic MVP, documentation and collaboration. |
| 3.5 | Meaningful functional improvement and satisfactory individual defence. Java or Python. |
| 4.0 | Extended application, coherent architecture, persistent data, documented REST API, validation, tests and good individual defence. Java or Python. |
| 4.5 | Java backend, well-integrated application, advanced functionality, meaningful automated tests, robust error handling and very good individual defence. |
| 5.0 | Java backend, practical SQL, substantial technical challenge, high-quality integrated implementation, clear architecture, reproducible deployment and excellent individual defence. |

Examples of advanced challenges include a shared REST API with web and mobile clients, authentication and authorization, different persistence implementations, test payment integration, CI/CD or cooperation between several pairs developing interoperable components. These are alternatives, not a mandatory list. Use sandbox/test payments; paid developer accounts and real store publication are not required.

If your semester project also meets your assigned presentation topic, you may demonstrate the same application in the presentation rather than build another full application. Keep the presentation repository and its documentation separate; link to the exact demonstrated code version and include reproducible examples as required.

Submit the shared project link once through the designated Platon submission area. Its assessment contributes to both final grades; neither grade is determined by the project alone.

## 5. Submissions, deadlines and assessment organisation

- Submit each required assignment in its designated Platon submission area. Do not submit work by email as a replacement for Platon.
- Follow the individual assignment instructions and published deadlines. Keep original assignment repositories separate from extensions and the project.
- Use the dedicated GitHub account for the course and make repositories accessible for assessment.
- Team collaboration is allowed where specified; individual grades may differ according to demonstrated knowledge and contribution.
- Assessment dates, detailed test instructions, the topic allocation list and any remaining grading thresholds will be announced separately.
- If you have a previously approved individual arrangement or an explicitly announced alternative assessment route, its conditions remain applicable.

The objective is not simply to submit working software or AI-generated materials. It is to demonstrate that you can learn, understand, explain and, where required, independently develop software.
