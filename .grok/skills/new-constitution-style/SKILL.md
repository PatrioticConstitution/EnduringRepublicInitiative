---
name: new-constitution-style
description: >-
  Apply the review principles for new/constitution.md. Use when reviewing
  changes, running /review, /new-constitution-style, or a code review, and
  when editing new/constitution.md.
---

# New constitution review

The principles have one home: `new/AGENTS.md`. Read that file before you edit `new/constitution.md`, and before you review a diff that touches it.

The bundled review skill decides how a review runs. This skill adds those principles to that review. When you launch a reviewer subagent and the diff touches `new/constitution.md`:

1. Read `new/AGENTS.md`.
2. Append its full text to the reviewer prompt, after the review skill's template.
3. Leave that text in the prompt. Its opening tells the reviewer the severity and the scope, including the override of the persona rule that a style preference is not a bug.

A diff that does not touch `new/constitution.md` skips this skill. Leave `amended/` in its historical form.
