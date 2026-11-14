# Contributing

## Branches

Work only on your own module branch, or on a short-lived branch for a new idea named `feature/<idea-name>`. Never commit directly to `main`.

## Workflow

1. Get the latest code:

        git checkout main
        git pull origin main

2. Switch to your branch and bring it up to date:

        git checkout feature/<your-branch>
        git merge main

3. Make your changes and commit often.
4. Push your branch:

        git push origin feature/<your-branch>

5. Open a pull request into `main` and fill in the template.
6. The repository owner reviews it. Fix any requested changes, and it will be merged.

## Commit messages

Use the format `type: short description`.

- feat: a new feature
- fix: a bug fix
- docs: documentation only
- refactor: code change that adds no feature and fixes no bug
- test: adding or fixing tests
- chore: config, dependencies, tooling

Examples: `feat: add swap request validation`, `fix: prevent duplicate substitutions`.

## Code guidelines

- Use TypeScript and keep types explicit.
- Use the shared design tokens in `src/lib/honey.ts` for colours, fonts and shadows. Do not hard-code colours.
- Never commit secrets. Keep keys in `.env.local` and update `.env.example` when you add a variable.
- Database changes must respect Row Level Security. Test them with each role.
- Run the app locally and check your change before opening a pull request.

## Reporting problems

Open a GitHub issue with steps to reproduce, what you expected and what happened. Add screenshots where they help.
