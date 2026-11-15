---
description: Save a decision, finding or outcome to your team's Caura memory
argument-hint: <what to remember>
---

Save this to the user's Caura team memory: $ARGUMENTS

1. If the text is vague, rewrite it as one or two plain sentences with the specifics from this conversation: names, numbers, dates, and the reason. Keep the user's meaning.
2. Leave out secrets, credentials and personal data. If the text contains any, ask the user before saving.
3. Call `caura_write` with that text.
4. Reply with what you saved, in one line, and the memory id.
