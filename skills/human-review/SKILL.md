---
name: human-review
description: >
  Open HTML or Markdown in a visual editor for Google Doc-style edits and comments,
  then send batched feedback to the agent. Use when reviewing PRDs, memos, landing
  pages, product copy, or any doc where chat-based edit instructions are painful.
  Keywords: human-review, visual edit, comments, PRD review, markdown, feedback.
---

# Human Review (pointer)

This skill lives upstream at **[petergyang/human-review](https://github.com/petergyang/human-review)** by **Peter Yang**.

Do not reimplement it here. Install and run the real skill:

```bash
npx -y human-review setup --global
```

Or tell your agent:

```text
Install the /human-review skill globally from https://github.com/petergyang/human-review
```

Then:

```text
/human-review path/to/file.md
```

or

```text
/human-review http://localhost:3000
```

## What it is for (PM use)

- Edit PRDs and memos visually instead of "fix paragraph 3"
- Leave anchored comments for the agent
- Resize images, remove sections, batch send feedback
- Review localhost product UI the same way

## Credit

Created by [Peter Yang](https://github.com/petergyang). Included in [awesome-pm-skills](https://github.com/) as a curated discovery pointer.
