# SC-900 | Part 1: Shared Responsibility Model (Updated — includes AI) 🏢

> 📖 *Story context: Shiva at SriTech learns who's accountable for what in the cloud — and meets the new AI intern, Copilot.*

---

## 1. The Cloud Service Models (Apartment Analogy)

| Model | Analogy | Provider handles | You handle |
|---|---|---|---|
| **On-premises** | Own house | Nothing | Everything — building to data |
| **IaaS** | Empty flat | Datacenter, network hardware, hosts | OS, apps, network controls, data |
| **PaaS** | Furnished flat | + OS, runtime | App code, config, access, data |
| **SaaS** | Hotel room | Entire app stack | Access mgmt, data, tenant settings |

📈 Higher up the stack = more delegated to the provider. But delegation ≠ zero responsibility.

---

## 2. ⭐ Responsibilities You ALWAYS Retain (D-I-E-C)

> Memory hook: *"Misconfigure it and your data can DIE-C"* 💀

1. **Data** — what you collect, who accesses it, retention, encryption decisions
2. **Identities & access** — accounts, MFA, least privilege (one stolen keycard bypasses everything)
3. **Endpoints** — laptops/phones/tablets; a compromised device = the legitimate user
4. **Configuration choices** 🆕 — misconfigured storage or over-permissive policies expose data even on a perfectly secured platform

---

## 3. Cloud Security Advantages

- Providers invest at scale: physical security, patching, compliance certs, threat intelligence, 24/7 monitoring
- On-prem gaps happen because teams are stretched thin (delayed patches, aging hardware)
- Cloud shift = focus your energy on the D-I-E-C items only you can do

---

## 4. 🆕 AI Shared Responsibility Model 🤖

> Analogy: Copilot = a super-smart intern at SriTech

| Layer | Analogy | Who's responsible |
|---|---|---|
| **AI platform** | Intern's brain & body (model, infra, built-in content filters) | Provider (Microsoft) |
| **AI application** | Intern's desk setup (connectors, data sources, plugins, config) | Shared / mostly you |
| **AI usage** | What people ask the intern + rules you set | Entirely you |

**Landmarks:** Microsoft 365 Copilot = **SaaS AI** · Azure AI Foundry = **PaaS AI**

### Your AI responsibilities:
- Protect data the AI can access (access controls, governance)
- Identity & access — who can use AI, what they can do
- Safe configuration — connectors, logging, retention
- ⭐ **Mitigate prompt injection** — attacker hides malicious instructions in input/external data to manipulate AI behavior. Defenses: input validation, access controls, monitoring
- User training & acceptable use policies — yes, this is officially a security control!

---

## 5. Key Takeaway 🎯

> You can **delegate the work**, but you never delegate **accountability** — for your data, identities, endpoints, and how the technology is used.

---
