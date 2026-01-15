---
layout: practice
title: Dark Launch
title_mark: Dark Launch
published_date: 2026-01-15
refactored_date: 2026-01-15
areas:
  - devops
excerpt: Deploying changes in a way that separates delivery from exposure so teams can learn and reduce risk before full release.
icon: fa-moon
---
### What is this practice?

Dark launch is the practice of deploying changes without immediately exposing them to all users. It separates getting code into production from turning a capability on.

This can be accomplished through techniques like feature flags, gradual rollouts, or limiting exposure to internal users or small cohorts.

---

### Why does this matter in this transformation?

During a cloud migration, teams need to make frequent changes while keeping customer impact and operational risk under control. Releasing everything at once raises the cost of mistakes and slows learning.

Dark launch supports the transformation by allowing teams to ship incrementally, observe real behavior, and expand exposure only as confidence grows.

---

### What does “good” look like?

When dark launch is working well, teams can deploy frequently with low drama. Changes are observable in production before broad exposure, and rollback or disablement is fast if risk appears.

Learning happens earlier, and the blast radius of surprises is contained.

---

### What gets in the way?

Common challenges include insufficient observability, unclear criteria for expanding exposure, poor hygiene around feature flags, and organizational pressure to treat a launch as a single event.

Teams can also mistake dark launch for “hiding work,” rather than using it to learn safely and reduce risk.

---

### How might someone begin?

Many teams begin by choosing one small capability that can be gated and rolled out gradually, then defining simple criteria for increasing exposure.

Starting with internal users or a small cohort, and learning how to observe and respond before scaling rollout, builds confidence without requiring complex tooling upfront.

---

### Explore deeper with your AI assistant

Use your AI assistant to reason through this practice in your own context.

**Prompt:**

I’m exploring the practice of dark launch in the context of a cloud migration and broader organizational change.

Help me reason through this practice by:

- explaining it in plain language without assuming specific tools or frameworks
- highlighting the tradeoffs and tensions it introduces
- describing what “good” tends to look like in real teams
- calling out common failure modes or misunderstandings
- suggesting small, low-risk ways teams often begin experimenting
- articulating who are the vendor-neutral thought leaders in the space

Please keep the discussion exploratory and context-aware rather than prescriptive.
