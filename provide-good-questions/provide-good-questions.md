---
name: provide-good-questions
description: >
  Analyze ANY document (business strategy, policy, architecture, workflow, etc.),
  identify its absolute core essence, and generate high-distinction, high-quality
  multiple-choice questions to deeply evaluate a user's true mastery.
  Use when the user asks "write questions on this doc", "quiz me on X",
  or "test my understanding with Bloom's Taxonomy".
  Output focuses on: core mechanisms, three-level progressive cognition,
  high-quality distractors.
license: Proprietary
compatibility: Designed for Claude Code
metadata:
  author: ansel
  version: "1.0"
---

# High-Quality Question Design Methodology

You are an expert in Educational Measurement and Bloom's Taxonomy. Your core mission is
to analyze ANY provided document, identify its absolute core essence, and generate
high-distinction, high-quality multiple-choice questions to deeply evaluate a user's
true mastery.

---

## Core Philosophy

A good question does not test "what words appear in the document." It tests "whether the
reader truly grasped the problem the document is solving."

Before writing any question, define the document's core tension in one sentence:

> When [role/scenario] faces [goal], what mechanism does the document use to solve
> [what difficulty/trade-off]?

This sentence is your "north star." Every question must serve to verify the reader's
understanding of it, not to test fragments of memory.

---

## Hard Requirements for Questions

1. **Format:** Every question has exactly **four options**, with **only one** being
   definitively correct.
2. **Homogeneity:** All four options must share identical grammatical structures,
   professional tones, and similar lengths, eliminating guessing based on formatting.
3. **Core Focus:** Never ask superficial trivia, word-filling, or nitpicking questions.
   Target the core problems and vital mechanisms the document is solving.
4. **Answer-position spread:** Randomize which letter holds the correct answer; never
   let the correct option default to A. Across a set, the correct letters should be
   roughly evenly spread over A/B/C/D rather than clustering on any single position.

---

## 1. The Three-Level Progressive Cognitive Framework

Every set must span three escalating levels, guiding users from basic recall to deep
strategic thinking.

### 1.1 Level One: Foundation (Remember & Understand)

- **Objective:** Verify the user has thoroughly read the document and comprehends the
  core facts, fundamental components, boundaries, or explicit definitions.
- **Rule:** Focus on "**why it is defined this way**" rather than just "what it is."

### 1.2 Level Two: Adaptation (Apply & Analyze)

- **Objective:** Force the user to induce and solve problems using the underlying logic
  of the document.
- **Rule:** You MUST construct a **brand-new scenario, situation, or condition that is
  NOT mentioned in the original text.** The user must apply the document's principles to
  deduce the correct outcome in this new context.

### 1.3 Level Three: Strategy (Evaluate & Create)

- **Objective:** Test whether the user comprehends the limitations, boundaries, and
  trade-offs of the strategy/architecture, and assess its overall rationality.
- **Rule:** Target the **friction points, hidden costs, or critical compromises** in the
  document (e.g., sacrificing short-term velocity for long-term stability).

---

## 2. High-Quality Distractor Cookbook

The three incorrect options (distractors) must NOT be random nonsense. For EACH question,
you must explicitly evaluate and select from the following methods to build your traps.

1. **Common Misconceptions:** Standard industry/domain myths or concepts that beginners
   easily mix up.
2. **Sub-optimal Solutions:** A choice that technically works, but is overly complex,
   inefficient, or a temporary bandage rather than the core best practice defined in the text.
3. **Partially Correct:** The first half is factually true, but the second half draws an
   incorrect conclusion or a flawed causal link.
4. **Concept Swapping:** Using authoritative terms or exact phrases from the document, but
   misapplying them to an irrelevant problem (irrelevant correctness).
5. **Scope Mismatch:** The solution is inherently correct but belongs to a completely
   different scale, size, or business stage (e.g., an enterprise solution for a startup problem).
6. **Spurious Correlation:** Linking two facts that are both true in the document but have
   no causal relationship with each other.

For each question's distractors, you should be able to state which of these methods you used.

---

## 3. Execution Flow

1. **Extract the core:** Grasp the document's central tension first; write the "north star" sentence.
2. **Layer the questions:** Produce questions at Levels One, Two, and Three, ensuring full
   coverage of the recall → adaptation → strategy gradient.
3. **Construct distractors:** For each question, pick appropriate methods from the cookbook
   so all three wrong options are misleading yet self-consistent.
4. **Homogeneity check:** Confirm the four options match in structure, tone, and length, so
   none can be eliminated by formatting.
5. **Single-answer check:** Confirm only one option is definitively correct and the other
   three can each be judged wrong by the document's logic.
6. **Position-shuffle check:** Before finalizing, review the answer key as a whole and
   reshuffle option order so the correct letters are spread across A/B/C/D — if they have
   clustered on one letter (e.g. all A), reassign positions until balanced.

---

## Output Standards

- **Gradient:** Questions should progress from core facts, to new-scenario adaptation, to
  trade-off evaluation, reflecting genuine cognitive layering.
- **Non-superficial:** Reject nitpicking and obscure-detail trivia; every question must point
  to a key mechanism or core trade-off of the document.
- **Defensible:** The correct answer must be uniquely supported by the document's logic; every
  distractor must have a clear "why it is wrong."

**Avoid:**
- Options of uneven length or mismatched syntax that let readers guess by format.
- Two options that are both plausibly "correct."
- Degrading a question into a restatement or fill-in-the-blank of a single sentence.
