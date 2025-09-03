---
title: "tmdr"
description: "Too Medical Didn't Read a CLI & TUI for medical acronyms"
date: "Aug 18 2025"
demoURL: "https://www.tmdr.sh"
repoURL: "https://github.com/anthony-langham/tmdr"
---

Too Medical; Didn’t Read

Introducing tmdr : a command line tool with optional TUI that provides clinical acronym context to engineers working in healthtech.

<img src="/tmdr-demo.gif" alt="TMDR" width="600"/>

In healthtech, engineers, analysts, and pm’s encounter a lot of medical acronyms:

- ABG
- GCS
- BNF

So much so we had acronym glossary pages at both suvera and babylon.

It’s a small problem, but a sticky one. Especially when you’re building, debugging, or trying to make product decisions in a clinical context.

## The Insight

This isn’t really a medical knowledge problem. It’s a **workflow** problem. Clinical acronyms aren’t going away. But the way we look them up? That could be definitely be better especially for people whos primary workflow is based around the terminal.

## The Solution

I built [`tmdr`](https://github.com/anthony-langham/tmdr) — **Too Medical; Didn’t Read**.

`tmdr` is a terminal native, offline tool for looking up clinical acronyms with zero friction and zero token burn.

```bash
$ tmdr abg
ABG → Arterial Blood Gas
A test measuring oxygen and carbon dioxide in arterial blood.
```

- No browser.
- No notion hunt.
- No LLM.
- No fluff.

Just the definition, where you need it.

Details:

- Written in Go
- Distributed via curl
- Styled with BubbleTea + Lip Gloss
- Fully open source

Install it with:

```bash
curl -fsSL https://tmdr.sh/install | bash
```

Or visit: [https://tmdr.sh](https://tmdr.sh)

## Why It Matters

- For engineers: less distraction, more flow
- For PMs: clarity in specs and sprint planning
- For ML teams: consistent terminology without burning tokens
- For me: a way to turn clinical experience into something useful

## What’s Next

This is a quick experiment to see how clinical context can be made more accessible to people working in the terminal.

If you're building in healthtech, and you’ve felt this friction before let me know your thoughts
