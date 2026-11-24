# Make It Sticky

<!--
SPDX-FileCopyrightText: 2026 Alexander Samuel Ricciardi (Omegapy)
SPDX-License-Identifier: Apache-2.0
Original project: https://github.com/Omegapy/Make-It-Sticky
-->

**Make It Sticky** is a way to explain ideas so they are easier to understand, remember, and use. It starts with an accurate explanation and adds a short memory anchor. The optional [Quick Check](Make-It-Sticky-Method.md#quick-check) gives the learner a chance to recall or apply the idea and is off by default.

A memory anchor, called a *sticky*, might be a concrete image, an analogy, a contrast, or a sentence that captures the main mechanism. The anchor supports the explanation. It never replaces it.

This repository contains two ways to use the same method:

- **[Make It Sticky method](Make-It-Sticky-Method.md):** A readable guide with examples and prompts, including a prompt you can use to request this preference in ChatGPT Memory.
- **[Make It Sticky skill](make-it-sticky/README.md):** A reusable set of instructions for AI agents. Use it when you want to apply the method without relying on saved memory.

## Which one should I use?

If you want an AI assistant to consider your learning preference across conversations, start with the [method guide](Make-It-Sticky-Method.md) and its memory prompt. Whether that preference is retained depends on the assistant's memory settings and behavior.

If you want a portable, versioned set of instructions for an agent or project, use the [skill folder](make-it-sticky/). It contains its own `SKILL.md`, `README.md`, and reference material. You can copy the folder without copying the rest of this repository.

For a single conversation, you can simply say:

> Explain this with the Make It Sticky method.

The method works across subjects, including machine learning, programming, mathematics, science, writing, and everyday planning. Use it where an anchor improves understanding, not where an analogy would get in the way.

## Files

```text
Make-It-Sticky/
├── README.md
├── LICENSE
├── NOTICE
├── Make-It-Sticky-Method.md
└── make-it-sticky/
    ├── README.md
    ├── LICENSE
    ├── NOTICE
    ├── SKILL.md
    └── references/
        └── method-guide.md
```

## The basic idea

**Explain accurately. Make it memorable. Retrieve and apply it.**

A good sticky helps someone remember how something works, not just what it is called.

## License and attribution

Created by **Alexander Samuel Ricciardi (Omegapy)**. See [NOTICE](NOTICE) for the author's other aliases and the original project attribution.

The Make It Sticky method, skill, and accompanying documentation are licensed under the [Apache License 2.0](LICENSE). You may use, adapt, and redistribute the licensed material, including commercially, subject to the license. When redistributing copies or derivative works, include the license, preserve applicable copyright and attribution notices (including the attribution in NOTICE), and identify modified files as required by Section 4.

When copying the skill as a standalone folder, keep its LICENSE and NOTICE files with it. Attribution in lessons, generated explanations, or other materials that merely use the method is appreciated but is not an additional license condition.

Suggested credit: *Make It Sticky method by Alexander Samuel Ricciardi (Omegapy), https://github.com/Omegapy/Make-It-Sticky.*
