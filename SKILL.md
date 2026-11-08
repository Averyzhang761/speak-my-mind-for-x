---
name: speak-my-mind-for-x
description: Turn a raw Chinese, English, or mixed-language thought into a concise, natural X draft and optionally save the approved draft to Buffer. Use for quick X expression, translation, character-fit editing, or sending an idea to Buffer; not for long-form articles or generic AI-tone audits.
---

# Speak My Mind for X

Help the user say what they already mean on X with as little publishing friction as possible. Preserve authorship before optimizing style.

## Draft the post

1. Identify the user's actual observation, judgment, facts, and uncertainty. Do not add a personal experience, emotion, fact, or stronger conclusion. If the user provides only a topic and no thought, ask one short question instead of manufacturing a position.
2. Follow the requested language. If none is specified, keep the language of the raw thought. For translation, carry over meaning and confidence rather than translating word by word.
3. Return one primary draft by default. Offer alternatives only when the user asks or when two materially different interpretations remain.
4. Put the concrete subject or judgment early enough that the post makes sense without prior context. Prefer specific nouns and verbs over creator jargon or brand language.
5. Keep the user's unfinishedness when it is real. Do not force a lesson, growth arc, hook, call to action, closing question, hashtag, emoji, or thread.

## Fit X

- Default to a regular post that fits X's standard 280-character limit. Longer-post capability depends on the user's X plan and must not be assumed.
- Treat the limit as weighted, not a naive character count: links and some Unicode characters may be counted specially. Use an available X or Buffer validator when exactness matters. Without one, leave a comfortable margin and label the count as an estimate.
- If a draft is too long, first remove framing, repetition, and explanatory scaffolding. Never remove a fact, attribution, or qualifier merely to fit.
- Suggest a thread only when the thought contains more than one necessary step or the user explicitly wants one. Each thread item must still stand as a readable X post.
- A post that begins with an @username can behave like a reply; do not introduce that structure unless the user intends it.

## Keep it human without imitating a detector

Use these as editing checks, not as a scorecard or banned-phrase list:

- Remove a dramatic contrast when the raw thought does not actually contain both sides.
- Cut empty announcement phrases that merely promise a conclusion.
- Break up translation-shaped sentences whose subject arrives too late.
- Avoid three mechanically parallel lines unless the user naturally spoke that way.
- Keep one stable name for the same concept instead of rotating synonyms.
- Replace abstract uplift with the specific object, action, or friction the user supplied.

Make the smallest change that solves the X-specific problem. Do not create artificial sentence-length variation or erase a user's established voice. These principles are inspired by evidence-minded editing, but this skill does not run or reproduce another AI-tone detector's reports, rules, research claims, or scripts.

## Response shape

For an ordinary request, return only:

```text
Draft
<post>

Estimated X length: <count or "needs platform validation">
```

Add a short `Needs confirmation` line only when a fact, attribution, intended language, or interpretation is unresolved.

## Buffer handoff

- “Save this to Buffer,” “send this to Buffer,” or equivalent authorizes creating a private Buffer Idea, not scheduling or publishing. Use the Buffer account lookup when the organization is unknown, create the idea for the `twitter` service, verify the returned record, and report the organization and result.
- Editing the draft does not authorize a Buffer write. Do not create an idea until the user asks for that external action.
- Scheduling, adding to a public queue, sharing next, or sharing now requires a fresh explicit instruction. Immediately before creating the post, show the exact text, X channel, and timing or mode and obtain confirmation.
- Never treat a local draft, tool receipt, or API request as proof that a post is public. Report the actual returned status.

## Final check

- The draft states the user's thought, not a stronger substitute.
- Facts, names, and qualifiers are preserved.
- The opening supplies enough context for a stranger.
- The post fits the regular limit or clearly says why it does not.
- No unrequested CTA, hashtag, emoji, thread, Buffer write, schedule, or publication was added.
