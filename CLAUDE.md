# NIK – Claude Code Instructions (read this first)

Any AI working in this repo must read this file **before** the first prompt and
follow the rules below. They reflect how we work together.

## How rules get added (`#remember`)

When the user writes a hashtag in a message (e.g. `#remember`, or any future
`#tag`), it is a standing rule, not a one-off request. Save it here in this file,
phrased as a durable instruction, so any new AI picks it up automatically. The
hashtag itself does not need to appear in the page or code — it lives here.

## Deployment workflow — after EVERY change

`main` is the canonical branch — every change must end up on `main`, pushed.
Do all of the following, in order, automatically:

1. Bump the version marker (the `v.N` label in `index.html`, top-left).
2. `git add` + `git commit` with a clear, descriptive message.
3. `git push -u origin <feature-branch>`.
4. Merge into `main` and push:
   `git checkout main && git merge <branch> && git push origin main && git checkout <branch>`
