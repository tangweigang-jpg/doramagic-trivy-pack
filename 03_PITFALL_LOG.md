# Pitfall Log

## Pitfall 1: Security or permission risk requires verification

- Symptom: Project evidence flags a security or permission risk. Review the linked source before relying on this workflow.
- Likely cause: Security or permission risk
- How to verify: Reproduce the official install and quickstart path in an isolated environment.
- Recovery step: Stop, inspect the pitfall source, and rerun only after the boundary is clear.
- When to stop: Stop when license, tool permission, or host compatibility is unclear.
- Source/evidence: packet_text.keyword_scan | https://github.com/aquasecurity/trivy

## Doramagic Source Extract

# Pitfall Log

Project: aquasecurity/trivy

Summary: Found 11 structured pitfall item(s), including 1 high/blocking item(s). Top priority: Security or permission risk - Security or permission risk requires verification.

## 1. Security or permission risk - Security or permission risk requires verification

- Severity: high
- Evidence strength: source_linked
- Finding: Project evidence flags a security or permission risk. Review the linked source before relying on this workflow.
- User impact: May increase setup, validation, or first-run risk for the user.
- Evidence: packet_text.keyword_scan | https://github.com/aquasecurity/trivy

## 2. Installation risk - Installation risk requires verification

- Severity: medium
- Evidence strength: runtime_trace
- Finding: Project evidence flags a installation risk. Review the linked source before relying on this workflow.
- User impact: May increase setup, validation, or first-run risk for the user.
- Repro command: `docker run aquasec/trivy`
- Evidence: identity.distribution | https://github.com/aquasecurity/trivy

## 3. Configuration risk - Configuration risk requires verification

- Severity: medium
- Evidence strength: source_linked
- Finding: Project evidence flags a configuration risk. Review the linked source before relying on this workflow.
- User impact: May increase setup, validation, or first-run risk for the user.
- Evidence: community_evidence:github | https://github.com/aquasecurity/trivy/issues/10622

## 4. Capability evidence risk - Capability evidence risk requires verification

- Severity: medium
- Evidence strength: source_linked
- Finding: README/documentation is current enough for a first validation pass.
- User impact: May increase setup, validation, or first-run risk for the user.
- Evidence: capability.assumptions | https://github.com/aquasecurity/trivy

## 5. Runtime risk - Runtime risk requires verification

- Severity: medium
- Evidence strength: source_linked
- Finding: Project evidence flags a runtime risk. Review the linked source before relying on this workflow.
- User impact: May increase setup, validation, or first-run risk for the user.
- Evidence: packet_text.keyword_scan | https://github.com/aquasecurity/trivy

## 6. Maintenance risk - Maintenance risk requires verification

- Severity: medium
- Evidence strength: source_linked
- Finding: Project evidence flags a maintenance risk. Review the linked source before relying on this workflow.
- User impact: May increase setup, validation, or first-run risk for the user.
- Evidence: evidence.maintainer_signals | https://github.com/aquasecurity/trivy

## 7. Security or permission risk - Security or permission risk requires verification

- Severity: medium
- Evidence strength: source_linked
- Finding: no_demo
- User impact: May increase setup, validation, or first-run risk for the user.
- Evidence: downstream_validation.risk_items | https://github.com/aquasecurity/trivy

## 8. Security or permission risk - Security or permission risk requires verification

- Severity: medium
- Evidence strength: source_linked
- Finding: no_demo
- User impact: May increase setup, validation, or first-run risk for the user.
- Evidence: risks.scoring_risks | https://github.com/aquasecurity/trivy

## 9. Security or permission risk - Security or permission risk requires verification

- Severity: medium
- Evidence strength: source_linked
- Finding: Project evidence flags a security or permission risk. Review the linked source before relying on this workflow.
- User impact: May increase setup, validation, or first-run risk for the user.
- Evidence: community_evidence:github | https://github.com/aquasecurity/trivy/issues/10859

## 10. Maintenance risk - Maintenance risk requires verification

- Severity: low
- Evidence strength: source_linked
- Finding: issue_or_pr_quality=unknown。
- User impact: May increase setup, validation, or first-run risk for the user.
- Evidence: evidence.maintainer_signals | https://github.com/aquasecurity/trivy

## 11. Maintenance risk - Maintenance risk requires verification

- Severity: low
- Evidence strength: source_linked
- Finding: release_recency=unknown。
- User impact: May increase setup, validation, or first-run risk for the user.
- Evidence: evidence.maintainer_signals | https://github.com/aquasecurity/trivy

