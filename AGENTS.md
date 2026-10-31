# Case E: College Counseling

This project helps Mr. Wolanin's counselors gather questionnaire answers and teacher comments into a Google Doc for each student. The first demo builds profiles for the counselor, who writes every recommendation letter.

## How we work

- This is a standalone project repository. Paths start at its root. The old `Civic-AI-Github-Repository` monorepo is archived; do not edit it or use old `projects/` paths.
- Developers are high school students learning together. Prefer clear code over clever code. If you generate code the developer cannot explain, say so and explain it in plain English.
- Never push to `main`. Work on a branch, open a pull request (PR), and get at least one approving review before merging.
- Use `feature/<short-description>`, `fix/<short-description>`, or `chore/<short-description>`: lowercase, hyphens, no spaces. Old case prefixes are retired.
- Make small, frequent commits with plain-English messages. Use `.github/pull_request_template.md` for PRs.
- For Git, branching, PRs and merge conflicts, use the club's [Developer Onboarding Guide](https://github.com/CivicAIClub/docs/blob/main/developer-onboarding.md) instead of guessing.

## Commit and PR messages

- Never add `Co-authored-by`, `Generated with`, `Made-with`, `Claude-Session`, or any other AI attribution line to a commit message or PR description.
- When squash merging, delete any such lines GitHub adds to the merge message.

## Stack, deliverable and boundaries

- Use Google Apps Script in a Google Sheet for this deliverable.
- Input is two Google Sheets of made-up data: questionnaire answers, and teacher comments with student, course, teacher and term.
- Output is one profile Doc per student, with answers by section and comments grouped by course and term. Keep the empty My notes section for the counselor; the tool must never touch it.
- Run from a Build profiles menu in Apps Script. Running it again must update existing Docs without duplicates. That behavior defines the finished Phase 1 demo.
- The tool only gathers and organizes. Never write or draft recommendation letter text; no AI-written letters. Adaptive questions must wait for counselor approval.
- This is a public repository. Use made-up students for building, testing and examples, and say so in the README. Never commit real student records, grades, essays, teacher comments, questionnaire answers, recommendations, exports or documents.
- Never commit Sheet IDs, Doc IDs or web app links. Add `.env.example` as soon as a credential or ID is needed.
- Never commit secrets: no API keys, tokens or `.env` files. Keep real values in a gitignored local `.env`; every environment variable needs a placeholder in `.env.example`.
- If a developer pastes a real credential into a file, stop and tell them.
- Keep code at the repository root; there is no `projects/` folder. Keep the README accurate for setup.
- The project rule lists James Tian, James Lake, Alex Tong, Erin Park, Claire Desrosiers and Mason Gordon as developers, and Cayden Auyang as club lead. It says to keep the team line and `.github/CODEOWNERS` current when the team changes; resolve the conflicting source below before changing ownership.

## Setup status

The README has no Setup from a fresh clone section and no runnable setup commands. It asks for that section when real setup is added, covering install, environment variables with `.env.example`, run and build. Do not invent installation, package or server commands; use the current Apps Script stack and raise the missing setup instructions.

## Source disagreements

- `README.md:14` says teacher comments now come from report-card PDFs in Drive. `.cursor/rules/case-e-college-counseling.mdc:25` and `README.md:29` still specify two sample Sheets. Follow the project rule's two-Sheet demo until these sources are reconciled.
- `README.md:10-11` adds Keke and Luke to the team, names Keke lead developer and Luke club lead. `.cursor/rules/case-e-college-counseling.mdc:12` lists six developers and Cayden as club lead. Follow the project rule and flag the conflict before ownership changes.

## Beginner quick start

Full guide: https://github.com/CivicAIClub/docs/blob/main/developer-onboarding.md

1. First time: check Git with `git --version`, set your Git name and GitHub email, accept the club invite, and sign in with GitHub Desktop or `gh auth login`. Clone only your project's repo, open its folder, and read its README setup steps.
2. Start each work session from the latest main, then make a branch:

```sh
git checkout main
git pull origin main
git checkout -b feature/short-description
# Make and check your changes before continuing.
git status
git add .
git commit -m "Describe your change"
git push --set-upstream origin feature/short-description
```

Use `feature/`, `fix/`, or `chore/` as appropriate, with lowercase names and hyphens. Commit small working pieces; do not edit or push main directly.
3. Open a PR on GitHub, fill in the template, and get someone else's approval and passing checks where CI exists. Push review fixes to the same branch. After it is merged, pull main again before starting another branch.
4. If stuck, ask in the case chat, then Keke, then Luke or Cayden. Ask before doing anything drastic.

## Sources

- `README.md`
- `.cursor/rules/case-e-college-counseling.mdc`
- `.cursor/rules/civic-ai-workflow.mdc`
- `.cursor/rules/commit-messages.mdc`
- [Developer Onboarding Guide](https://github.com/CivicAIClub/docs/blob/main/developer-onboarding.md)
