# SC-900 | Part 1: Defense in Depth & CIA Triad 🧅

> 📖 *One wall can fail. Layers slow attackers down and buy time to detect them.*

---

## The 7 Layers (outside → in)

> Memory hook: "**P**lease **I** **P**romise **N**ot to **C**ompromise **A**ny **D**ata"

| Layer | What it does | Key controls |
|---|---|---|
| **Physical** | Protect the hardware itself | Guards, badges, cameras, locked facilities |
| **Identity & access** | Verify who you are | MFA, RBAC, Conditional Access ⭐ (stops even stolen passwords) |
| **Perimeter** | Guard the network boundary | DDoS protection, perimeter firewalls |
| **Network** | Limit movement inside | Segmentation, NSGs ⭐ (limits damage *after* compromise) |
| **Compute** | Protect VMs/containers | Patching, close unused ports, restrict admin ⭐ (unpatched = top entry point) |
| **Application** | No exploitable code | Input validation vs. SQL injection & XSS; test before production |
| **Data** 💎 | The treasure at the center | Access controls, encryption, classification |

**Why layers:** each one slows the attacker + adds detection chances. Design as if the outer wall WILL fall (assume breach → connects to Zero Trust).

---

## CIA Triad 🔺

| Property | Meaning | Controls | Attack examples |
|---|---|---|---|
| **Confidentiality** | Only authorized eyes | Encryption, access controls, policies | Data breach / theft |
| **Integrity** | Accurate, untampered (⭐ deletion counts too!) | Hashing, digital signatures, audit logs | Tampering, unauthorized deletion |
| **Availability** | Accessible when needed | Redundancy, failover, backups, DDoS protection | DDoS, ⭐ ransomware (= availability attack!) |

### ⭐ The triad has tradeoffs
- Encrypt everything but lose the keys → data gone forever (C vs. A)
- Heavy auth → secure but kills productivity
- Security = **risk-based balance**, not maximum everything

### Attack classifier 🎯
Steal data → **C** · Modify/delete → **I** · Take offline → **A**

---
