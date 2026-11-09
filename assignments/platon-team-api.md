# Team Project Assignment 0 — Public REST API on GitHub Pages

*(final text to paste into Platon; copy everything below this line)*

---

## Team Project 0 — minimal web page with a public REST API (GitHub Pages)

**Deadline (suggested):** one week from publication. This is the simplest team
task of the course — treat it as a warm-up.

### Goal

Working in a **pair** (team work, as in Practical Assignment 1: one partner
opens the pull request), publish a minimal personal page on **GitHub Pages**
that fetches and displays data from a **REST API reachable from the outside**
(Supabase or a similar hosted backend).

### Technical requirements

1. **GitHub account format (mandatory):** the account that hosts the project
   must be named `vistula-team-project-<YOUR_STUDENT_ID>` (optionally with a
   three-letter suffix, e.g. `vistula-team-project-123456-abc`). Use the same
   account format as in the previous team assignment.
2. **Repository name (mandatory):** `vistula-team-project`.
3. The repository must contain:
   - `index.html` — a minimal page that displays data downloaded from your API,
   - `config.json` — with exactly this structure:
     ```json
     { "api_url": "https://<your-project>.supabase.co/rest/v1/<table>",
       "api_key": "<public anon key>" }
     ```
     (use the **public anon key** — never the service key).
4. **CORS open (mandatory):** the API must be callable from a different domain
   than the page (Supabase REST allows this by default — do not restrict it).
   Your page will be tested from another origin.
5. The API must answer `GET` with HTTP 200 and a JSON body.

### How to build it (shortest path)

1. Create/verify the GitHub account (format above) and the repository
   `vistula-team-project`.
2. Put `index.html` + `config.json` in the repository, commit, push.
3. Create a free Supabase project, create one table (e.g. `messages` with a
   text column), insert 2–3 rows, enable public read.
4. In repository **Settings → Pages**, publish from the `main` branch.
5. Open `https://<account>.github.io/vistula-team-project/` and verify the page
   shows your API data.

### What to upload to Platon

**Only the link to the repository**, e.g.

    https://github.com/vistula-team-project-123456/vistula-team-project

Do **not** upload screenshots. The page and API are checked automatically.

### How to test yourself before submitting

Open the platform page your lecturer gives you
(`…/index.html#/assignment-check`), paste your GitHub Pages URL and press
**Run self-check**. You will see, point by point, what works and what needs
fixing. When all checks are green, submit the repository link to Platon.
