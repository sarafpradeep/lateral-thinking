# lateral-thinking

**Your AI agent's ideas are predictable. These skills fix that.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
![Skills: 9](https://img.shields.io/badge/skills-9-blue.svg)

Eight lateral thinking techniques — de Bono, Eberle, Gordon — plus a router that diagnoses how you're stuck and picks the right one.

---

## The demo

Same agent. Same prompt. One of them read a skill first.

> **Prompt:** *"Suggest names for a feature that shows users which parts of their codebase change most often."*

<table>
<tr>
<th width="50%">Any agent, vanilla</th>
<th width="50%">Same agent, <code>random-stimulus</code></th>
</tr>
<tr valign="top">
<td>

**Direct and descriptive**
- **Change Frequency** — plainly says what it measures.
- **Change Hotspots** — "hotspots" is already common vocabulary in this space.
- **Churn Map** — "code churn" is an established metric.
- **File Activity** — broad and neutral.

**Hotspot / heat metaphor**
- **Hotspots** — the metaphor does the explaining for you.
- **Code Heatmap** — more color = more activity.
- **Hot Zones** — a softer take on hotspots.

**Insight / analytics framing**
- **Churn Insights** — positions it as analytics.
- **Code Pulse** — a heartbeat of the codebase.
- **Activity Radar** — suggests ongoing monitoring.

*(15 names, competently reasoned.)*

</td>
<td>

🌋 **The fault line**
Two plates grind past each other. Stress accumulates invisibly. The line is mapped *because* it's dangerous.

→ Files that change constantly aren't the danger. The danger is where two **teams** grind against the same file.

**Faultline** — churn × distinct authors. Not "what changes" but *what changes under contention.*

🦩 **The heron stalking**
Absolute stillness, then one strike. The stillness *is* the technique.

→ Then the *stillest* files are the interesting ones.

**Heron** — inverts the brief. Shows what **hasn't** changed, and asks if that's maturity or abandonment.

🐜 **The termite mound** — collapses into the fault-line idea, and every name it yields is worse. **Abandoned.**

</td>
</tr>
</table>

The vanilla answer isn't bad. It's *good* — and every name in it is a synonym for "the thing that changes." Fifteen names, one idea.

The technique produced different **concepts**: churn against contention, churn against ownership, churn against time. Then it found the meta-pattern the exercise was really about — *raw churn isn't the signal; churn is only meaningful against a second axis* — and that's why two of the eight stimuli were abandoned. They restated churn as a prettier picture of itself.

[See the full session →](skills/random-stimulus/references/worked-example.md)

---

## Install

**Any agent (recommended):**

```bash
npx skills add danium/lateral-thinking
```

**Claude Code (plugin):**

```
/plugin marketplace add danium/lateral-thinking
/plugin install lateral-thinking@lateral-thinking
```

**Codex:** ask `$skill-installer` to install from `https://github.com/danium/lateral-thinking`

**Manual:** clone and copy `skills/*` into your agent's skills directory.

> The toolkit installs as one bundle — the `lateral` router needs its sibling techniques.

---

## Pick your technique

| Symptom | Technique |
|---|---|
| Ideas all feel the same; brainstorm output is predictable | [`random-stimulus`](skills/random-stimulus/SKILL.md) |
| A constraint or rule feels unbreakable | [`provocation`](skills/provocation/SKILL.md) |
| Requirements assume things nobody has questioned | [`inversion`](skills/inversion/SKILL.md) |
| We might be solving the wrong problem | [`concept-fan`](skills/concept-fan/SKILL.md) |
| The solution works but feels derivative | [`analogy`](skills/analogy/SKILL.md) |
| We have one idea and need variations | [`scamper`](skills/scamper/SKILL.md) |
| A decision is being made too fast / everyone agrees | [`six-hats`](skills/six-hats/SKILL.md) |
| Everything feels timid, safe, cautious | [`worst-idea`](skills/worst-idea/SKILL.md) |

Or just tell your agent **"use the lateral skill"** and let it diagnose you.

---

## Anatomy of a session

Every technique in this repo is required to fail in public. Here is `scamper` refusing to pad its own output, mid-session:

> **Substitute:** nothing new. The command is already swapped down to one line, and the only meaningful substitution (git for installer) already ships as a channel. Moving on.
>
> **Put to other use:** empty. The install does one job and generates no by-product worth repointing. Moving on.
>
> **Reverse / Rearrange:** empty as a distinct idea. The one real reversal (router-first, siblings later) is Variant D under another name, so it counts once. Nothing else to flip. Moving on.

Three of seven operations came up empty — and the last one had a genuine hit that it *disqualified for being a duplicate.*

This is the whole point. An agent that produces seven strong ideas from seven prompts is pattern-matching on the shape of a good answer, and you can't tell which ideas it actually believes. Every skill here carries an **abandonment rule** — a stated condition for giving up, and an instruction to show you when it does. The visible failures are what make the rest credible.

The second requirement is a **meta-pattern step**: after the batch, scan across what landed and name the structural insight. In that `scamper` session, the empty operations *were* the finding — the install command's surface is already tight, so the softness had to be somewhere else. It was: in the unstated dependency between the router and its siblings.

---

## What this is (and isn't)

These are real methods, sourced:

- **Random Stimulus**, **Provocation (Po)**, **Concept Fan** — Edward de Bono, *Lateral Thinking* (1970), *Po: Beyond Yes and No* (1972), *Serious Creativity* (1992)
- **Six Thinking Hats®** — Edward de Bono (1985). A registered trademark of the de Bono Group; this is an independent educational implementation.
- **SCAMPER** — Bob Eberle (1971), building on Alex Osborn's checklist
- **Forced Analogy** — Synectics, William J.J. Gordon (1961)
- **Assumption Inversion** — classical dialectic; "invert, always invert" (Carl Jacobi, via Charlie Munger)
- **Worst Possible Idea** — reverse brainstorming; standard in the d.school/IDEO toolkit

**This is not magic and it is not a prompt pack.** It is structured divergence with quality rules attached. The techniques constrain *how* an agent generates, and the honesty mechanics constrain what it's allowed to claim afterward.

**On invocation:** auto-invocation is best-effort — your agent may or may not reach for a skill on its own, and that depends on the agent. Explicit invocation always works: name the skill, or name the router.

---

## Contributing

New techniques need provenance and honesty mechanics. Worked examples must come from real sessions. See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

[MIT](LICENSE)
