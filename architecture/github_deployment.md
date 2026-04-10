# SOP: GitHub Deployment

## Objective
Deploy the local codebase to a new GitHub repository while maintaining a clean history and including project planning metadata.

## Prerequisites
- Repository created on GitHub.
- Local git initialized.
- Remote URL: `https://github.com/iamShaaan/Plumbing-Landing-page.git`

## Layer 2 Execution Steps
1. **Prepare Remotes:**
   - Rename existing `origin` to `legacy_remote`.
   - Add new `origin` pointing to `https://github.com/iamShaaan/Plumbing-Landing-page.git`.
2. **Stage Files:**
   - Add all files including documentation (`claude.md`, `task_plan.md`, `findings.md`, `progress.md`, `gemini.md`).
   - Ensure `.tmp` and `.git` are excluded.
3. **Commit:**
   - Initial commit for the new repository structure.
4. **Push:**
   - Push to `main` branch.

## Edge Cases
- **Branch Discrepancy:** If local branch is not `main`, rename it to `main`.
- **Merge Conflicts:** Force push if the remote is empty (standard for initial push).
