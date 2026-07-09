# Contributing

This repo collects lateral thinking techniques as agent skills. Contributions are welcome, and the bar is specific — please read it before writing.

## What we accept

- **New techniques**, with provenance. The technique must come from somewhere: a named author, a book, a documented practice. We do not accept invented "methods" dressed up with a citation-shaped sentence.
- **New reference material** for existing techniques: stimulus entries, analogy domains, SCAMPER questions, provocation templates.
- **Worked examples from real sessions.**
- **Fixes**: broken links, unclear steps, typos, structural problems.

## The quality bar

**Every technique must have honesty mechanics.** Two things, non-negotiable:

1. **An abandonment rule.** A stated condition under which the technique gives up on a line of thought, and an instruction to show that abandonment to the user. If every stimulus, provocation, or flip in a session produces a usable idea, the session was faked — and a reader can tell. The visible failures are what make the successes credible.
2. **A meta-pattern step.** After the batch, scan across the results for the structural insight that recurs. The individual ideas matter less than what they have in common.

**Worked examples come from real sessions.** Run the technique. On a real problem. Include the abandonments that actually happened. Do not compose a plausible transcript — the difference is visible, and a fabricated example undermines the one thing this repo is for.

**Descriptions use technique-specific triggers only.** Generic stuck-ness language is reserved for the `lateral` router:

> `I'm stuck` · `going in circles` · `need fresh ideas` · `try a different angle`

If a technique's description claims those phrases, it competes with the router for auto-invocation and routing becomes unpredictable. Describe what *your* technique is for, in its own words.

## The template

Every technique `SKILL.md` has exactly these sections, in this order:

```markdown
---
name: <technique>
description: <technique-specific triggers only>
---

# <Technique Title>

## What this technique does
<3–4 sentences + provenance line: source, author, year.>

## Workflow
### Step 1: Confirm the target
<What a valid target looks like; one focused question to ask if unclear;
refusal rule: refuse requests to PERFORM analytical work (debug this,
review this code, implement this) — suggest an analytical approach
instead. Redesigning or ideating about such a process is a valid
creative target (e.g., "reinvent our code-review ritual" is in scope;
"review this PR" is not).>
### Step 2..N: <technique-specific>

## Honesty mechanics
<The technique's abandonment rule + meta-pattern step.>

## What NOT to do
<Bulleted anti-patterns.>

## References
<Relative links to files in ./references/.>
```

## Compatibility rules

These skills run across different agents. Keep them portable:

- **Frontmatter is `name` and `description` only.** No other keys.
- **No tool-specific syntax** in any skill body: no agent names, no slash-commands, no vendor-specific formatting conventions. The single exception is the router's fallback, which may name the portable installer `npx skills add danium/lateral-thinking`.
- **Relative paths only.** Reference a sibling technique as `../<technique>/SKILL.md`, never an absolute path.
- **English only**, plain markdown.

## How to propose

1. **Open an issue first** for a new technique. State the technique, its provenance, and which symptom it addresses that no existing technique covers. The `lateral` router's decision table maps one symptom to one technique — a new entry needs a symptom of its own.
2. **Then open a PR** following the template above.

For reference material and fixes, a PR without a prior issue is fine.
