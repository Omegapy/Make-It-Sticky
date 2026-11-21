# The Make It Sticky method

Some concepts make sense when you hear them but are hard to recall later. The **Make It Sticky method** adds a memorable connection to a clear explanation, then uses recall and practice to help the idea stay available.

## What is a sticky?

A **sticky** is a short memory anchor attached to an accurate explanation. It can be an analogy, a mental image, a concrete example, a useful contrast, or a compact phrase.

A sticky is not a substitute for understanding. It should make the underlying idea easier to retrieve, not change what the idea means.

> **Principle:** Explain it accurately. Make it memorable. Retrieve and apply it.

## When to use the method

Use Make It Sticky across subjects, including machine learning, programming, mathematics, science, writing, project planning, and everyday decisions. It is especially useful when a mechanism has several parts, two concepts are easy to confuse, or a new idea needs to connect to something familiar.

Do not force a metaphor into a simple factual answer, a formal artifact, or a sensitive discussion. If an analogy hides an important exception or makes the subject less clear, leave it out.

## How the method works

1. **Explain.** State the concept correctly, with enough context to understand it. Keep necessary technical terms and conditions.
2. **Anchor.** Choose one memorable connection. Prefer an image, analogy, example, contrast, or short phrase that reflects how the concept works.
3. **Map.** Connect the parts of the anchor to the actual concept. Point out where the analogy stops being accurate if that limit matters.
4. **Check.** In a teaching conversation, ask a brief recall or application question. Let the learner answer before giving feedback.
5. **Reinforce.** Revisit the same anchor later and apply it to a different example. Recall is more useful than simply rereading the explanation.

Keep each sticky concise. The goal is a helpful connection, not a performance or an elaborate story.

## Examples

### Machine learning: k-nearest neighbors (KNN)

**Explanation:** For classification, KNN predicts a label using the labels of the *k* nearest training examples. With a very small *k*, one noisy neighbor can have a large effect. If *k* is too large, nearby patterns can get lost among distant examples.

**Sticky:** "Ask one stranger for directions and you may get bad advice. Ask a small crowd and the answer is steadier. Ask the whole city and the local knowledge gets drowned out."

**How it maps:** One stranger represents *k* = 1, the small crowd represents a moderate *k*, and the whole city represents an excessively large *k*. This is a way to remember the tradeoff, not a rule that increasing *k* always improves predictions.

**Recall:** Why might KNN with *k* = 1 be sensitive to a mislabeled training point?

### Machine learning: parameters and hyperparameters

**Explanation:** In many fitted models, parameters, such as logistic regression coefficients, are learned from training data. Hyperparameters, such as regularization strength, are configured or selected through tuning outside that ordinary fitting step.

**Sticky:** "Parameters are learned. Hyperparameters set the learning rules."

**How it maps:** Model fitting estimates parameters. Configuration and tuning select hyperparameters. The distinction is about their roles in training, not simply whether a person typed a value.

### Programming: functions and arguments

**Explanation:** A function defines reusable behavior. Arguments are the values supplied for a particular call.

**Sticky:** "The function is the recipe; the arguments are today's ingredients."

**How it maps:** The recipe is the reusable procedure, and the ingredients are the supplied inputs. Unlike a recipe, a function may have side effects, and arguments may themselves be functions or complex objects.

### Everyday planning: priorities

**Explanation:** Prioritization selects what matters most given current goals, urgency, effort, and constraints.

**Sticky:** "A to-do list is the entire menu; a priority is what you actually order."

**How it maps:** The menu represents the possible tasks, and the order represents the tasks selected for attention. Some obligations still have to be done regardless of preference.

## How to ask an AI assistant to use it

You can use the method for one answer, an entire tutoring session, or an explanation inside a document.

**Short request**

> Explain this using the Make It Sticky method.

**Teaching request**

> Teach me [TOPIC] with the Make It Sticky method. Explain the concept accurately and briefly, then give me one memorable sticky. Tell me how it maps to the real concept and where the analogy breaks down. Ask one recall or application question and let me answer. Bring back the same sticky later when it helps.

**For a document**

> Explain [TOPIC] in clear, professional language. Use the Make It Sticky method for difficult concepts, but keep the technical explanation complete and do not force analogies into every paragraph.

**For recall practice**

> Quiz me on the stickies we have used in this conversation, one at a time. Do not reveal the answer until I respond. If I struggle, give me a hint before the full explanation.

### Prompt to request a saved memory preference

If you use ChatGPT Memory and want the method considered across conversations, you can ask ChatGPT to remember this preference:

> Remember that I prefer the **Make It Sticky method** when learning or discussing complex ideas. First explain the idea accurately, with enough context to understand it. When it helps, add a short memorable sticky, show how it maps to the real concept, and identify important limits. In interactive tutoring, ask me a brief recall or application question and revisit earlier stickies when relevant. Do not force analogies into simple answers, formal writing, or sensitive topics. Refer to this preference as the **Make It Sticky method**, not by an earlier name.

A memory preference may influence future answers, but it is not a guarantee that every response will follow a strict procedure. You can explicitly request the method when you need it. Saving or updating memory depends on the chat product and its settings.

## Memory, prompts, and the reusable skill

| Option | What it does | Best use |
| --- | --- | --- |
| **Memory preference** | Tells a memory-enabled assistant about your preferred way to learn | Personalization across conversations |
| **Prompt** | Requests the method for one answer or session | A specific learning task |
| **[Make It Sticky skill](make-it-sticky/README.md)** | Defines reusable agent instructions independent of saved memory | Projects, multi-agent workflows, sharing, and versioning |

The skill is stored in a separate folder with its own `SKILL.md` and `README.md`. A file named `SKILL.md` does not automatically install a skill in ChatGPT or every agent environment. Follow the instructions for the platform where you want to use it.

## Quality check

Before using a sticky, ask whether it meets these tests:

- Is the underlying explanation correct?
- Does the anchor help recall the mechanism rather than merely the label?
- Is the mapping clear, including an important limit when needed?
- Is it short enough to remember?
- Can the learner explain or apply the idea without the analogy?

**Core rule:** A good sticky makes the truth easier to retrieve, not easier to misunderstand.
