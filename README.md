# Speak My Mind for X

A small Codex skill for turning a passing Chinese, English, or mixed-language thought into one natural X draft.

It is designed for the moment when you have something to say but do not want to turn it into a polished “content piece.” The skill preserves the original judgment, adapts it to X, checks whether it fits a regular post, and can optionally save an approved draft as a private Buffer Idea.

## What it does

- Keeps the author's meaning, uncertainty, and voice
- Produces one primary X draft instead of a wall of variants
- Handles Chinese-to-English or English-to-Chinese adaptation
- Accounts for X's standard post limit and suggests a thread only when needed
- Avoids forced hooks, hashtags, emoji, calls to action, and inflated conclusions
- Sends content to Buffer only when explicitly requested

## Install

Install it with the Skills CLI:

```bash
npx skills add Averyzhang761/speak-my-mind-for-x
```

Or clone/download the repository and place the folder in your Codex skills directory:

```bash
~/.codex/skills/speak-my-mind-for-x/
```

Restart or reload Codex so the skill can be discovered.

## Use

Invoke the skill explicitly:

```text
Use $speak-my-mind-for-x:
我刚想到，很多人不是没有观点，只是把每条 X 都当成正式发表，心理门槛就变高了。帮我发成英文。
```

To save the approved result as a private idea:

```text
Send this draft to Buffer as an idea.
```

Saving a Buffer Idea is not publishing. Scheduling or publishing requires a separate, explicit confirmation.

## Compatibility

The skill itself is plain Markdown. Buffer handoff requires a compatible Buffer connector in the host agent. Availability in a mobile ChatGPT or Codex client depends on whether that client can access installed skills and the connected Buffer account.

## Design note

The editing approach was inspired in part by the minimal-change and information-preservation discipline in [Lieflat Less AI Tone](https://github.com/larashero3-dotcom/lieflat-less-ai-tone). This repository does not copy that project's detector, research claims, scoring system, rules, examples, or scripts.

X's current help documentation describes the regular post limit as 280 characters and longer posts as a subscription feature: [How to Post](https://help.x.com/en/using-x/how-to-post) · [Types of Posts](https://help.x.com/en/using-x/types-of-posts).
