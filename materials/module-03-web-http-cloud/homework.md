# Module 3 — Homework: Improve Your Task Manager

**Estimated time:** 30–60 minutes
**Individual work** (each student submits their own commit and answers).

This homework builds on the `tasks.html` page from the lab.

## Task 1 — Add a new field: Category (10–15 min)

Add one more field to your task form:

- A **category select** (`<select>`) with at least four options, for example: `Studies`, `Work`, `Home`, `Other`.

The category must:

- Appear in the task list next to the title, due date and priority.
- Be saved in **localStorage** together with the other fields (remember: localStorage lives only in this browser — that is fine for now; the shared database comes in Module 4).
- Be loaded back correctly when the page refreshes.

## Task 2 — Improve the validation (10–15 min)

Your lab page already rejects an empty title and a title longer than 60 characters. Add at least **two** of these improvements:

- Reject a **due date in the past** with a clear error message, for example "The due date cannot be in the past."
- Require a **due date** (it cannot be empty).
- Show the error message **next to the field** it concerns, not only at the bottom of the form.
- Show a short **green confirmation message** ("Task added") for 2–3 seconds after a successful add.
- **Trim** the title (remove extra spaces at the start and end) before saving it.

Every rule you add must show a **visible, human-readable message**. Silent failure is not acceptable — the user must always know why the task was not added.

## Task 3 — Write 5 sentences (10 min)

In a file called `REFLECTION.md` in your repository, write **exactly 5 sentences** in English answering:

> What happens, step by step, when the browser loads your `tasks.html` page?

Explain the order: **HTML → CSS → JavaScript**. Say what each of the three languages contributes, and mention what localStorage does when the page opens. Simple English is fine — correctness matters more than fancy words.

*Hint from theory:* the browser reads the HTML file and builds the page structure, then applies the CSS to style it, then runs the JavaScript — which loads your saved tasks from localStorage and shows them.

## Task 4 — Commit and push (5 min)

Use a feature branch, as in the lab:

```bash
git switch main
git pull
git switch -c feature/homework-3
# ... make your changes ...
git add tasks.html tasks.js REFLECTION.md
git commit -m "Add category field, better validation, and load-order reflection"
git push -u origin feature/homework-3
```

Then open a Pull Request, merge it (a partner review is welcome but not required this time), and check that your GitHub Pages URL shows the new version.

## Submission Instructions

Submit through the course platform on the assignment page (Assignments section): paste your GitHub repository URL / deployed app URL / PR URL as required.

1. **Repository URL** — your GitHub project.
2. **GitHub Pages URL** — the live link to `tasks.html`.
3. Confirm that `REFLECTION.md` is in the repository with your 5 sentences.

**Deadline:** before the next class (see the assignment page on the course platform).
