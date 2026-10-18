# Azure-Devops-Hands-on

Azure DevOps Learning Roadmap
Goal
Build practical Azure DevOps skills by learning to create, explain, troubleshoot, and improve CI/CD workflows—not just follow tutorials.
How I Will Learn
Use this cycle for each topic:
Understand → Practise → Break it → Troubleshoot → Explain it → Record the lesson
Study Session (60 minutes)
- 10 min: Learn one concept.
- 35 min: Complete a hands-on task.
- 10 min: Answer questions or troubleshoot a failure.
- 5 min: Explain what I learned in my own words.
Notes Rule
Do not write down videos word for word. For each topic, record only:
- What is it?
- Why is it needed?
- How does it work?
- Example
- Common failure and troubleshooting steps
Learning Roadmap
Level 0 — Azure DevOps Overview
Learn the purpose of each service and how they fit together:
- Organization and project
- Azure Boards
- Azure Repos
- Azure Pipelines
- Azure Artifacts
- Test Plans
- Agents and agent pools
- Environments and service connections
Hands-on: Explore the services in the practice project.
Level 1 — Git and Azure Repos
Learn and practise:
- Repositories, clone, status, add, commit, pull, and push
- Branches and merges
- .gitignore
- Pull requests
- Merge conflicts
- Branch policies and build validation
Outcome: Make a change on a feature branch, push it, open a pull request, and merge it safely.
Level 2 — Pipeline Fundamentals
Learn the pipeline hierarchy:
Pipeline
└── Stage
    └── Job
        └── Step / Task
Topics:
- YAML pipeline structure
- Microsoft-hosted and self-hosted agents
- Agent pools
- Scripts and built-in tasks
- Variables and predefined variables
- Triggers and conditions
- Pipeline logs and troubleshooting
Outcome: Create a pipeline, run it, deliberately introduce a failure, and explain how to fix it.
Level 3 — YAML Skills
Learn:
- Variables and parameters
- Expressions: ${{ }}, $ , and $( )
- Conditions
- Dependencies between stages and jobs
- Templates and reusable YAML
- Path and branch filters
Outcome: Build a readable, reusable pipeline without copying YAML blindly.
Level 4 — Continuous Integration (CI)
Build a pipeline that:
1. Starts when code is pushed.
2. Checks out the repository.
3. Installs dependencies.
4. Builds the application.
5. Runs tests.
6. Packages the output.
7. Publishes an artifact.
Practise troubleshooting broken builds, failed tests, missing dependencies, incorrect variables, paths, permissions, and missing artifacts.
Level 5 — Continuous Delivery / Deployment (CD)
Learn:
- Multi-stage pipelines
- Deployment jobs and environments
- Development, test, and production stages
- Environment-specific variables
- Approvals and checks
- Deployment history
- Rollback concepts
Outcome: Deploy the same build artifact through multiple environments with appropriate controls.
Level 6 — Security and Reuse
Learn:
- Service connections
- Secret variables and secure files
- Variable groups
- Azure Key Vault integration
- Repository and pipeline permissions
- Reusable templates
- Pipeline resources and artifact traceability
Outcome: Keep credentials out of source code and reuse common pipeline logic safely.
Level 7 — Classic and YAML Pipelines
Understand the differences between:
- Classic build pipelines
- Classic release pipelines
- YAML pipelines
Prioritise YAML for new practice while learning enough about Classic pipelines to understand existing enterprise systems.
Level 8 — End-to-End CI/CD Project
Build a small application pipeline that follows this flow:
Work item
   ↓
Git feature branch
   ↓
Pull request
   ↓
Build validation
   ↓
Merge
   ↓
Build and test
   ↓
Publish artifact
   ↓
Deploy to Dev
   ↓
Deploy to QA
   ↓
Approval
   ↓
Deploy to Production
Include variables, conditions, templates, artifacts, environments, approvals, secrets, deployment history, and troubleshooting where appropriate.
Personal Project — Build-to-Release Traceability
Problem
Identify exactly which source build, commit, artifact, configuration, and work items were included in a deployment.
Target Information
- Release identifier
- Pipeline and build number
- Commit ID
- Artifact name
- Target environment
- Deployment timestamp
- Related work items
- Configuration or schema version, where available
Example
Release: 596
Pipeline: Atrias-AX-Build
Build: 10.4.22
Commit: a8f92d1
Artifact: Atrias_AXMECOMSMainScheduledBuild_10.4.22
Environment: DEV
Deployment: 2026-09-28 18:42
Work Items: AB#1842, AB#1849
Use this project to practise preserving traceability between code changes, builds, artifacts, and deployments.
Learning Resources
- Hands-on environment: KodeKloud playground
- Official reference: Microsoft Learn — Azure DevOps
- Guidance: Use documentation to answer a specific question; do not try to read everything cover to cover.
Progress Tracker
Update this checklist only when the skill has been practised.
- [ ] Level 0 — Azure DevOps overview
- [ ] Level 1 — Git and Azure Repos
- [ ] Level 2 — Pipeline fundamentals
- [ ] Level 3 — YAML skills
- [ ] Level 4 — CI
- [ ] Level 5 — CD
- [ ] Level 6 — Security and reuse
- [ ] Level 7 — Classic vs YAML
- [ ] Level 8 — End-to-end CI/CD project
- [ ] Build-to-Release Traceability project
Definition of Done
A topic is complete when I can:
- Explain the concept in my own words.
- Perform the task without blindly following a tutorial.
- Troubleshoot at least one realistic failure.
- Explain what happened and why.
- Recreate the task after a short break without relying entirely on notes.
Rule: Practical ability matters more than the number of videos watched.
