## Objective

Learn how Git merge conflicts happen, how to identify conflicting changes, and how to resolve them without losing the intended work.

## Challenge

You must resolve a merge conflict deliberately created by the workshop bot.

### Instructions

1. Create a new branch from the latest default branch.
2. Create `task/<YOUR_ROLL_NUMBER>.md`.

   Example: `task/IIT2025099.md`

3. Be creative! Play around with markdown.
4. Commit your changes and open a Pull Request against the default branch.
5. The workshop bot will modify the same file on the default branch, creating a merge conflict.
6. Fetch the latest changes and resolve the conflict locally.
7. Commit your resolution and push the update to the same PR.

## Resolution Requirements

- Preserve your original introduction.
- Incorporate the bot's requested sentence.
- Remove all Git conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`).
- Do not close the PR and create a replacement merely to avoid the conflict.
- Do not modify workflow files or the bot's configuration.

## Useful Git Commands

Inspect the current branch and status:

```bash
git status
git branch
```

Fetch the latest default branch:

```bash
git fetch origin
```

Merge the latest default branch into your branch:

```bash
git merge origin/main
```

Replace `main` with the actual default branch name if different.

After resolving the file:

```bash
git add task/<YOUR_ROLL_NUMBER>.md
git commit -m "Resolve Task 3 merge conflict"
git push
```

If Git reports that the merge is still in progress, complete the resolution and commit before pushing.

## Pull Request Requirements

- Reference this issue using `Issue #1` in the PR description.
- Keep the same PR open throughout the challenge.
- Explain briefly what caused the conflict and how you resolved it.

## Completion Criteria

A maintainer verifies that the conflict was genuinely resolved, the required content is present, and the PR contains no conflict markers.

**No auto-merge:** Passing validation does not automatically merge the PR.
