# Make It Sticky: reference guide for agents

<!--
SPDX-FileCopyrightText: 2026 Alexander Samuel Ricciardi (Omegapy)
SPDX-License-Identifier: Apache-2.0
Original project: https://github.com/Omegapy/Make-It-Sticky
-->

This file supplements the [Make It Sticky skill](../SKILL.md) with prompt patterns and examples. The skill's main workflow is complete without this file.

## Quick prompts

**One explanation**

> Explain [TOPIC] with the Make It Sticky method. Give me an accurate explanation, a short sticky, and a sentence showing what the sticky represents.

**Interactive tutoring**

> Teach me [TOPIC] with the Make It Sticky method. Use analogies often when they help me picture the idea, and add a little humor now and then if it helps me remember. Revisit earlier stickies in new examples.

**Interactive tutoring with Quick Check on**

> Teach me [TOPIC] with the Make It Sticky method and turn on Quick Check. Ask one recall question at a time and wait for my answer before giving feedback.

**Technical document**

> Explain [TOPIC] clearly. Use a concise sticky only where it makes a difficult concept easier to understand. Preserve equations, conditions, limitations, and exact terminology.

**Review session**

> Test my understanding of the stickies from this conversation. Ask one question, wait for my reply, then give feedback and the next question.

**Try a different anchor**

> That sticky did not work for me. Keep the technical explanation, but use a different analogy or concrete example.

## Additional examples

### Prioritization

**Explanation:** Prioritization selects what matters most under current goals, urgency, effort, and constraints.

**Sticky:** "A to-do list is the entire menu; a priority is what you actually order."

**Map and limit:** The menu is the complete set of possible tasks. The order is what you choose to do. Some tasks remain mandatory even when they are not appealing.

### A machine-learning validation set

**Explanation:** A validation set helps compare model choices during development using examples kept separate from the data used to fit the model. A final test set serves a different role: estimating performance after choices are made.

**Sticky:** "Practice on your homework; check your choices with practice exams; save the final exam for the end."

**Map and limit:** Homework represents training data, practice exams represent validation data, and the final exam represents the held-out test set. This analogy assumes the datasets remain appropriately separated; repeated use of the test set for tuning undermines that separation.

## Teaching decisions

- **Already understood:** A short contrast may be enough.
- **Confusing mechanism:** Start with the correct steps. Use a sticky only after the learner has an accurate starting point.
- **Repeated confusion:** Change the representation. Try a physical example, a numerical example, or a counterexample.
- **Quick Check:** When the learner has opted in, prefer a short question that asks them to use the idea in a new case.
- **Long conversations:** Reuse an earlier sticky when it is available and relevant, but do not pretend to remember something that is not in context.

A sticky succeeds when a learner can explain the concept correctly without relying on the metaphor.
