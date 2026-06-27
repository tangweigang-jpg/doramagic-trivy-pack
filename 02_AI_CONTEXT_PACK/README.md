# AI Context Pack

## Pack Identity

- Upstream: https://github.com/aquasecurity/trivy
- Pack type: Security Scanner Context Pack
- Doramagic canonical: https://doramagic.ai/en/projects/trivy/
- Relationship: independent pack; not affiliated or endorsed unless explicitly stated.

## Operating Rules

- Evidence first.
- No official endorsement claim.
- Run evals before claiming success.
- Use pitfall and risk files for recovery.

## Host Files

- `../AGENTS.md`
- `../CLAUDE.md`

## Doramagic Source Extract

# trivy - Doramagic AI Context Pack

> Purpose: pre-work context for the user's host AI. This pack does not prove that the project has been installed, run, or validated.

## Project

- canonical_name: `aquasecurity/trivy`
- capability: Find vulnerabilities, misconfigurations, secrets, SBOM in containers, Kubernetes, code repositories, clouds and more
- expected_user_outcome: Find vulnerabilities, misconfigurations, secrets, SBOM in containers, Kubernetes, code repositories, clouds and more

## Operating Boundaries

- Do not claim that the project has been installed, run, called through an API, or used on local files unless separate evidence proves it.
- Project facts must come from repo evidence, Claim Graph, or explicit source references.
- When a capability is not verified, mark it as unverified instead of completing it as fact.
- publish_status: `publishable`
- blocking_gaps: none

---

## Doramagic Context Augmentation

The following sections strengthen the repository context for a host AI. Human Manual data is a reading route, and pitfall notes become operating constraints.

## Human Manual Outline

Usage rule: this is only a reading route and salience signal, not factual authority. Concrete claims must still return to repo evidence or Claim Graph.

Host AI hard rules:
- Do not treat page titles, section order, summaries, or importance values as factual project evidence.
- When explaining the Human Manual outline, state that it is only a reading route or salience signal.
- Capability, installation, compatibility, runtime state, and risk claims must cite repo evidence, source paths, or Claim Graph.

- **Trivy Overview and Getting Started**: importance `high`
  - source_paths: README.md, cmd/trivy/main.go, pkg/commands/app.go, docs/getting-started/installation.md, docs/getting-started/index.md
- **System Architecture and Core Components**: importance `high`
  - source_paths: cmd/trivy/main.go, pkg/commands/app.go, pkg/commands/artifact/run.go, pkg/commands/artifact/scanner.go, pkg/commands/server/run.go
- **Scanning Capabilities: Vulnerabilities, Misconfigurations, Secrets, Licenses, and IaC**: importance `high`
  - source_paths: pkg/detector/ospkg/detect.go, pkg/detector/library/detect.go, pkg/detector/library/driver.go, pkg/dependency/parser/library/all/import.go, pkg/iac/scanners/scanner.go
- **Configuration, Output Formats, Reporting, Plugins, and Operations**: importance `high`
  - source_paths: pkg/flag/options.go, pkg/flag/report_flags.go, pkg/flag/scan_flags.go, pkg/flag/db_flags.go, pkg/flag/cache_flags.go

## Repo Inspection Evidence

- repo_clone_verified: true
- repo_inspection_verified: true
- repo_commit: `13de603dce17f5c6114a010d6aed6a440993edb0`
- inspected_files: `Dockerfile`, `README.md`, `docs/commercial/compare.md`, `docs/commercial/contact.md`, `docs/community/contribute/checks/overview.md`, `docs/community/contribute/checks/service-support.md`, `docs/community/contribute/discussion.md`, `docs/community/contribute/issue.md`, `docs/community/contribute/pr.md`, `docs/community/contribute/vulnerability-database/add-vulnerability-source.md`, `docs/community/contribute/vulnerability-database/overview.md`, `docs/community/maintainer/backporting.md`, `docs/community/maintainer/help-wanted.md`, `docs/community/maintainer/pr-review.md`, `docs/community/maintainer/release-flow.md`, `docs/community/maintainer/triage.md`, `docs/community/principles.md`, `docs/ecosystem/cicd.md`, `docs/ecosystem/ide.md`, `docs/ecosystem/index.md`

Host AI hard rules:
- Without repo_clone_verified=true, do not claim that the source code has been read.
- Without repo_inspection_verified=true, do not write README, docs, or package-file conclusions as facts.
- Without quick_start_verified=true, do not claim that the Quick Start path has run successfully.

## Doramagic Pitfall Constraints

These rules come from Doramagic discovery, validation, or compilation findings. The host AI must treat them as operating constraints, not background notes.

### Constraint 1: Security or permission risk requires verification

- Trigger: Project evidence flags a security or permission risk. Review the linked source before relying on this workflow.
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: packet_text.keyword_scan | https://github.com/aquasecurity/trivy
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 2: Installation risk requires verification

- Trigger: Project evidence flags a installation risk. Review the linked source before relying on this workflow.
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: identity.distribution | https://github.com/aquasecurity/trivy
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 3: Configuration risk requires verification

- Trigger: Project evidence flags a configuration risk. Review the linked source before relying on this workflow.
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: community_evidence:github | https://github.com/aquasecurity/trivy/issues/10622
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 4: Capability evidence risk requires verification

- Trigger: README/documentation is current enough for a first validation pass.
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: capability.assumptions | https://github.com/aquasecurity/trivy
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 5: Runtime risk requires verification

- Trigger: Project evidence flags a runtime risk. Review the linked source before relying on this workflow.
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: packet_text.keyword_scan | https://github.com/aquasecurity/trivy
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 6: Maintenance risk requires verification

- Trigger: Project evidence flags a maintenance risk. Review the linked source before relying on this workflow.
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: evidence.maintainer_signals | https://github.com/aquasecurity/trivy
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 7: Security or permission risk requires verification

- Trigger: no_demo
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: downstream_validation.risk_items | https://github.com/aquasecurity/trivy
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 8: Security or permission risk requires verification

- Trigger: no_demo
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: risks.scoring_risks | https://github.com/aquasecurity/trivy
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 9: Security or permission risk requires verification

- Trigger: Project evidence flags a security or permission risk. Review the linked source before relying on this workflow.
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: community_evidence:github | https://github.com/aquasecurity/trivy/issues/10859
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 10: Maintenance risk requires verification

- Trigger: issue_or_pr_quality=unknown。
- Host AI rule: Reproduce the official install and quickstart path in an isolated environment.
- Why it matters: May increase setup, validation, or first-run risk for the user.
- Evidence: evidence.maintainer_signals | https://github.com/aquasecurity/trivy
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

