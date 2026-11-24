# Make It Sticky skill

<!--
SPDX-FileCopyrightText: 2026 Alexander Samuel Ricciardi (Omegapy)
SPDX-License-Identifier: Apache-2.0
Original project: https://github.com/Omegapy/Make-It-Sticky
-->

This folder contains the **Make It Sticky skill**, a reusable set of instructions for AI agents that teach or explain concepts. It uses accurate explanations, concise memory anchors called *stickies*, and optional recall practice.

The skill does not require ChatGPT Memory. An agent can use it whenever the host environment loads the instructions.

## Contents

- [`SKILL.md`](SKILL.md) defines when to use the method, the teaching steps, examples, and quality checks.
- [`references/method-guide.md`](references/method-guide.md) provides extra prompt patterns, examples, and guidance for teaching sessions.

The full, reader-facing method guide is also available in the repository root: [`Make-It-Sticky-Method.md`](../Make-It-Sticky-Method.md). It is not required to run this skill.

## Use the skill

Copy the **entire `make-it-sticky` folder** into a location supported by your agent environment. Some repository-based agents discover skills in a directory such as `.agents/skills/make-it-sticky/`. Other tools use different paths or require a manual setup step, so check your host's instructions.

When the skill is available, requests can be simple:

> Use the Make It Sticky skill to explain how regularization works.

> Make this concept sticky. Then ask me a question to check whether I understand it.

An agent may also use the method proactively for a difficult idea when an analogy genuinely helps.

## What to expect

The agent explains the idea accurately, makes one useful memory connection, relates that connection to the actual mechanism, and mentions any important limit. It adapts the depth to your request and uses a metaphor when it helps explain the topic.

Quick Check is off by default. The agent asks whether to activate it when you begin using the method and can explain the topic while you decide. Say yes to get a brief recall or application question. You can also specify on or off up front or change your choice during the session.

## Skill versus memory

The skill and saved memory provide two different entry points to the same method. The skill contains explicit instructions for the agent to follow when loaded. A memory preference tells a memory-enabled assistant what learning style you like, but it does not guarantee a fixed workflow.

To request the preference in ChatGPT Memory instead, see the [memory prompt in the method guide](../Make-It-Sticky-Method.md#prompt-to-request-a-saved-memory-preference).

## License and attribution

Created by **Alexander Samuel Ricciardi (Omegapy)** and licensed under the [Apache License 2.0](LICENSE). See [NOTICE](NOTICE) for the original project attribution and the author's other aliases.

The LICENSE and NOTICE files are included in this folder so the skill can be distributed independently of the full repository. Keep them with redistributed copies of the skill. Preserve applicable attribution notices and identify modified files as required by Section 4 of the license.

Suggested credit: *Make It Sticky skill by Alexander Samuel Ricciardi (Omegapy), https://github.com/Omegapy/Make-It-Sticky.*

Credit in generated explanations that merely use the skill is appreciated, not an additional license condition.
