 📖 *Story context: Shiva at SriTech moves company data to the cloud and learns the foundations of security thinking.*
 
---
 
## 1. Shared Responsibility Model 🏢
 
**Question:** If something goes wrong in the cloud, whose fault is it?
**Answer:** Depends on the service model — like renting property:
 
| Model | Analogy | Who does what |
|---|---|---|
| **On-premises** | Own house | You own & manage everything |
| **IaaS** | Empty flat | Microsoft: building (hardware, network). You: OS, apps, data |
| **PaaS** | Furnished flat | Microsoft: building + furniture (OS, runtime). You: apps & data |
| **SaaS** | Hotel room | Microsoft: almost everything |
 
⭐ **Exam-critical:** These are ALWAYS the customer's responsibility, in every model:
- **Data**
- **Devices**
- **Accounts & identities**
*(Real-world tie-in: Exchange Online is SaaS, but tenant data backup is still the customer's job — hence third-party tools like Datto.)*
 
---
 
## 2. Zero Trust 🛡️
 
Old model: castle & moat — trusted once inside. ❌
**Zero Trust: "Never trust, always verify."** ID checked at every door, every time.
 
**Three principles:**
1. **Verify explicitly** — authenticate & authorize using all data points (identity, location, device health)
2. **Least privilege access** — just enough access (JEA), just in time (JIT)
3. **Assume breach** — act like the attacker is already inside: segment, encrypt, monitor
---
 
## 3. Defense in Depth 🧅
 
Security in layers — attacker must peel through all of them:
 
**Physical → Identity & Access → Perimeter → Network → Compute → Application → Data**
 
---
 
## 4. CIA Triad 🔺
 
The goal of all those layers — protect the data at the center:
 
- **Confidentiality** — only the right people can see it (encryption)
- **Integrity** — data hasn't been tampered with (hashing)
- **Availability** — accessible when needed (backups, redundancy)
---
 
## 5. Encryption & Hashing 🔐
 
| Concept | Analogy | Example |
|---|---|---|
| **Encryption at rest** | Data sleeping on disk, locked | BitLocker, storage encryption |
| **Encryption in transit** | Armored van on the road | HTTPS / TLS |
| **Hashing** | Fingerprint of data — one-way, irreversible | Password storage, integrity checks |
 
⭐ Hashing ≠ encryption. Hashing cannot be decrypted.
 
---
 
## 6. Data Residency & Compliance 🌍
 
- **Data residency** = laws governing *where* data physically lives (which country/region's datacenter)
- Different regions → different regulations (e.g., GDPR)
- Why Microsoft lets tenants choose their geo
- Deep dive comes in Part 4 (Microsoft Purview) 🌱
---
