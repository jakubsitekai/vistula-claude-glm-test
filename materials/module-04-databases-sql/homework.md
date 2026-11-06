# Module 4 — Homework: Priority Column and a Filter

**Vistula University · IT Fundamentals**

## Estimated Time

30–60 minutes.

## Prerequisites

- Module 4 lab is done: your Student Task Manager works with Supabase (Create, Read, Update, Delete).
- You still have the Supabase project URL and anon key from the teacher.

---

## Task 1 — Add a `priority` Column with ALTER TABLE (15 min)

Tables can change after they exist. SQL has a command for this: `ALTER TABLE` (change a table).

Open the Supabase **SQL Editor** and run:

```sql
-- Add a new column "priority" to the existing tasks table
ALTER TABLE tasks
ADD COLUMN priority text DEFAULT 'normal';
```

Now every task has a priority. The default value is `'normal'`, so old tasks keep working. Possible values in this homework: `'low'`, `'normal'`, `'high'`.

> **Note:** `ALTER TABLE` changes the table for **everyone** in the class project. Run it exactly once, and tell your teacher when it is done.

### Update the app

1. In `tasks.html`, add a small input (a `<select>` is a good choice) so a new task can get a priority: `low`, `normal`, or `high`.
2. In your **Create** (INSERT) call, send the chosen priority too:
   ```js
   .insert({ title: title, priority: chosenPriority })
   ```
3. Show the priority in the task list (for example, a small label next to the title).

---

## Task 2 — Filter: Show Only Not-Done Tasks (15 min)

Add a **checkbox** to the page: "Show only not-done tasks".

When it is checked, use Supabase to select only rows where `done` is `false`:

```js
let query = supabase
  .from("tasks")
  .select("*")
  .order("created_at", { ascending: false });

if (onlyNotDone) {
  query = query.eq("done", false); // like SQL: WHERE done = false
}

const { data, error } = await query;
```

When the checkbox is empty, show all tasks again (call the same function with `onlyNotDone = false`).

### Check yourself

- Create a task with priority `high` and mark another task as done.
- Tick "Show only not-done tasks". The done task must disappear.
- Reload the page: the filter state may reset, but the data is still there.

---

## Task 3 — Write 5 Sentences About Primary Keys (10 min)

Write **5 sentences** (in English) answering this question:

> **Why is the primary key important for UPDATE and DELETE?**

Think about:

- What does `WHERE id = 1` guarantee that `WHERE title = 'Buy milk'` does not?
- What could happen if two rows had the same title?
- What could a user delete or change by mistake without a unique id?

Write full sentences, not bullet points. Save them in a file called `homework4.md` in your repository.

---

## Task 4 — Push to the Repository (10 min)

1. Commit your changes on a feature branch (for example `module4-homework`):
   ```
   git checkout -b module4-homework
   git add .
   git commit -m "Add priority column, not-done filter, and homework answers"
   ```
2. Push the branch and merge the pull request into `main` (a quick self-review or partner review is welcome).
3. Check that your published page (e.g. GitHub Pages) shows the new version.

---

## Expected Deliverables

- The `tasks` table with the new `priority` column.
- The app can save a priority and filter for not-done tasks.
- `homework4.md` with your 5 sentences about primary keys.

## Submission Instructions

Submit through the course platform on the assignment page (Assignments section): paste your GitHub repository URL / deployed app URL / PR URL as required.

1. **Repository URL** (GitHub).
2. **Page URL** (published app).
3. Your **name and student ID**.

Deadline: before the next class.
