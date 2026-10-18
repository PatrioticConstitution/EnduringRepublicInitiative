---
name: new-constitution-style
description: >-
  Enforce the style of new/constitution.md on review and on edit. Use when
  reviewing changes, running /review, /new-constitution-style, or a code
  review, and when editing new/constitution.md, including its capitalization,
  spelling, and grammar.
---

# New constitution style

The rules have one home: `new/AGENTS.md`. Read that file before you edit `new/constitution.md`, and before you review a diff that touches it.

The bundled review skill decides how a review runs. This skill adds the standard to that review. When you launch a reviewer subagent and the diff touches `new/constitution.md`:

1. Read `new/AGENTS.md`.
2. Append its full text to the reviewer prompt, after the review skill's template.
3. Leave that text in the prompt. Its opening tells the reviewer the severity and the scope, including the override of the persona rule that a style preference is not a bug.

A diff that does not touch `new/constitution.md` skips this skill. Leave `amended/` in its historical form.
