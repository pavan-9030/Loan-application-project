# Bank Loan Application Tracking System — Practice Project

> A personal practice project built to learn and demonstrate Business Analyst / Product
> Owner tools: **Jira, Agile & Scrum, Postman, Confluence, and draw.io** — modeled on a
> realistic fintech scenario (inspired by how a company like Finastra manages loan
> features).

## 1. Project Idea

A bank wants a new digital feature: customers should be able to apply for a personal
loan online, track its status, and get notified at each stage — instead of visiting a
branch. This repo documents how I approached that as a Business Analyst / Product Owner,
end to end, using industry-standard tools.

## 2. What's in this repo

| Folder | Contents | Tool used |
|---|---|---|
| `/jira` | Epics, user stories, acceptance criteria, sprint plan | Jira |
| `/confluence` | Business requirement document (BRD) and process notes | Confluence |
| `/postman` | API test collection for the loan status endpoints | Postman |
| `/diagrams` | Process flow diagram (loan application lifecycle) | draw.io |
| `CHALLENGES.md` | Problems I ran into while building this, and how I solved them | — |

## 3. How I approached it (my process)

1. **Defined the problem** — wrote a one-paragraph business goal: reduce loan
   application time from 3 days (branch visit) to under 10 minutes (digital).
2. **Wrote the BRD in Confluence** — captured the business need, scope, and
   out-of-scope items before touching Jira, so the team has one source of truth for
   *why* we're building this.
3. **Broke it into Jira Epics and Stories** — one Epic ("Digital Loan Application"),
   split into 6 user stories with clear acceptance criteria (see `/jira`).
4. **Planned 2 sprints** — Sprint 1: application + document upload. Sprint 2: status
   tracking + notifications. (See sprint plan in `/jira`.)
5. **Modeled the process visually in draw.io** — a swimlane diagram showing the
   customer, bank system, and credit-check service, so developers and the client could
   agree on the flow before coding started.
6. **Tested the underlying API in Postman** — since "check loan status" is really an
   API call under the hood, I built a small Postman collection against a public test
   API to simulate and validate the request/response flow a developer would build.
7. **Tracked progress like a real sprint** — moved stories through
   To Do → In Progress → Done, and wrote a short retrospective note on what I'd do
   differently.

## 4. Tools mapped to real use in this project

- **Agile/Scrum** — the whole project is structured as 2 sprints with a sprint goal,
  backlog, and a retrospective (see `/jira/sprint_plan.md`).
- **Jira** — epics/stories are written in Jira's format so they can be directly
  imported (`/jira/epics_stories.csv`).
- **Confluence** — the BRD (`/confluence/BRD.md`) is written the way a Confluence page
  would be structured, with linked Jira references.
- **Postman** — `/postman/loan_status_api.postman_collection.json` can be imported
  directly into Postman to run the sample requests.
- **draw.io** — `/diagrams/loan_process_flow.drawio` can be opened directly at
  app.diagrams.net (draw.io) to view/edit the swimlane diagram.

## 5. How to talk about this in an interview

> "I built a small end-to-end practice project to apply BA/PO tools in a realistic
> fintech scenario — a digital loan application feature. I wrote the business
> requirement doc in Confluence, broke it into epics and stories in Jira with
> acceptance criteria, planned two sprints, mapped the process in draw.io, and tested
> the underlying API flow in Postman. It's on my GitHub if you'd like to see it."

Then be ready to open `/jira`, `/confluence`, `/postman`, or `/diagrams` live and walk
through one file — that's what makes it credible.
