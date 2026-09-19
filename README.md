# Kyle Swiger

Senior DevOps / full-stack engineer. I build small, fully serverless products on AWS and the
tooling that ships them: Terraform for everything, keyless GitHub Actions via OIDC, and AI
reviewers wired into every pull request.

🌐 [kswiger.dev](https://kswiger.dev)

## What I'm working on

| Project | What it is | Stack |
|---|---|---|
| [aws-deployment-tooling](https://github.com/kyleswiger/aws-deployment-tooling) | Reusable Terraform modules, CI templates, branch-ruleset scripts and a written methodology for shipping serverless apps | Terraform, Lambda, CloudFront, Cognito |
| [aws-reusable-workflows](https://github.com/kyleswiger/aws-reusable-workflows) | `workflow_call` GitHub Actions shared across my repos: SPA/API deploys, preview environments, ECS Fargate, Elixir CI, Fly.io | GitHub Actions, OIDC |
| [cabin-management](https://github.com/kyleswiger/cabin-management) | Invite-only app for a shared family property: priority booking window, occupancy-aware SMS reminders, supply checklist, maintenance ledger | TypeScript, React, Lambda, DynamoDB |
| [airhead-calendar](https://github.com/kyleswiger/airhead-calendar) | Family kitchen calendar for a wall-mounted touchscreen, with relevance tiers and a talk-or-type agentic interface | Python, FastAPI, Lambda |
| [gemini-pr-reviewer](https://github.com/kyleswiger/gemini-pr-reviewer) | Webhook-driven PR reviewer on Lambda that posts a commit status so it can gate merges | Python, API Gateway, Gemini |
| [beam-testbed](https://github.com/kyleswiger/beam-testbed) | Phoenix LiveView reference app proving the Elixir/BEAM path through the tooling above | Elixir, Phoenix, ECS Fargate |

Also in flight, privately: a trading-card scanner that identifies cards and lists them to
eBay, and an eBay deal monitor.

## How I work

- **Everything is Terraform.** No console clicks. One shared state bucket, one key per stack.
- **No long-lived cloud keys.** GitHub Actions assumes roles through OIDC; secrets live in SSM.
- **Two AI reviewers on every PR.** Claude Code and a self-hosted Gemini reviewer, both required
  status checks in the branch ruleset.
- **Small, hermetic tests.** pytest with in-memory SQLite, `tsc --noEmit`, `terraform validate`.
- **Conventional commits, release-please, squash or rebase only.**

## Toolbox

`AWS` `Terraform` `Python / FastAPI` `TypeScript / Node` `React + Vite` `Elixir / Phoenix`
`GitHub Actions` `CodePipeline` `Lambda` `DynamoDB` `ECS Fargate` `CloudFront` `Route 53`
