# Case E: College Counseling

## What this is

Mr. Wolanin in Pomfret's College Counseling Office is the client for this case. Before writing each student's recommendation letter, a counselor gathers that student's teacher comments and questionnaire answers into one Google Doc by hand. The first deliverable is a demo that builds those student profiles for the counselor; the counselor still writes every letter. Status: first meeting with Mr. Wolanin held October 9, 2026. Building a first demo.

| | |
|---|---|
| **Client** | Mr. Wolanin, College Counseling Office, Pomfret School |
| **Developers** | James Tian, James Lake, Alex Tong, Erin Park, Claire Desrosiers, Mason Gordon |
| **Club lead** | Cayden Auyang |
| **Status** | 🟡 First meeting held October 9, 2026. Building a first demo |

## The problem

Before writing each student's recommendation letter, a counselor gathers the student's teacher comments and questionnaire answers by hand into one Google Doc.

## Goal

Decisions from the first meeting:

- The counselor writes every letter. The tool only gathers and organizes. No AI-written letters.
- Adaptive questions come later, only after the counselors approve.

The first deliverable is a **student profile builder** demo:

- **In:** two Google Sheets of made-up data. One holds questionnaire answers. The other holds teacher comments, with the student, course, teacher and term for each.
- **Out:** one profile Doc per student, with the questionnaire answers by section, the teacher comments grouped by course and term, and an empty "My notes" section that the tool never touches.
- **How it runs:** from a "Build profiles" menu in Apps Script. Running it again updates each profile without duplicating anything.

## Stack

Google Apps Script in a Google Sheet, for this deliverable.

## Student data

This repository is public, and college counseling data is sensitive (teacher comments, questionnaire answers, recommendation letters). Build and test with made-up students only. Never commit real student data, exports, Docs, or any Sheet or Doc IDs.

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

The demo is done when the "Build profiles" menu turns the two sample Sheets into one profile Doc per student as described above, and a second run updates those Docs without duplicating anything.

## Contributors

- **Cayden Auyang:** club lead; set up this repository
- **James Tian:** developer
- **James Lake:** developer
- **Alex Tong:** developer
- **Erin Park:** developer
- **Claire Desrosiers:** developer
- **Mason Gordon:** developer
