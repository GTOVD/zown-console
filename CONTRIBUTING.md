# Contributing to Zown Console

This is the visual face of the Zown ecosystem. All contributions must maintain high visual fidelity and follow the professional Git Flow.

## 🛠 The Zown Atomic Pipeline (Git Flow)

### 1. Task Acquisition
- **Source of Truth**: [GitHub Issues](https://github.com/GTOVD/zown-console/issues).
- **Selection**: Choose a P1 issue (Modular Engine or Live Monitoring).

### 2. Branching & Linking
- **Branch Name**: `feat/CONSOLE-XXX-description` (Always branch from `develop`).
- **Linking**: Comment on the GitHub issue: `Started work in branch feat/CONSOLE-XXX`.

### 3. State Synchronization (Mandatory)
Before a PR is considered complete, you **MUST** update the following project files:
- **MEMORY.md**: 
  - Move the completed Issue from "Active Backlog" to "Strategic Milestones."
  - Update the "Technical State" (e.g., when a widget moves from mock to live data).
- **SOUL.md / IDENTITY.md**: Update if the visual theme or the scope of the command center evolves.

### 4. Pull Requests (PRs)
- **Target**: All PRs must target the `develop` branch.
- **Auto-Closing**: PR descriptions must include `Closes #XXX`.
- **Review**: PRs must be audited for layout stability, mobile responsiveness, and adherence to the "Dark/Gold" theme.

### 5. Integration & Promotion
- **Step A**: Merge PR into `develop`.
- **Step B**: Promote `develop` to `main`:
  ```bash
  git checkout main && git merge develop && git push origin main
  ```

## 🏁 Definition of Done
- Implementation matches the Acceptance Criteria.
- **Identity, Soul, and Memory files are synchronized.**
- UI passes visual inspection for the "Dark/Gold" luxury aesthetic.
- PR is merged into `develop` and promoted to `main`.
- The linked GitHub Issue is closed.
