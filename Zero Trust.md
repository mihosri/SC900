# SC-900 | Part 1: Zero Trust Model 🛡️

> 📖 *"Never trust, always verify." The castle-and-moat is dead — attackers phish their way inside, so nothing is trusted by default.*

⭐ **Zero Trust is a STRATEGY, not a product.** You can't buy it in a box.

---

## The 3 Guiding Principles

| Principle | Meaning | Key terms |
|---|---|---|
| **Verify explicitly** | Authenticate using ALL signals, not just password | Identity, location, device compliance, app, data sensitivity, anomalies |
| **Use least privileged access** | Minimum access, minimum time | ⭐ **JIT** (just-in-time) + **JEA** (just-enough-access), risk-based adaptive policies |
| **Assume breach** | Attacker is already inside — limit damage | Segmentation, end-to-end encryption, monitoring & analytics |

---

## 🆕 The 7 Foundational Pillars

> Memory hook: "**I D**rink **A**pple juice **D**aily **I**n **N**ice **V**enues" 🧃
> Structure: 6 pillars = things defended & signal sources · 7th = control room watching all six

| Pillar | Key points |
|---|---|
| **Identities** 👤 | Users, services, devices. Strong auth + least privilege. ⭐ "Identity is the primary control plane" — most attacks abuse an identity |
| **Devices** 💻 | Every device = potential entry point. Health/compliance status drives access decisions (→ Intune) |
| **Applications** 📱 | Visibility into ALL apps incl. ⭐ **shadow IT** (unsanctioned apps); manage app permissions |
| **Data** 💎 | Classify, label, encrypt. ⭐ "Data must carry its own protection" — safe even outside your environment |
| **Infrastructure** 🏗️ | Assess version currency, config compliance, anomalies. JIT admin access |
| **Networks** 🕸️ | Segmentation + ⭐ **micro-segmentation** (walls within zones), E2E encryption, monitoring |
| **Visibility, Automation & Orchestration** 🎛️ | Integrating layer — aggregates & correlates signals from all six. ⭐ **SIEM** = detects (ingests/correlates) · **SOAR** = responds (automated playbooks) → Microsoft Sentinel in Part 3 |

---

## Zero Trust in Practice 🎬

Scenario: sign-in from unfamiliar location + unmanaged device + accessing sensitive finance app:
- Each pillar flags its own signal (weird location, non-compliant device, policy violation...)
- Alone = six low-severity logs. **Correlated by pillar 7 = one high-confidence risk detection**
- Automated response: step-up auth, block app, alert security team — no human needed

---
