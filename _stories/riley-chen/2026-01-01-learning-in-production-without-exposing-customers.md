---
layout: story
title: Learning in Production Without Exposing Customers
title_mark: Learning in Production
practitioners:
  - riley-chen
practices:
  - dark-launch
  - hypothesis-driven-experimentation
areas:
  - devops
  - product
published_date: 2026-01-01
refactored_date: 2026-01-01
excerpt: Creating space to learn from real system behavior changed how the team balanced experimentation and customer trust.
---

As the cloud migration progressed, the team faced a familiar tension. They needed to learn how new systems behaved under real conditions, while also protecting customers from instability and surprise.

In the past, this tension had pushed teams toward one of two extremes: defer learning until after release, or avoid experimentation altogether in favor of predictability. Neither approach held up under the pace and complexity of the migration.

The team began exploring ways to observe real system behavior without fully exposing customers to change. Instead of treating release as a single moment, they introduced controlled exposure that allowed parts of the system to operate under new conditions while most customers remained unaffected.

This didn’t remove uncertainty. Early signals were sometimes ambiguous, and interpreting them required care. A small number of unexpected interactions surfaced, raising questions about whether the experiments themselves were introducing new risk.

What became clear, however, was that learning in production didn’t have to come at the expense of customer trust. The team could observe performance characteristics, usage patterns, and system interactions that were impossible to simulate in test environments, while keeping exposure bounded.

There were tradeoffs. Running experiments alongside live systems added operational overhead. Decisions about when to expand exposure relied on judgment rather than automation. Not every hypothesis produced clean answers.

Still, the practice changed how the team related to uncertainty. Instead of waiting for confidence to arrive before acting, they learned to design change so that uncertainty was visible, limited, and reversible.

Over time, this shifted decision-making upstream. Questions about impact surfaced earlier. Assumptions were tested in smaller ways. Course corrections became easier to make without triggering disruption.

**Insight:** by learning in production without broadly exposing customers, the team reduced the cost of uncertainty. Decisions became more informed earlier, experimentation no longer required betting customer trust, and leadership gained a safer way to balance innovation and reliability as the migration continued.