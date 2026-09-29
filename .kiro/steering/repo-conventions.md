---
inclusion: auto
name: repo-conventions
description: Conventions for referencing Carlos Biagolini's repositories and tutorial indexes inside the profile README.
---

# Repository and Content Conventions

Use this when editing the "About My GitHub" section or any part of the README that links to repositories, tutorial indexes, or featured projects.

## Repository Naming Convention

Carlos names repositories with the main technology as a prefix, followed by a short description of the content. Examples: `PythonAwsBedrockAgentCoreRuntime`, `TerraformCloudTrail`, `TerraformBabyCareApp`. When mentioning a repository, match this PascalCase, no-separator style exactly as it exists on GitHub. Confirm the exact name with `gh repo view biagolini/<repo>` before linking, because a wrong case or typo breaks the link.

## Tutorial Indexes

The README groups tutorials into curated index repositories by technology (for example `Terraform`, `Python`, `Java`, `Node`, `Php`, `C`, `R`, `Angular`, `WebPages`). These indexes are presented in a Markdown table grouped into columns such as "Cloud & IaC", "Languages", and "Web & Frontend". When adding a new index, place it in the matching column and keep the table aligned. Verify the index repository exists before adding it.

## Featured Projects

Featured projects highlight flagship AWS work (for example the Amazon Bedrock and AgentCore series, and full-stack Terraform serverless examples). When adding a featured project, keep the description short and factual, link to the real repository, and confirm the repository name and description with `gh repo view`. Prefer grouping related repositories into a single themed bullet rather than listing many separate lines.

## Verifying Before You Link

Any repository link added to the README must point to a repository that actually exists under the `biagolini` account. Always confirm with the GitHub CLI via the shell (`gh repo list biagolini --limit 200` or `gh repo view biagolini/<repo>`) before inserting or changing a link. Do not fabricate repository names or infer them from patterns.

## AWS Naming

Repository descriptions and project blurbs frequently mention AWS services. Use official AWS service names (for example "Amazon Bedrock", "Amazon ECS on AWS Fargate", "AWS Lambda"). When unsure of the exact current name, confirm it with the AWS Knowledge or AWS Documentation MCP servers.
