# Example run: `/eli12` on the `git worktree` manual

This is a real run, not a mock-up. On 2026-10-20, Claude Code (Claude Opus 5.5) followed
[`SKILL.md`](../../SKILL.md) on one input: the DESCRIPTION section of `git help worktree`
(git 2.50.1). The text below is the output, unedited. The same text appears in the explainer
page and the video.

**Input** (excerpt from the git manual):

> A git repository can support multiple working trees, allowing you to check out more than one
> branch at a time. With git worktree add a new working tree is associated with the repository [...]
> This new worktree is called a "linked worktree" as opposed to the "main worktree" [...]
> When you are done with a linked worktree, remove it with git worktree remove.

**Output:**

Imagine you need to fix something urgent in a school project while your half-finished draft is spread all over your only desk.

Here is what `git worktree` does, step by step:

1. **A Second Desk for the Same Project ([`git worktree add`](https://git-scm.com/docs/git-worktree))**
   - A *working tree* (the folder where you see and edit the project's files) normally comes one per project. `git worktree add ../hotfix` sets up a second desk in a new folder and puts a new *branch* (a separate line of edits, like a fresh copy of your draft) called `hotfix` on it.

2. **One Shared Filing Cabinet ([git-worktree manual](https://git-scm.com/docs/git-worktree))**
   - Both desks hang off the same *repository* (the cabinet that keeps every saved version). Your first desk is the "main worktree"; extra desks are "linked worktrees". Your messy draft stays on desk one while you work at desk two.

3. **How They Connect Together**
   - You do the urgent fix at desk two, save it into the shared cabinet, then fold desk two away with `git worktree remove` and go back to your draft.
