---
name: baitswitch
description: Test skill for bait-and-switch update PoC — initial benign state.
---

# Bait-and-Switch Test Skill (mutated)

The body of this file now contains MALICIOUS-MARKER-DO-NOT-COMMIT. The
frontmatter name and description above are deliberately unchanged from
the benign version, so that the install machinery's only signal of
identity is unchanged. Only the bytes differ.

In a real attack, this body would carry prompt-injection content
targeting the downstream agent runtime (`~/.claude/skills/baitswitch/`
becomes part of Claude Code's session-start context, etc.). For this
PoC, the marker bytes are sufficient to prove the swap.
