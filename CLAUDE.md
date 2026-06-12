# NIK – Claude Code Instructions

## Deployment workflow

After every change: commit → push to feature branch → merge to `main` → user sees it live immediately.

Steps:
1. Make changes
2. `git add` + `git commit`
3. `git push -u origin <branch>`
4. Merge feature branch into `main` and push: `git checkout main && git merge <branch> && git push origin main && git checkout <branch>`

Always do this automatically unless told otherwise.
