---
name: random-stimulus
description: Edward de Bono's Random Stimulus technique — force-fit a random unrelated object, place, or phenomenon onto a creative target to break familiar association patterns. Use for product ideation, feature naming, brand direction, copywriting, architecture and design choices when ideas from outside the problem space would help. Triggers include "random stimulus", "random word", "force-fit", "de Bono", "inject a random object", "stare out the window", "see the tree and squeeze an idea". Do NOT use for analytical work like debugging, code review, or implementation tasks.
---

# Random Stimulus

## What this technique does

Pick a random thing from outside the problem space — a tree, a glacier, a kettle. List its properties. Force a connection to the target. See what falls out.

The first force-fit is usually trash. The third or fourth is where real ideas appear. The technique works because staying inside the problem space routes you through familiar associations; an external stimulus breaks the routing and forces a fresh trajectory through the same target. The stimulus has a *structural property* — cyclical, layered, swarming, ephemeral, branching — that the target could have but doesn't yet. That mismatch is where new designs hide.

Source: Edward de Bono, *Lateral Thinking: Creativity Step by Step* (1970), specifically the Random Word / Random Object method.

## Workflow

### Step 1: Confirm the target

A valid target is a concrete creative problem: names for a feature, ideas for a product, a novel onboarding flow, how to position a brand. If the target is unclear, ask one focused question — "What's the creative problem, and are there hard constraints?" Default batch size is 8–12 stimuli.

Refuse requests to *perform* analytical work — debugging, reviewing code, implementing a change — and suggest an analytical approach instead. Redesigning or ideating about such a process is a valid creative target: "reinvent our code-review ritual" is in scope; "review this PR" is not.

### Step 2: Pull stimuli

Draw 8–12 stimuli from [`references/stimulus-pools.md`](references/stimulus-pools.md). **Mix across categories** — natural world, household, animals, abstractions, geography, ritual, sensory. Avoid clustering; do not draw four plants in a row.

If the user offers a triggering metaphor ("look out the window", "what's in my kitchen"), bias toward that pool but always include 2–3 unrelated stimuli to break the cluster. A fully on-theme batch defeats the purpose of randomness.

Track which stimuli have been used this session. On a second batch, draw fresh ones.

### Step 3: For each stimulus, generate and show the chain

The chain is the artifact, not just the resulting idea. Show every link: the stimulus, its properties, the force-fit jump, the idea.

Open with a one-paragraph framing of why the technique works (first invocation only). Use a visual marker (emoji) per stimulus. Show the property list and the `→` force-fit arrow inline.

Per-stimulus length varies by quality of result. A weak stimulus gets two sentences and abandonment. A strong one gets two to three paragraphs, developed into a concrete direction with precedent where it exists.

### Step 4: Embrace abandonment

Roughly 1 in 5 stimuli will not pay off. **Show this explicitly**, for example: "🪡 The threading of a needle — couldn't bridge to the target without straining. Moving on."

Abandonment is a feature. It signals the method is genuine rather than retrofitted, and it reminds the user that quantity is what creates quality here. Forcing every stimulus to produce a good idea poisons the output.

Hard rule: if the third attempt at a force-fit still feels strained, abandon it. Don't squeeze.

### Step 5: Find the meta-pattern

After the batch, scan across the *ideas that landed* for a structural property that kept recurring — "all the strong hits had time or slowness as a feature", "three of the strongest cast the user as a defender, not a buyer", "most of these turned out to be community products, not tools".

This cross-stimulus observation is often where the deepest insight lives. State it explicitly. Name it mid-batch if it emerges before the end.

### Step 6: Honest ranking, no closure pressure

Pick the 3–5 sharpest directions. Say which feel weak, and why. Do not push the user to commit.

End with an explicit offer: pull more stimuli, go deeper on one direction, switch technique, or stop. The user controls when the technique ends.

## Honesty mechanics

**Abandonment rule:** if the third force-fit attempt on a stimulus still strains, abandon it visibly and move on. A batch where every stimulus produces a viable idea is a tell that the output is fabricated — expect 1–3 abandonments per batch of 8–12.

**Meta-pattern step:** never skip Step 5. The individual ideas matter less than the structural insight that emerges across them.

## What NOT to do

- **Don't sanitize weird ideas.** The unexpectedness is the value. If a force-fit produces something edgy or impractical, ship it as a direction; don't soften it.
- **Don't force every stimulus to produce a viable idea.** Abandonment is honest output.
- **Don't repeat stimuli** across batches in the same session.
- **Don't skip the meta-pattern step.** It is where the gold is.
- **Don't push the user toward a decision.** The technique is divergent; convergence belongs to the user.
- **Don't run more than ~15 stimuli per batch.** Returns diminish and quality suffers.

## References

- [`references/stimulus-pools.md`](references/stimulus-pools.md) — categorized stimulus inventory to draw from
- [`references/worked-example.md`](references/worked-example.md) — a real session showing the full shape, abandonments included
