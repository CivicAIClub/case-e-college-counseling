# Case E — College Counseling

| | |
|---|---|
| **Client** | Mr. Wolanin, College Counseling Office, Pomfret School |
| **Developers** | _Unassigned — this case is open._ |
| **Club lead** | Cayden Auyang |
| **Status** | 🔵 Discovery not started |

## The problem

_To be written with Mr. Wolanin during discovery: what the college counseling office does by hand today, where the time goes, and what "better" would look like for him and for students._

## Goal

_To be defined in discovery._ Candidate directions to explore in the first meeting (not commitments): tracking application deadlines and requirements per student, organizing recommendation-letter requests, summarizing counseling notes, or drafting communications.

## Stack

_Not decided._ Pick the simplest thing that fits the office's existing tools (Google Workspace is likely). Decide during discovery and record the decision here and in `.cursor/rules/case-e-college-counseling.mdc`.

## Repository layout

```
case-e-college-counseling/
├── README.md              ← this file; keep it the source of truth for setup
├── .cursor/rules/         ← committed Cursor rules (workflow + project context)
├── .github/               ← pull request template, CODEOWNERS
└── .gitignore
```

Add code at the repo root (no `projects/` folder). When you add a real setup, write a "Setup from a fresh clone" section here: install, env vars (with a `.env.example`), run, build.

## Working on this repo

- Branch from `main` as `feature/<short-description>`, `fix/<short-description>`, or `chore/<short-description>` (lowercase, hyphens).
- Every change goes through a pull request with at least one approval. `main` cannot be pushed to directly.
- Never commit secrets. Put real values in a gitignored `.env`; list variable names with placeholders in `.env.example`.
- Cursor rules for this project are committed in `.cursor/rules/`. You do not need to paste anything into your IDE settings.
- The full Git walkthrough for beginners is the club's **[Developer Onboarding Guide](https://github.com/CivicAIClub/docs/blob/main/developer-onboarding.md)**.

## Definition of done (Phase 1)

_To be set after the discovery meeting._ A good Phase 1 is one concrete workflow of Mr. Wolanin's, automated end to end, that he can run himself.
