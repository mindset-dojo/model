---
layout: practice
title: GitOps
title_mark: GitOps
published_date: 2026-01-15
refactored_date: 2026-01-15
areas:
  - devops
excerpt: Managing system state through version-controlled intent and automated reconciliation to reduce drift and improve reliability.
icon: fa-code
---
### What is this practice?

GitOps is a way of operating systems where the desired state is declared in version control and the running environment is continuously reconciled to match that declared intent.

Instead of treating configuration as something applied manually or remembered implicitly, Git becomes the source of truth for what should be running and why.

---

### Why does this matter in this transformation?

Cloud migration increases the number of environments, changes, and dependencies teams must manage. Manual configuration and undocumented steps create drift, uncertainty, and fragile recoveries.

GitOps supports the transformation by making operational intent explicit, reviewable, and repeatable—so teams can change and recover systems with less hidden risk.

---

### What does “good” look like?

When GitOps is working well, changes to system configuration are visible, reviewable, and traceable. Environments converge toward the declared state, and unexpected drift is detected and corrected quickly.

Teams can reason about what is running and reproduce it reliably across environments, reducing reliance on heroics or tribal knowledge.

---

### What gets in the way?

Common challenges include unclear ownership of operational code, weak review habits, inconsistent environments, and a mismatch between desired state and what teams can safely automate.

Teams may also confuse GitOps with “everything must be automated immediately,” rather than adopting automation progressively and safely.

---

### How might someone begin?

Many teams begin by placing a small but meaningful slice of system configuration under version control, using pull requests as the mechanism for review and change.

Starting with one service or one environment, and tightening the loop between declared intent and actual state, often creates early clarity without requiring a wholesale overhaul.

---

### Explore deeper with your AI assistant

Use your AI assistant to reason through this practice in your own context.

**Prompt:**

I’m exploring the practice of gitops in the context of a cloud migration and broader organizational change.

Help me reason through this practice by:

- explaining it in plain language without assuming specific tools or frameworks
- highlighting the tradeoffs and tensions it introduces
- describing what “good” tends to look like in real teams
- calling out common failure modes or misunderstandings
- suggesting small, low-risk ways teams often begin experimenting
- articulating who are the vendor-neutral thought leaders in the space

Please keep the discussion exploratory and context-aware rather than prescriptive.
