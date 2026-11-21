# Make It Sticky skill

This folder contains the **Make It Sticky skill**, a reusable set of instructions for AI agents that teach or explain concepts. It uses accurate explanations, concise memory anchors called *stickies*, and recall practice when appropriate.

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

The agent should explain the idea correctly first, make one useful memory connection, relate that connection to the actual mechanism, and mention any important limit. In a tutoring session it can ask a question and return to the same anchor later.

The skill should not add a quiz to every answer or invent a metaphor for every topic. It should respect the user's requested depth, the available evidence, and the purpose of the response.

## Skill versus memory

The skill and saved memory provide two different entry points to the same method. The skill contains explicit instructions for the agent to follow when loaded. A memory preference tells a memory-enabled assistant what learning style you like, but it does not guarantee a fixed workflow.

To request the preference in ChatGPT Memory instead, see the [memory prompt in the method guide](../Make-It-Sticky-Method.md#prompt-to-request-a-saved-memory-preference).
