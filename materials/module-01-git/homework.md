# Module 1 — Homework: Git Practice and Reflection

**Estimated time:** 30–60 minutes
**Work mode:** solo (this is your own work — do not copy from classmates)

This homework continues the laboratory work on your `project-website` repository.

## Task 1 — Pull the Newest Version

1. Open a terminal in your `project-website` folder.

```bash
git pull
```
This downloads any new commits from GitHub (for example, the merge from the laboratory class).

## Task 2 — New Branch with a README Improvement

2. Create and switch to a new branch:

```bash
git checkout -b feature-readme
```
This creates a branch called `feature-readme` and switches to it in one step.

3. Open the file `README.md` and improve it. Add at least:
   - one short paragraph (2–3 sentences) explaining what the project is,
   - one section "How to view the page" with a link to your GitHub Pages site.

4. Stage, commit and push:

```bash
git add README.md
```
Puts the file into the staging area.

```bash
git commit -m "Improve README with project description"
```
Saves the staged change on the `feature-readme` branch.

```bash
git push -u origin feature-readme
```
Sends the new branch to GitHub.

5. On GitHub, open a pull request from `feature-readme` into `main`. Give it a clear title and one sentence of description. You can merge it yourself — or ask a classmate to review it first (recommended!).

## Task 3 — One More Pull Request (Your Choice)

6. Repeat the same workflow one more time with a small change of your choice. Ideas:
   - add one more feature to `index.html`,
   - fix a typo anywhere in the repository,
   - add a short "Team rules" section to the README.

   The important part is the **workflow**, not the size of the change:

```bash
git checkout -b fix-typo
```
Creates and switches to a new branch for this small fix.

Make the change, then:

```bash
git add .
git commit -m "Fix typo in the feature list"
git push -u origin fix-typo
```
Stages all changes, commits them, and sends the branch to GitHub.

7. Open a pull request on GitHub and merge it into `main`.

## Task 4 — Reflection: Git versus GitHub

8. In your repository, create a new file called `reflection.md`. Write **five sentences** (in English) explaining the difference between Git and GitHub. Use your own words — do not copy from the theory handout. Helpful questions to think about:
   - Which one is a program on your computer, and which one is a website?
   - Which commands belong to Git, and which actions happen only on GitHub?
   - Why do you need both for teamwork?

9. Save the reflection in the repository and publish it using the same workflow:

```bash
git checkout -b feature-reflection
```
Creates a branch for the reflection.

```bash
git add reflection.md
git commit -m "Add reflection on Git and GitHub"
git push -u origin feature-reflection
```
Stages, commits and pushes the reflection file. Then open a pull request on GitHub and merge it into `main`.

## Checklist Before You Finish

- [ ] At least two new pull requests merged into `main`.
- [ ] `README.md` has a project description and a link to your site.
- [ ] `reflection.md` exists on `main` and contains exactly five sentences.
- [ ] All commit messages are short and describe what you did.
- [ ] No work was done directly on `main` — everything went through a branch and a pull request.

## Submission Instructions

Submit through the course platform on the assignment page (Assignments section): paste your GitHub repository URL / deployed app URL / PR URL as required.

1. **Repository URL** — your GitHub project.
2. **GitHub Pages URL** — the live link to your site.
3. Your **name and student ID**.

Deadline: before the next class.
