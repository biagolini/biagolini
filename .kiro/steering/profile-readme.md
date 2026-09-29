---
inclusion: always
---

# GitHub Profile README Guidelines

This repository is a **GitHub profile repository**: its `README.md` is rendered at the top of Carlos Biagolini's public GitHub profile (the special repository whose name matches the username). Treat the README as a public, personal home page, not as project documentation.

## Purpose and Audience

The README introduces Carlos to recruiters, fellow builders, and the AWS community. It should quickly communicate who he is, what he works with, his AWS certifications, and where to find his content. Keep it welcoming, credible, and easy to skim.

## Identity to Preserve

Carlos Biagolini is an AWS Cloud Solutions Architect at OpsTeam (AWS Premier Partner), an AWS Community Builder in AI Engineering, based in São Paulo, Brazil, with a PhD in Ecology. The profile centers on AWS: Generative AI (Amazon Bedrock, AgentCore, Bedrock Agents, Knowledge Bases, RAG), serverless and event-driven architecture, Well-Architected and FinOps, Infrastructure as Code, cloud security, observability, and AI-assisted development. Do not dilute this AWS-centric focus.

## Section Structure (current order)

Keep the existing sections and their order unless the user asks otherwise:

1. Header: name, one-line role summary, short intro paragraph, and the PhD-in-Ecology note.
2. Social and content badges (LinkedIn, Medium, AWS Builder Center, YouTube, Credly).
3. AWS Skills & Focus Areas.
4. AWS Certifications (Credly badges that link to public verification).
5. About My GitHub (naming convention, tutorial indexes, featured projects).
6. AWS Community & Content.
7. Connect.

Use the existing emoji section headers (for example `## 🏅 AWS Certifications`) for visual consistency.

## Tone and Style

First person, professional yet approachable, honest, no hype or corporate speak. Follow the repository writing-style rules: no hard wrap inside a paragraph, avoid em dashes and stray hyphens as stylistic pauses (prefer commas, parentheses, or separate sentences), and do not overuse bullet lists. Reserve lists for genuine enumerations such as skills or certifications.

## Accuracy Rules

Never invent certifications, repositories, projects, badges, or links. Before adding or changing anything factual, verify it with the GitHub CLI via the shell:

- `gh api user` or `gh api users/biagolini` for profile data.
- `gh repo list biagolini --limit 200` to confirm repository names.
- `gh repo view biagolini/<repo>` to confirm a repository's description and existence.

Do not guess repository names or URLs; confirm them with `gh`. When touching AWS service names or technical claims, confirm exact, current AWS naming with the AWS Knowledge and AWS Documentation MCP servers.

## Badges and Links

Social/content badges use `shields.io` with the `flat` style and a service logo. New badges must match that pattern. Certification badges use the Credly image (`images.credly.com/size/110x110/...`) wrapped in a link to the public verification URL (`credly.com/badges/<id>/public_url`). When adding a certification, confirm both the image URL and the verification URL before inserting.

## What Not to Do

Do not commit, push, or open pull requests unless explicitly asked. Keep edits focused and reversible. Do not add tracking, analytics, or third-party content the user did not request.
