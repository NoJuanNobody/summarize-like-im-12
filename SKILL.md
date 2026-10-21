---
name: summarize-like-im-12
description: Summarize complex codebases, multi-agent trajectories, research papers, or system architectures as if explaining to a sharp 12-year-old. Uses vivid analogies, zero unexplained jargon, step-by-step story flow, and clickable links to real code files. Triggers on "summarize like im 12", "explain like im 12", "/summarize-like-im-12", "/eli12", or "break this down simply".
---

# Summarize Like I'm 12 (`summarize-like-im-12`)

Turns dense technical architectures, multi-agent build logs, academic papers, or repository diffs into crystal-clear, engaging explanations written for a curious, sharp 12-year-old—without dumbing down the truth or losing links to the actual files.

## Core Principles

1. **Hook First with a Real-World Analogy**:
   - Start with a one-sentence setup comparing the system to something tangible (a vending machine, a walkie-talkie squad, a LEGO factory line, a library with a secret coin slot).
2. **Translate Every Jargon Term on First Use**:
   - Never drop terms like *Git worktree*, *GraphRAG*, *zk-SNARK*, *KV-cache*, or *SLURM* without an immediate everyday translation in parentheses:
     - *Git worktree* → "giving each robot builder its own separate desk so they don't bump elbows"
     - *GraphRAG* → "connecting notes like a giant spiderweb of clues instead of a messy pile of pages"
     - *Cryptographic hash (SHA-256)* → "a digital wax seal that breaks if anyone changes even one letter"
     - *Paywall API ($0.05)* → "a digital coin slot that charges 5 cents—like a library printer—every time someone's AI asks a question"
3. **Numbered Story Beats ("What We Built & Why It Matters")**:
   - Group the explanation into 3–5 numbered sections with punchy titles (`1. The Idea Harvester`, `2. Six Robot Builders at Separate Desks`, etc.).
4. **Keep Real Clickable Code Links**:
   - Even though the language is simple and fun, always link to the real files, scripts, and GitHub URLs so the reader can click straight into the code.
5. **No Condescension**:
   - A 12-year-old understands games, money, teams, robots, servers, and logic—just skip the academic fluff and get straight to how the machine works.

## Output Template

```markdown
Imagine [1-sentence relatable setup of the problem].

Here is what we built, step by step:

1. **[Catchy Name for Component 1] ([`repo-or-file`](file:///path/to/file))**
   - [Plain-English explanation + concrete analogy + what it actually does].

2. **[Catchy Name for Component 2] ([`repo-or-file`](file:///path/to/file))**
   - [Plain-English explanation + concrete analogy + what it actually does].

3. **[How They Connect Together]**
   - [1-2 sentences showing how all the pieces pass the baton from start to finish].
```

## CLI Usage

```bash
# Summarize a file, markdown doc, or text string using the ELI12 formatter
summarize-like-im-12 --input README.md
```
