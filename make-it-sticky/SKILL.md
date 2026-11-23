---
name: make-it-sticky
metadata:
  version: "1.2.0"
description: Teach or clarify ideas using the Make It Sticky method. Explain accurately, create a concise memory anchor (a "sticky"), and map it to the real mechanism and its important limits. Offer an optional Quick Check for recall or application. Use when asked to "make it sticky," use the "Make It Sticky method," or use the "Make It Sticky skill"; also apply selectively to difficult explanations.
---

# Make It Sticky skill

## Purpose

Help people understand and retain ideas by pairing accurate explanations with short, memorable connections called **stickies**. A sticky may be an analogy, mental image, concrete example, contrast, or compact phrase. It is a memory anchor attached to a correct explanation, never a replacement for one.

Use the method across domains when it improves understanding, not only in machine learning or education.

## When to use it

- Apply the method when a user explicitly asks for the **Make It Sticky method**, the **Make It Sticky skill**, or asks to **make an explanation sticky**.
- Consider using it when explaining a difficult mechanism, several interacting steps, an easily confused distinction, or a decision with meaningful tradeoffs.
- Adapt to the person's background, the available context, the requested depth, and whether the response is spoken or written.
- Do not force it into short factual answers, formal artifacts, emotionally sensitive topics, source-bound verbatim work, or responses where a metaphor would distort the point. Honor requests to skip analogies or questions.

## Quick Check

Quick Check starts off for each new use of the method, whether it is one explanation or an ongoing tutoring session. At the start, ask in chat, “Do you want me to activate Quick Check?” Continue with the explanation in the same reply when the topic is known.

Activate Quick Check only after a clear yes or an explicit request to turn it on or be quizzed. A no, an unclear answer, or no answer leaves it off. If the user already specified on or off, apply their choice without asking again. Keep the choice for the current use, and honor any request to turn it on or off later. Without an interactive chat, leave it off unless the user explicitly requested it.

When it is on and the learner can respond, ask one specific recall or application question at a time. Let the learner answer before giving feedback. Keep these questions in the conversation when the main deliverable is an artifact.

## Teaching workflow

1. **Explain.** State the correct idea in clear language. Give enough context to understand the mechanism, while keeping necessary technical terms, mathematics, conditions, and caveats.
2. **Anchor.** Create one compact sticky tied to the real mechanism. Use analogies often when a familiar comparison makes the idea easier to picture. Occasionally add a little humor when it suits the learner and helps them remember the idea. Use an example, image, contrast, or short phrase when it fits better.
3. **Map.** Briefly show what the sticky's important parts represent. Name a limitation when taking the analogy literally could mislead.
4. **Check, if enabled.** Ask a brief recall or application question as described above.
5. **Reinforce.** When the earlier sticky is available in context, reuse it in a later relevant example. Ask the learner to apply it only if Quick Check is on.

## Response guidance

- The answer must remain correct and useful even if the sticky is removed.
- Generally use one sticky per main concept. Keep it to one or two sentences unless more detail is needed to prevent misunderstanding.
- Weave the anchor into the explanation naturally. A **Sticky:** label can help in lessons but is not required.
- Distinguish an illustrative analogy from evidence, and preserve material uncertainty and exceptions.
- Use the user's provided material as the authority for source-based tasks. Do not add unsupported facts to make an example more colorful.
- If a sticky does not connect with the learner, try a materially different example rather than restating the same analogy.

## Examples

### K-nearest neighbors (KNN)

**Explanation:** In classification, KNN uses the labels of the nearest *k* training points. Very small *k* can be sensitive to noise; too-large *k* can hide local patterns.

**Sticky:** "Ask one person for directions and you might pick the one holding the map upside down. Ask a few people nearby and one bad answer carries less weight. Ask the whole city and people across town can drown out the local advice."

**Map and limit:** The person with the upside-down map represents a noisy neighbor. At *k* = 1, that one answer decides the prediction. A few people nearby represent a moderate *k*, and the whole city represents an excessively large *k*. The best *k* depends on the data.

**Quick Check (if enabled):** Why might *k* = 1 make a poor prediction near a mislabeled point?

### Parameters versus hyperparameters

**Explanation:** A fitted model learns parameters from training data. Hyperparameters determine aspects of the model or its training and are configured or selected through tuning.

**Sticky:** "Parameters are learned. Hyperparameters set the learning rules."

**Map and limit:** The difference concerns ordinary model fitting versus configuration and tuning, not who physically enters a value.

### Functions and arguments

**Explanation:** A function defines reusable behavior. Arguments supply values for a particular call.

**Sticky:** "The function is the recipe; the arguments are today's ingredients."

**Map and limit:** Recipe means reusable procedure; ingredients mean inputs. Real functions can also produce side effects or accept complex values.

## Quality check

Before responding, confirm that the explanation is correct, the sticky maps to the mechanism, important limitations are clear, and the analogy fits the audience and situation. Keep the output focused on the user's actual question.

## More detail

See [`references/method-guide.md`](references/method-guide.md) for prompts and optional teaching variations. This `SKILL.md` is complete on its own; the reference is supplemental.
