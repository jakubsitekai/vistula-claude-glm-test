# Module 5 — Homework

*Vistula University · IT Fundamentals*

**Estimated time:** 30–60 minutes

**Before you start:** finish the laboratory first. Your project should already have `js/utils.js`, `js/utils.test.js`, and a green CI workflow on GitHub.

---

## Part 1 — Add one negative test case (15–20 min)

In the lab you tested an empty title `""` and a title with only spaces `"   "`. Now think of **one more negative case** for `formatTaskTitle` (or another helper function you wrote).

Ideas:

- a value that is not text at all, for example the number `42`,
- a very long text (for example 500 characters) — decide what the function *should* do,
- a title with strange characters, for example `"   \t \n "` (tab and newline).

Steps:

1. Write the new case in your test table first (input → expected result → actual result).
2. Add one new `test(...)` block with at least one `assert` to `js/utils.test.js`.
3. Run it locally: `node js/utils.test.js`. All tests must pass.
4. Push to GitHub and check that the Actions run is green ✅.

## Part 2 — Authentication vs Authorization in your own words (15–20 min)

Write **exactly 5 sentences** (simple English is fine) that explain the difference between **authentication** and **authorization**, using one example from your Student Task Manager project. Use these hints:

- Supabase login = ... (which of the two? why?)
- RLS policy (Row Level Security — the rule in the database that says which rows a user may see or change) = ... (which of the two? why?)

Example shape (do not copy it — use your own words):

1. Authentication means checking who the user is...
2. In my project, when a student enters an email and password in Supabase, this is ...
3. Authorization means checking what the user may do...
4. In my project, the RLS policy that lets a user see only their own tasks is ...
5. My own sentence, for example: a user who is logged in but opens another student's task gets ... because ...

Save your 5 sentences in a file `HOMEWORK.md` in your repository (or add them below your test table in `TESTS.md`).

## Part 3 — Push everything (5 min)

```
git add .
git commit -m "Homework: negative test case and authn vs authz"
git push
```

Check on GitHub: the Actions run is green, and your new text file is visible in the repository.

---

## Checklist before submitting

- [ ] One new negative test added, all tests pass locally (`node js/utils.test.js`).
- [ ] New test case also written in the test table.
- [ ] Exactly 5 sentences about authentication vs authorization, with the Supabase login and RLS examples.
- [ ] Pushed to GitHub; the latest Actions run is green.
- [ ] Submitted: repository link (+ deployed app link if it changed).
