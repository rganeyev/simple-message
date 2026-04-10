# Simple Message

A minimal, full-screen message board hosted on GitHub Pages.

## How it works

- The current message is stored in [`message.txt`](./message.txt) in this repository.
- The website reads that file directly via the **GitHub Contents API** — no backend required.
- The page auto-refreshes the message every **30 seconds**.

## Setting a new message

1. Open the live site.
2. Click anywhere on the screen.
3. Type your new message in the dialog.
4. Enter a **GitHub Personal Access Token** with `repo` (or `public_repo`) scope.
   - Create one at <https://github.com/settings/tokens>
   - The token is held in memory only and never persisted.
5. Press **Save** (or Ctrl/Cmd + Enter).

The message is written back to `message.txt` via the GitHub API and will be visible to all viewers within ~30 seconds (the next auto-refresh cycle).

## Live site

<https://rganeyev.github.io/simple-message/>
